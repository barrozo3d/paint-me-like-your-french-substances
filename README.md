# Paint Me Like Your French Substances

An expert consultant for **Adobe Substance 3D Painter** that also builds its own knowledge base by ingesting tutorials, and can optionally drive a real, running Painter session over MCP.

## What it does

Ask it Substance Painter questions and it answers from a growing library of ingested tutorials plus a hand-written reference knowledge base covering:
- Layer stacks, masks, generators, anchor points, smart materials/masks
- Baking (mesh maps: AO, curvature, normal, position, thickness, ID) and high-to-low poly workflows
- PBR channels, metal/rough vs. specular/glossiness, OpenPBR
- The `substance_painter` Python scripting API and plugin authoring
- Export presets, channel packing, and game-engine (Unreal/Unity/Godot) specifics

It can also write Painter Python for you, and — optionally — connect to a real running Painter session via a third-party MCP server to inspect, edit, bake, and export a live project.

## Quick start

```powershell
git clone https://github.com/barrozo3d/paint-me-like-your-french-substances.git "$HOME\.claude\skills\paint-me-like-your-french-substances"
cd "$HOME\.claude\skills\paint-me-like-your-french-substances"
.\setup.ps1
```

Then just ask Claude Code a Substance Painter question — it reads `SKILL.md` automatically. Full setup and troubleshooting details live in `SETUP.md`.

---

## The Ingest Pipeline, in full detail

This is the part of the skill you'd actually touch to extend it: give it a video, an article, or any source of technical knowledge and the skill will trigger the steps to extract, read, organize, cross-reference and push it.

```
ingest.py  ──►  select_frames.py  ──►  Claude Code (extraction)  ──►  validate.py
(Step 1:         (Step 2:                (Step 3:                    (integrity
 transcript)      frame capture)          structured notes)           check)
```

### `ingest.py` — Step 1: data collection (no API calls, no video download)

| Function | What it does |
|---|---|
| `slugify(text)` | Turns a title into a filesystem-safe slug (`tutorials/<slug>.md`) — lowercases, strips punctuation, collapses whitespace to hyphens, caps at 80 chars. |
| `_ytdlp_cmd()` | Builds the base yt-dlp command. Defaults to forcing the `android` player client to dodge YouTube's "Sign in to confirm you're not a bot" 429s; switches to `cookies.txt`-based auth automatically if that file exists in the skill directory. |
| `check_prerequisites()` | Verifies `yt-dlp` is importable (hard requirement, exits if missing); detects whether `ffmpeg` and `whisper` are available (soft — pipeline degrades gracefully without them). |
| `get_info(url)` | Runs `yt-dlp --dump-json` and parses the result: title, uploader, duration, chapters, video ID. |
| `WHISPER_VOCAB_HINT` | A domain-vocabulary string (Substance Painter terms: smart material, UDIM, Iray, etc.) fed to Whisper as an `initial_prompt` so it transcribes jargon correctly instead of mishearing it. |
| `_load_whisper_model(model_name)` | Loads (and caches) a Whisper model, suppressing the noisy first-download progress bar in favor of one clean notice. |
| `whisper_transcribe(audio_path, model_name)` | Runs Whisper transcription with the vocab hint applied. |
| `download_audio(url, tmp)` | Downloads and extracts audio as mp3 (one automatic retry on YouTube throttling failures). |
| `ytdlp_captions(url, tmp)` | Fallback path when Whisper isn't installed or transcription fails: pulls YouTube's own auto-captions and strips VTT markup down to plain text (no per-sentence timestamps in this path). |
| `segment_by_chapters(transcript, chapters)` | Buckets the transcript into per-chapter sections (or one "Full Content" section if the video has no chapters), preserving a per-sentence `(timestamp, text)` list per section — this is what lets Step 2 pick *content-anchored* frame moments instead of guessing blind percentages. |
| `download_video_low(url, tmp)` | Downloads the lowest-quality video stream available (reused by `select_frames.py` — frame pixels don't need to be high-res). |
| `extract_frames(video_path, timestamps, out_dir)` | Runs `ffmpeg -ss <t> -frames:v 1` per timestamp to grab exact stills. |
| `_detect_hallucination(text)` | ASR-hallucination guard: flags a chapter if one content word repeats ≥8 times in its last 50 words (a classic Whisper infinite-loop symptom). |
| `run_safeguards(ch_transcripts)` | Runs all Step-1 quality checks: per-chapter transcript emptiness/shortness, total-transcript-length thresholds (<500 chars = critical, <1200 = warning), and the hallucination check above. Returns `(warnings, critical)`. |
| `build_safeguard_section(...)` / `append_safeguard_note(...)` | Render safeguard findings as a `## Ingest Safeguard Report` markdown block and persist it *inside* the tutorial file — so a `needs-review` flag stays auditable later instead of only ever existing in a terminal that's since closed. |
| `build_raw_md(...)` | Assembles the actual `tutorials/<slug>.md` file: YAML frontmatter (title/source/url/author/tags/extraction_status/frame_status) + the chapter-by-chapter timestamped transcript + a `Structured Notes` skeleton full of `[PENDING EXTRACTION]` markers for Step 3 to fill in. |
| `update_index_pending(...)` | Appends (or refuses to duplicate) a pending stub entry in `tutorials/INDEX.md`. |
| `update_readme_tutorial_count()` | Recomputes the real on-disk tutorial count and rewrites this README's `**N tutorials ingested**` line — runs automatically at the end of every ingest so the number never goes stale. |
| `fetch_article(url)` | Non-YouTube path: fetches a plain HTML page, strips scripts/styles/tags, and extracts a title + up to 8000 chars of body text for text-only ingestion. |
| `find_duplicate_by_video_id(video_id, exclude_name)` | Dedup guard — searches existing tutorial files for the same 11-char YouTube video ID (catches re-ingests where the uploader renamed the video, which a slug/URL-only check would miss). |
| `main()` | Orchestrates all of the above: fetch metadata → transcribe → segment → run safeguards → write the `.md` file → update `INDEX.md` and `README.md` → `git add` + `commit` + `push`. Flags: `--whisper-model {tiny,base,small,medium,large}`, `--skip-video` (permanently marks `frame_status: skipped`, text-only), `--force` (overwrite even if `extraction_status: complete`). |

**Run it:** `python ingest.py "<url>"` from this skill's own directory.

### `select_frames.py` — Step 2: content-aware frame capture

| Function | What it does |
|---|---|
| `parse_timestamp(raw)` | Accepts plain seconds (`"485"`) or `mm:ss` / `h:mm:ss` (`"8:05"`) — Claude picks these by hand after reading the timestamped transcript, not by blind percentage splits. |
| `read_frontmatter_field(content, key)` / `set_frontmatter_field(content, key, value)` | Regex-based YAML-frontmatter getter/setter used to read `frame_status`/`url` and write back `frame_count`/`frame_status`/`frame_selection`. |
| `main()` | Guards against re-capturing an already-`complete` or `skipped` file (unless `--force`), clears stale frames from a prior capture, downloads the low-quality video via `ingest.download_video_low()`, extracts the requested frames via `ingest.extract_frames()`, appends a `## Captured Frames` section, and updates frontmatter. Does **not** commit — that happens together with the Structured Notes in Step 3. |

**Run it:** `python select_frames.py <slug> <ts1> <ts2> ...` (4-8 timestamps is typical) after reading the transcript in `tutorials/<slug>.md`.

### Step 3 — Extraction (done by Claude Code, not a script)

Claude reads each captured frame with the Read tool (which supports images), identifies the panel/layer/setting shown, fills in every `[PENDING EXTRACTION]` marker in the Structured Notes (Core Technique, Summary, Key Steps, Layers/Tools/Settings, Difficulty, App & Version, Tags), cross-links related tutorials sharing 2+ tags, sets `extraction_status: complete`, and commits `tutorials/<slug>.md` + `INDEX.md` together.

### `validate.py` — post-ingest integrity checker

| Function | What it does |
|---|---|
| `get_tutorial_files()` | Lists every `tutorials/*.md` file except `INDEX.md`. |
| `parse_index_refs()` | Extracts every `**File:** tutorials/...` reference out of `INDEX.md`. |
| `get_notes_content(content)` | Pulls the `## Structured Notes` section body out of a tutorial file. |
| `is_youtube_source(content)` / `parse_duration_secs(content)` | Read `source:` frontmatter and the `**Duration:**` line. |
| `get_transcript_text(content)` | Reconstructs the raw transcript text from the `## Raw Data` section (stripping out any `## Ingest Safeguard Report` box first, since that has its own `---` divider that would otherwise be mistaken for the section boundary). |
| `check_tutorials()` | Runs checks 1–4 and 8–10: no `[PENDING EXTRACTION]` markers, no `extraction_status: pending`, no `app`/`version` PENDING placeholders, no empty `tags: []`, no `PLACEHOLDER` URLs, structured notes ≥200 chars for YouTube sources, and a transcript-length sanity check (≥3 chars/sec of runtime) for videos over 3 minutes. |
| `check_index()` | Runs checks 5–7: no duplicate `INDEX.md` entries, every disk file is indexed, no `INDEX.md` entry points at a missing file. |
| `check_script_drift()` | Cross-skill check (warn-only, never fails the run): compares this repo's shared helper functions (`slugify`, `download_audio`, `ytdlp_captions`, `segment_by_chapters`, `_detect_hallucination`, `append_safeguard_note`, `find_duplicate_by_video_id`) against the same functions in every sibling skill installed on the same machine, and warns if a copy has drifted — catching an intentional fix in one skill that never got ported to the others. |
| `main()` | Runs all checks, prints a pass/fail summary, exits 1 on any failure. |

**Run it:** `python validate.py` after a batch of ingests, or any time you want to sanity-check the library.

### Extending this pipeline

- **New source type** (e.g. a forum thread, a PDF): follow the `fetch_article()` pattern — fetch + extract title/text, feed it through `build_raw_md()`'s `is_yt=False` path, no frame capture needed.
- **New quality check**: add a check function inside `check_tutorials()`/`check_index()` in `validate.py`, following the existing `fail(msg)` pattern.
- **New safeguard**: add a check inside `run_safeguards()` in `ingest.py`, appending to `warnings`/`critical` — it'll automatically get persisted via `build_safeguard_section()`.
- **New reference file**: add `references/<topic>.md`, then add it to the table in `SKILL.md` → "Step 2 — Check Reference Files" so Claude knows when to reach for it.
- **Point it at a live Painter session**: see "Live connection" below — no pipeline code changes needed, it's a separate MCP layer.

---

## Every mode this skill supports

| Mode | Trigger phrases | What happens |
|---|---|---|
| **Setup** | "set up this skill", "new machine", "is this configured" | Walks the `SETUP.md` checklist (Python/ffmpeg/deno/yt-dlp/whisper/torch), fixes what's missing. |
| **1 — Consult** | "how do I...", "explain...", "what's the best way to..." | Searches `tutorials/INDEX.md` + the 7 `references/*.md` files, answers with Approach / Step-by-Step / Key Settings / Python (if relevant) / Gotchas / cited sources. |
| **2 — Write code** | "write me a plugin", "python for substance painter", "script to batch export" | Writes real `substance_painter` module Python — Python Console snippet or full plugin skeleton (`start_plugin()`/`close_plugin()`), never invented API calls. |
| **3 — Ingest** | "ingest this: [URL]", "learn from this", "add this tutorial" | Runs the full 3-step pipeline above, unprompted through all three steps. |
| **4 — Live connection (optional)** | "connect to my open Painter", "bake this project live", "export my textures right now" | Drives a real running Painter session via one of three third-party MCP servers (see below) — only if configured; otherwise walks you through setup first. |

**Auto-changelog check (Mode 0):** at the start of every consultation, if `references/version-tracker.md`'s `last_checked` date is over 7 days old, the skill checks Adobe's release notes for a newer Painter version and updates its own knowledge accordingly — so recommendations don't quietly go stale as Painter ships new features (e.g. OpenPBR becoming the default shading model in 12.1).

## Live connection (optional)

Substance Painter ships a built-in remote-scripting HTTP API (`--enable-remote-scripting`, `localhost:60041`) — no Painter-side plugin install needed, unlike some other DCC tools. Three independent, third-party MCP servers wrap it:

| Option | Tools | Cost | Notes |
|---|---|---|---|
| `elliezu/SubstancePainterMCP` | 79 | Free (MIT) | Recommended default — live-validated against Painter 12.1.1 |
| `diffdaff/substance-painter-mcp` | 10 | Free (MIT) | Minimal, single-file FastMCP server |
| "MCP Pro for Painter" | 179 | $15 one-time | Widest coverage, **not open source**, third-party commercial |

None are official Adobe products, and none are active by default. Full setup steps: `SKILL.md` → "Live Substance Painter Connection", `SETUP.md` → "Substance Painter MCP Connection".

## Repo structure

```
SKILL.md          Main instructions Claude reads (modes, reference map, MCP options, tag pool)
SETUP.md           Human + Claude setup guide
README.md           This file
CODE_OF_CONDUCT.md   Purpose/ethics statement — knowledge + consultation, not reproduction
ingest.py           Step 1 of the ingest pipeline
select_frames.py    Step 2 of the ingest pipeline
validate.py          Post-ingest integrity checker
references/          Hand-written Substance Painter knowledge base (7 files)
tutorials/            Ingested tutorial library + INDEX.md
```

## Sibling skills

Same ingest/validate/setup architecture as this skill's siblings — `blender-motion`, `houdini-wand`, `unreal-sidekick`, and `nuke-em-all` — each covering a different DCC/VFX toolset. `validate.py`'s drift check compares shared pipeline internals across all five and warns (never fails) if a copy has drifted.

## Status

Public personal project, no warranty, not affiliated with or endorsed by Adobe. **52 tutorials ingested** (count auto-updates on every `ingest.py` run — do not hand-edit this line).
