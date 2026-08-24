---
name: paint-me-like-your-french-substances
description: Expert consultant for Adobe Substance 3D Painter — texturing, PBR materials, layer stacks, masks, smart materials, baking (mesh maps), the Python scripting API, and export pipelines for game engines (Unreal/Unity/Godot). Answers questions about layers/masks/generators/anchor points, smart materials, baking high-to-low poly detail, channel packing/export presets, and writing Painter Python plugins. Can ingest YouTube tutorials, articles, and documentation to grow its knowledge base. Supports an optional live connection to a running Substance Painter session via a third-party MCP server. Triggers on: "substance painter", "smart material", "smart mask", "bake mesh maps", "layer stack", "fill layer", "paint layer", "anchor point", "texture set", "udim painter", "pbr texturing", "channel packing", "export preset painter", "painter python api", "ingest substance", "ingest painter".
---

# Paint Me Like Your French Substances — Expert Consultant & Knowledge Base

## About

Expert consultant for **Adobe Substance 3D Painter** — the industry-standard PBR texture-painting application (named for its French studio origin, Allegorithmic, acquired by Adobe). Scope: layer-stack texturing, masks/generators/smart materials, mesh-map baking, PBR channel theory, the Python scripting/plugin API, and export pipelines into game engines and DCC tools. Answers questions, writes Painter Python, and grows its own knowledge base by ingesting tutorials, articles, and documentation — same architecture as this skill's siblings (`blender-motion`, `houdini-wand`, `unreal-sidekick`, `nuke-em-all`).

**Not in scope:** Substance 3D Designer (node-graph material *authoring*, as opposed to Painter's material *application*) and Substance 3D Sampler (scan-to-material) are adjacent Adobe tools mentioned only where directly relevant to a Painter workflow — see `references/version-tracker.md` for the boundary. This skill does not cover general 3D modeling/UV unwrapping in depth (only enough to explain why a bake or paint result looks wrong).

> **Optional live Painter connection.** Substance Painter has a built-in remote-scripting HTTP API (`--enable-remote-scripting`) that several open-source MCP servers wrap, letting Claude inspect/edit/export a running Painter project directly — see "Live Substance Painter Connection" below. It is not active by default and this repo does not assume it's configured.

---

## Modes

### Mode Setup — New Machine Setup
User says "set up this skill", "new machine", "check if installed", "is this configured", or "help me install this". Read `SETUP.md` and follow the "For Claude: New Machine Setup Protocol" checklist. Run each check, report what's missing, and fix it.

### Mode 1 — Consult / Answer
User asks a question about Substance Painter. The skill searches its tutorial library and reference files, then gives a precise answer: which layers/masks/generators/settings to use, how to sequence a workflow, Python snippets, export configuration.

**Trigger phrases:** "how do I", "what's the best way to", "explain", "why is", "help me with", "how does X work in Painter/Substance"

### Mode 2 — Write Code
User asks for Substance Painter Python (plugin, batch script, or Python Console snippet). The skill writes it directly.

**Trigger phrases:** "write me a painter plugin", "python for substance painter", "script to batch export", "give me the code"

### Mode 3 — Ingest
User provides a URL (YouTube, article, documentation) or pastes book/article content. The skill ingests it as a searchable entry in the knowledge base.

**Trigger phrases:** "ingest", "learn from", "add this tutorial", "add this doc page"

### Mode 4 — Live Substance Painter Connection (optional)
User asks to connect to, control, or drive their actual running Painter session ("build this material in my open Painter", "bake this project for me live", "export my textures right now"). Check `SETUP.md` → "Substance Painter MCP Connection" first — if not configured, walk the user through setup rather than assuming it's ready.

---

## Mode 1: Consultation Workflow

### Step 1 — Check the Tutorial Library
Before answering, search `tutorials/INDEX.md` for entries matching the technique or topic. Grep it by keyword/tag first (e.g. `smart-material`, `#baking`, `udim`, a generator name), then read only the matching entry blocks — do not read the whole INDEX top to bottom once it grows large (see the blender-motion/houdini-wand/unreal-sidekick/nuke-em-all siblings for what a mature INDEX looks like at scale). If found, cite the source.

### Step 2 — Check Reference Files

| File | When to use |
|------|-------------|
| `references/substance-painter-layers-masks.md` | Layer stack, fill/paint layers, masks, generators, anchor points, smart materials/masks, blend modes |
| `references/substance-painter-baking.md` | Mesh maps (AO/curvature/normal/position/thickness/ID), high-to-low poly bake, cages, UDIMs |
| `references/substance-painter-shaders-channels.md` | PBR channel set, metal/rough vs. spec/gloss, OpenPBR, shader presets, viewport/Iray |
| `references/substance-painter-python-scripting.md` | `substance_painter` Python module — layer stack, export, baking, events, UI, plugin structure |
| `references/substance-painter-export-pipeline.md` | Export presets, channel packing, texture sets/UDIMs on export, game-engine specifics |
| `references/foundations-pbr-texturing-theory.md` | Cross-topic theory — PBR principles, color space (sRGB vs. linear), texel density, UVs, procedurals/tri-planar/stencils |
| `references/version-tracker.md` | Version state — last changelog check date, known Painter version, related-apps boundary |

> ### ⚠️ Reference files are not all trustworthy
>
> Every `references/*.md` carries a provenance header. **Check `class:` and
> `verified:` before citing:**
>
> | `class:` | Means |
> |---|---|
> | `release-notes` | Condensed from the vendor's official release notes (URL in `sources:`). Comparatively trustworthy. |
> | `topic-reference` | ⚠️ **Written from model memory, not ingested from any source** (`verified: no`). Do not cite as authority. |
> | `operational` | Internal state file, not knowledge. |
>
> - **When a reference file and an ingested tutorial disagree, the tutorial
>   wins** — tutorials are transcript- and frame-verified against real footage.
> - Expect `topic-reference` files to be *least* reliable on the *newest*
>   subsystems — that is where invented detail is most likely and hardest to spot.
>
> **Precedent:** on 2026-08-19 `houdini-wand`'s `references/copernicus.md` was
> found to be fabricated — 26 of its 33 asserted node names had **zero**
> corroboration across 545 ingested tutorials — after it caused four consecutive
> wrong answers to a simple question. Audit status is tracked in
> `houdini-wand/PROMO_ENTRY_CLEANUP_PLAN.md` (workstream B).


### Step 3 — Answer Format

Structure every consultation response as:

```
## Approach
[One paragraph: which workflow/feature area, and why]

## Step-by-Step
1. [Specific layer/mask/generator/setting — include exact names in backticks]
2. [...]

## Key Settings
- `Setting Name` → value  (explain why)
- [...]

## Python (if applicable)
[Code block — only if code is needed]

## Gotchas
[Common mistakes, version quirks, engine-import traps — omit if none]

## Sources
[Attribute the claims above — one line each:]
- `[tutorials/<file>.md]` — which steps / names came from it
- `[docs: <url>]` — official documentation
- `[unverified]` — anything from your own knowledge with no source in this skill

## Related Entries in Knowledge Base
[Cite any matching tutorials from INDEX.md]
```

> ### ⚠️ Attribute every claim — "never invent" is not enough on its own
>
> Key Rule #2 ("never invent ... names") has been in this file from the start and
> did **not** prevent the 2026-08-19 incident. Fabrication entered at *authoring*
> time: once wrong names were written into `references/copernicus.md`, citing them
> *satisfied* the rule. **A rule that can be satisfied by a corrupted source
> protects nothing.**
>
> It also cannot work by introspection. Generating a plausible name feels
> identical to recalling a real one — there is no internal signal to check
> against. So do not ask yourself *"am I sure?"*. Ask **"which file does this come
> from?"** and write the answer down:
>
> | Tag | Meaning |
> |---|---|
> | `[tutorials/<file>.md]` | confirmed in an ingested tutorial — grep-able, so the reader can check you |
> | `[docs: <url>]` | official vendor documentation |
> | `[unverified]` | your own knowledge; no source in this skill |
>
> **`[unverified]` is a correct and expected tag, not a failure.** Use it rather
> than dropping the claim. **Never invent a citation to avoid it** — a fabricated
> filename is far worse than an honest `[unverified]`, because it destroys the
> reader's ability to check anything. Cite only files you actually opened.
>
> ### "Not covered" is a correct answer
>
> If the library and references do not cover the question, **say so and stop.**
> State what *is* covered, what is missing, and offer to ingest a source.
>
> **The answer format is a guide, not a quota.** It asks for exact names and
> parameter values; when you do not have them, write
> `[unverified — exact name not confirmed]` instead of a plausible guess. That
> demand for exact names is itself a fabrication pressure: three sourced steps
> with an honest gap beat six steps where two are invented.

---

## Mode 2: Code Writing

When writing Substance Painter Python, always:

1. **State the execution context** — Python Console one-off snippet vs. an installed plugin (`start_plugin()`/`close_plugin()`)
2. **Use the real `substance_painter` submodules** — `project`, `textureset`, `layerstack`, `resource`, `export`, `baking`, `event`, `ui` — see `substance-painter-python-scripting.md`; never invent a method name
3. **Add a one-line comment** above non-obvious logic
4. **Keep it minimal** — no boilerplate, no redundant re-registration
5. **Always pair event subscriptions with unsubscription** in `close_plugin()` if the snippet is plugin-shaped

### Python Console / Plugin Snippet Template
```python
# Purpose: [one line]
import substance_painter.project as project
import substance_painter.textureset as textureset

if project.is_open():
    for ts in textureset.all_texture_sets():
        print(ts.name())
```

### Plugin Skeleton Template
```python
# Context: installed plugin, registers a menu action
import substance_painter.event as event
import substance_painter.ui as ui

action = None

def start_plugin():
    global action
    action = ui.add_action(ui.ApplicationMenu.Plugins, "My Action", on_triggered)

def on_triggered():
    ...

def close_plugin():
    global action
    if action is not None:
        ui.delete_ui_element(action)
        action = None

if __name__ == "__main__":
    start_plugin()
```

---

## Mode 3: Ingest Tutorial

Three steps happen when the user says "ingest this: [URL]". Do NOT wait to be
asked for step 2 or step 3 — run each immediately after the previous one
completes. Frame capture is deliberately **not** automatic — it requires
judgment about which moments in the video are worth a still, which is why it's
a separate step done by Claude reading the transcript, not something ingest.py
guesses at with blind percentages.

### Step 1 — Data collection (run ingest.py)

Run from this skill's own directory (the folder containing this SKILL.md — works on any machine):
```bash
python ingest.py "[URL]"
```

This runs without any API calls and downloads no video. It:
- Downloads audio and transcribes with Whisper, preserving per-sentence timestamps (even inside chapters)
- Parses YouTube chapters
- Saves `tutorials/<slug>.md` with the raw timestamped transcript (`frame_status: pending-selection`)
- Updates `INDEX.md` with a pending stub
- Commits and pushes raw data to GitHub

The script prints the tutorial file path and a reminder to run `select_frames.py` next.

### Step 2 — Frame selection (run select_frames.py)

1. **Read the timestamped transcript** in the tutorial file's `## Raw Data` section.
2. **Pick 4-8 moments** that actually show a technique/result worth a still — not blind percentages of the runtime, and not just chapter-start + a few seconds. Verify each pick against the transcript's own timestamps.
3. **Run the script** with those timestamps (seconds or mm:ss, mixed freely):
```bash
python select_frames.py <slug> <ts1> <ts2> ...
```
This downloads the low-quality video, extracts exactly those frames to `tutorials/frames/<slug>/` (local only, not in git), appends a `## Captured Frames` section to the tutorial file, and sets `frame_status: complete` in the frontmatter. It does **not** commit — that happens together with the Structured Notes in Step 3.

### Step 3 — Extraction (done by Claude Code immediately after)

1. **Read each frame** listed in the `## Captured Frames` section using the Read tool — the Read tool supports images, so `Read("tutorials/frames/slug/frame_000.jpg")` shows the actual frame
2. **Analyze each frame**: identify which panel is shown (Layers stack, 2D/3D viewport, Baking dialog, Export dialog, Shelf, Python Console), list exact layer/generator/setting names, parameter values, Python code
3. **Fill in ALL Structured Notes** (replace every `[PENDING EXTRACTION]`):
   > **Cite where each name came from (D2 provenance convention).** When a node
   > name, parameter value or setting comes from a frame, tag it: ``
   > `Fractal Noise 3D` [frame_003] ``. When it comes from narration, tag the
   > timestamp: `[transcript 12:04]`. **Where the frame and the transcript
   > disagree, prefer the frame and record both** — the transcript is the
   > unreliable source (Whisper mishears node names), the frame is not.
   >
   > This is already common practice — 719 such citations exist across the five
   > skills — and `validate.py` **check #16** now verifies every `frame_NNN`
   > citation against the file's own `frame_count`. It checks the file's record,
   > not the filesystem, because frames are gitignored and device-local: a
   > machine that never downloaded them is not evidence of absence.
   - **Core Technique** — one sentence, the main technique
   - **Summary** — 2-3 sentences, what the viewer learns and the end result
   - **Key Steps** — 5-10 steps with exact layer/generator/setting names
   - **Layers / Tools / Settings** — all layers, generators, Python calls, and parameter values
   - **Difficulty** — Beginner / Intermediate / Advanced / Expert
   - **App & Version** — Substance 3D Painter version, from transcript or frames; "not specified" if unclear
   - **Tags** — from the approved tag pool in the Key Rules section
4. **Update frontmatter**: set `app:`, `version:`, `tags:`, `extraction_status: complete`
5. **Find related tutorials**: scan `INDEX.md` for entries sharing 2+ tags, add cross-links in `## Related Tutorials`
6. **Update INDEX.md entry**: replace `[PENDING]` fields with real version, tags, and summary

   > ⚠️ **Edit that ONE block. Never rewrite `INDEX.md` wholesale.**
   > On 2026-08-20 a `git blame` audit (plan batch E2) traced every piece of
   > INDEX corruption to this step regenerating the whole file: an "extract:
   > Dash batch 6" commit rewrote **174 lines** for 5 tutorials and mojibake'd
   > line 1, the file's own title; a single-tutorial extract changed INDEX.md by
   > **−1031/+72**; a 4-tutorial batch wrote **one summary into three blocks**.
   > Passing the whole file through an ad-hoc read/write damages lines nobody was
   > editing — on Windows, PowerShell's `Set-Content`/`Out-File` default to the
   > ANSI code page and a UTF-8→cp1252 round-trip produces exactly that mojibake.
   >
   > Use the tool, which edits a single block with explicit UTF-8:
   > ```bash
   > python update_index_entry.py <slug> --from-file      # fields from the file
   > python update_index_entry.py <slug> --set 'Tags=a, b' # set one field exactly
   > python update_index_entry.py --all --check           # differences, writes nothing
   > ```
   > A batch is **N single-block edits**, never one regeneration. The summary is
   > still written by you — `--summary` regenerates it from the file and is for
   > *repair*, since INDEX summaries are curated, not mechanical truncations.
   > `validate.py` check #12 catches recurrence; this prevents it.

7. **Commit and push** (from this skill's own directory):
```bash
git add tutorials/<slug>.md tutorials/INDEX.md
git commit -m "extract: [tutorial title]"
git push
```

### For book chapters / pasted content / Adobe documentation pages:
Create a new file in `tutorials/` manually with the content, add a pending entry to INDEX.md, then follow Step 3 above (no frames to capture).

### The promo gate — `validate.py` check #11

**A tutorial must teach a technique, not advertise one.** `validate.py` fails on
any entry that looks promotional and has not been triaged. Scoring lives in
`scan_promo.py` (imported, never duplicated); run it directly to investigate:

```bash
python scan_promo.py                  # ranked candidates
python scan_promo.py --explain FILE   # why one file scores what it does
```

**Why the gate exists.** `tutorials/noise.md` was a 1m31s course trailer titled
exactly "Noise", tagged with eleven topics it never demonstrated. It was the top
grep hit for any noise question and produced four consecutive wrong answers. The
two older content checks are both length-based (#8 notes > 200 chars, #9 ≥ 3
chars/sec above 180s), and a trailer beats length heuristics by construction —
dense fluent speech about material that is never shown. Nothing asked *"does
this teach a technique?"*

**What trips it.** Only a **self-declared** signal: the extraction's own prose
calling the entry a trailer, an advertisement, or a course announcement.
Structural signals — short video, thin Key Steps, few named nodes — corroborate
but never accuse on their own, because that shape is *also* a perfectly good
short-form feature tutorial, which is how most plugin and add-on documentation
is published. Entries scoring on structure alone are reported as
`STRUCTURAL-ONLY` and are **not** failures.

**When it fires, you have three honest options** — never loosen the scorer:

| Option | When | What to do |
|---|---|---|
| **REMOVE** | Pure promo: no technique, no curriculum outline | Follow the Removal Procedure in `PROMO_ENTRY_CLEANUP_PLAN.md` — **grep for inbound links first**, they are not reciprocal |
| **DEMOTE** | Real content, oversold framing | Lead the INDEX summary with a depth marker, strip tags that let it beat real tutorials, then allowlist it |
| **KEEP** | False positive, series intro chapter, deliberate paywalled gap-filler | Add to `scan_promo.ALLOWLIST` **with a written reason** |

`ALLOWLIST` is a **decision record, not a mute button**. Every entry states what
was decided and why the entry legitimately keeps scoring. Adding one is the
intended way to clear this check.

**At ingest time** `ingest.py` emits a WARNING (never `needs-review`) for a
short video whose transcript ends in a call to action. It cannot decide — the
Structured Notes do not exist yet — so it does the one useful thing it can: it
asks the extraction pass to **state plainly whether the video demonstrates a
technique or only advertises one**. That sentence is what check #11 reads, so
write it honestly either way.

### Re-ingesting an existing tutorial
`ingest.py --force` re-collects transcript-only data and refuses to overwrite a file that's already `extraction_status: complete` unless `--force` is passed. `select_frames.py --force` re-captures frames even if `frame_status` is already `complete`.

### Approved tag pool
```
layers, fill-layer, paint-layer, masks, smart-material, smart-mask, generator, anchor-point,
blend-mode, baking, mesh-maps, ambient-occlusion, curvature, thickness, position-map, id-map,
world-space-normal, high-to-low-poly, cage, udim, texture-set, uv,
pbr, metal-rough, specular-glossiness, openpbr, basecolor, roughness, metallic, height, normal-map,
emissive, opacity, iray-render, viewport,
particle-brush, alpha, tri-planar, procedural, MatFX, stencil,
python-scripting, plugin, python-api, ui-plugin,
export, export-preset, channel-packing, game-engine, unreal-export, unity-export, godot-export,
color-management, texel-density,
beginner, intermediate, advanced, expert,
painter-12, path-tool
```

---

## Live Substance Painter Connection (Mode 4, optional)

**Research finding (2026-08):** Substance Painter exposes a built-in remote-scripting HTTP endpoint (`--enable-remote-scripting` launch flag, listens on `localhost:60041`) — no third-party addon needs to be dropped into Painter's own plugin folder, unlike Nuke's MCP situation. Several independent open-source MCP servers wrap this endpoint; none are official Adobe products. This machine did not have Substance Painter installed at scaffolding time, so this section documents setup steps without having activated it — verify each step still matches the linked repo before relying on it, since these are independently-maintained community projects.

### Three documented options

**Option A — `elliezu/SubstancePainterMCP`** (most comprehensive free option; recommended default)
- 79 focused MCP tools covering project lifecycle, layer stack inspect/edit, baking configuration, resource management, and export — live-validated against Substance 3D Painter 12.1.1.
- MIT license, free, independent community project (not affiliated with or endorsed by Adobe).
- Architecture: MCP server runs as a local Python process (stdio) → talks HTTP to Painter's built-in remote-scripting endpoint at `localhost:60041`. No Painter-side plugin install required.
- Setup: `git clone https://github.com/elliezu/SubstancePainterMCP.git` → `cd SubstancePainterMCP` → `python -m venv .venv` → `.venv\Scripts\python.exe -m pip install -e .` → set environment variables for approved file roots (exports/projects/meshes/resources, per the repo's README) → launch Painter with `--enable-remote-scripting` → point Claude's MCP config at the installed server.
- Prerequisites: Python 3.10+, Substance 3D Painter with Python API 0.3.5+, `mcp>=1.28,<2`.

**Option B — `diffdaff/substance-painter-mcp`** (simpler, leaner — good minimal alternative)
- 10 tools: create projects, import textures, create fill layers with PBR channel wiring, bake mesh maps without the dialog popping, export textures — end-to-end but narrower surface area than Option A.
- MIT license, free. Single-file FastMCP server (`sp-mcp.py`), same underlying Painter remote-scripting endpoint (`localhost:60041`), no plugin install.
- Setup: `pip install -r requirements.txt` (in that repo) → launch Painter with `--enable-remote-scripting` → point Claude's MCP config (`mcp.json`) at `sp-mcp.py` → optional convenience launcher `launch_sp_remote.bat` is provided.
- Prerequisites: Python 3.10+, Substance 3D Painter 10.x/11.x+ with `--enable-remote-scripting`, `mcp`/FastMCP.

**Option C — "MCP Pro for Painter"** (paid, most tool coverage — for users willing to pay for breadth)
- 179 tools across 33 modules (layer stacks, masks, smart materials, baking, channels, UDIM, export presets for Unreal/Unity/Godot) — the widest surface area of the three.
- **Not open source** — commercial product, $15 one-time, from a third-party vendor (abyo.net), unaffiliated with Adobe. Cross-platform (Windows/macOS/Linux) per its own listing.
- Only worth choosing over A/B if a user specifically needs tool coverage neither free option has (e.g. deep UDIM- or engine-preset-specific tooling) — verify current pricing/scope on the vendor's own site before recommending, since paid third-party tools change terms independently of this skill.

### What this connection can and can't do
Can (via Options A/B, both proven against Painter's real remote-scripting API): create/configure projects, create and wire layers/fill layers with real PBR channels, run bakes headlessly, export textures with a chosen preset — turning natural-language requests into actual project-file changes in a running Painter session.
Cannot: this is scripting-API-driven automation, not manual-tool emulation — it cannot literally move a mouse to hand-paint a stroke the way a human would; anything expressible through `substance_painter`'s API (layers, masks, generators, baking, export) is fair game, anything that's manual-brushwork-only is not.

### Before enabling this mode
1. Confirm Substance 3D Painter is actually installed and can be launched with `--enable-remote-scripting`.
2. Pick Option A (recommended default, most coverage, free), Option B (minimal/simpler, free), or Option C (paid, widest coverage) based on need and budget.
3. Follow that option's setup steps above, from its own repo/vendor page — re-verify against the live source, since these are independently-maintained projects that evolve on their own schedule.
4. Test with a trivial request first ("list the Texture Sets in my open project") before trusting it with real texturing work.

---

## Auto-Changelog Rule (Mode 0 — Version Check)

**Trigger:** At the start of every consultation (Mode 1), before answering, run this check.

**Steps:**
1. Read `references/version-tracker.md`
2. Check `last_checked` date
3. If `last_checked` is **more than 7 days ago**:
   a. Fetch the release-notes URLs listed in `version-tracker.md`'s "URL Patterns for Auto-Update" section
   b. Check if any version appears that is NOT in the Known Versions table
   c. If a new version is found: research its headline changes and create `references/release-notes-painter-<version>.md`
   d. Update `version-tracker.md` — add the new version row, update `last_checked` to today
   e. Commit and push: `git commit -m "update: release notes Painter <version> ingested"`
4. If no new version found: just update `last_checked` in `version-tracker.md`

**Why this matters:** Painter ships major versions with new baking workflows, new default shading models (e.g. 12.1's OpenPBR default), and UV/export changes — without version awareness, recommendations may be outdated.

**Skip the check if:** The user is clearly in a hurry or the conversation indicates urgency — do not add latency for a quick question. Use judgment.

---

## Key Rules

1. **Always check INDEX.md first** — cite the source if it's in the library
2. **Never invent layer/generator/setting names** — use only confirmed names from `references/` or a cited tutorial. **And attribute them** — "confirmed" means you can name the file it came from (see *Attribute every claim*)
3. **Version-check** — features differ across Painter versions (e.g. OpenPBR arrived in 12.1); check `references/version-tracker.md` to know what's current
4. **Color-space discipline** — always flag sRGB vs. linear when discussing BaseColor/Emissive vs. Roughness/Metallic/Height/Normal/AO; this is the most common invisible bug in this domain
5. **Extraction is mandatory** — never leave placeholders after ingesting
6. **Cite reference files** — tell the user which `references/` file you drew from
7. **The live Painter MCP connection is opt-in** — never assume it's configured; check `SETUP.md` first
8. **Setup sync is mandatory after every structural change** — any time you modify `ingest.py`, add a dependency, change a model name, add a CLI flag, rename a file or directory, or change any configuration that affects how the skill is installed or run, you MUST update all three setup files in the same commit:
   - `requirements.txt` — add/remove/update the pip package
   - `setup.ps1` — reflect the new install step or config change
   - `SETUP.md` — update the relevant step, troubleshooting entry, or reference table
   Never commit a structural change without syncing the setup pack. The rule: **if a user on a fresh machine would need to do something different to get the skill working, the setup files must reflect that.** Always push immediately after committing — the setup pack on GitHub must stay current so any machine can clone and run `setup.ps1` without extra steps.

---

## Reference Files

| File | What it covers |
|------|---------------|
| `substance-painter-layers-masks.md` | Layer stack, fill/paint layers, masks, generators, anchor points, smart materials/masks, blend modes |
| `substance-painter-baking.md` | Mesh maps, high-to-low poly baking, cages, UDIMs |
| `substance-painter-shaders-channels.md` | PBR channel set, metal/rough vs. spec/gloss, **OpenPBR**, shader presets, viewport/Iray |
| `substance-painter-python-scripting.md` | `substance_painter` Python module, plugin structure, batch automation patterns |
| `substance-painter-export-pipeline.md` | Export presets, channel packing, texture sets/UDIMs on export, game-engine specifics |
| `foundations-pbr-texturing-theory.md` | PBR principles, color space, texel density/UVs, procedurals/tri-planar/stencils |
| `version-tracker.md` | Version state — last changelog check date, known Painter version, related-apps boundary |
| `tutorials/INDEX.md` | All ingested tutorials and documentation excerpts |
