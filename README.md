# Paint Me Like Your French Substances

A Claude Code skill: an expert consultant for **Adobe Substance 3D Painter** that also builds its own knowledge base by ingesting tutorials, and can optionally drive a real, running Painter session over MCP.

The name is a nod to Substance Painter's French origins (Allegorithmic, the studio Adobe acquired to make it) and to the [Rembrandts' theme song](https://en.wikipedia.org/wiki/I%27ll_Be_There_for_You_(The_Rembrandts_song)) — no relation to Adobe, and not an official Adobe product.

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

## How it works

**Consulting.** Every question is answered against `tutorials/INDEX.md` (the ingested-tutorial library) plus seven `references/*.md` files covering layers/masks, baking, shaders/channels, Python scripting, export, PBR/texturing theory, and version tracking. See `SKILL.md` for the full reference-file map and answer format.

**Growing the library.** Say "ingest this: [URL]" and a three-step pipeline runs:
1. `ingest.py` — pulls a YouTube transcript (Whisper, with per-sentence timestamps) or article text, no video download, no API calls.
2. `select_frames.py` — Claude reads the timestamped transcript, picks 4-8 moments that actually show a technique, and this script captures just those frames.
3. Claude reads the captured frames and the transcript, writes structured notes (technique, steps, settings, tags), cross-links related tutorials, and commits everything to this repo.

`validate.py` is a post-ingest integrity checker (no `[PENDING]` leftovers, no broken INDEX cross-references, transcripts long enough to be real) — run `python validate.py` after a batch of ingests.

**Live connection (optional).** Substance Painter ships a built-in remote-scripting HTTP API (`--enable-remote-scripting`). Three third-party MCP servers wrap it — a free 79-tool option, a free 10-tool minimal option, and a paid 179-tool option — documented in `SKILL.md` → "Live Substance Painter Connection" and `SETUP.md` → "Substance Painter MCP Connection". None are official Adobe products, and none are active by default.

## Repo structure

```
SKILL.md          Main instructions Claude reads (modes, reference map, MCP options, tag pool)
SETUP.md           Human + Claude setup guide
ingest.py           Step 1 of the ingest pipeline
select_frames.py    Step 2 of the ingest pipeline
validate.py          Post-ingest integrity checker
references/          Hand-written Substance Painter knowledge base (7 files)
tutorials/            Ingested tutorial library + INDEX.md
```

## Sibling skills

Same ingest/validate/setup architecture as this skill's siblings — `blender-motion`, `houdini-wand`, `unreal-sidekick`, and `nuke-em-all` — each covering a different DCC/VFX toolset. `validate.py`'s drift check compares shared pipeline internals across all five and warns (never fails) if a copy has drifted.

## Status

Public personal project, no warranty, not affiliated with or endorsed by Adobe. The knowledge base starts empty; ingest tutorials to grow it.
