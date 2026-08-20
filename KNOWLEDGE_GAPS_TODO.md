# Knowledge Gap To-Do List

Generated 2026-08-20 from a library-wide gap analysis (97 ingested tutorials
checked against `SKILL.md` scope + all `references/*.md`). Every gap below was
**measured** — each line records how many tutorial files actually mention the
topic — not guessed. Ingest with `python ingest.py "[URL]"` from this directory,
then run the mandatory extraction pass (see `SKILL.md` Mode 3).

> **How the counts were taken.** Case-insensitive regex over all 97 tutorial
> files (not `INDEX.md`, which counts tags rather than content), then the thin
> results hand-checked by listing the matching files. That second step matters:
> a first pass counted **5** files for "Painter Python", but every one of them
> matched only the generic word *plugin* — the real count for the
> `substance_painter` module is **0**. *Suspect the instrument before the data.*

**This library is in good shape.** Core texturing is covered deeply (generators
67, layer stacks 68, alpha/stencil 69, displacement/height 72, baking 44, anchor
points 44, smart materials 37). The gaps below are narrow, and they share one
pattern: **they are capabilities `SKILL.md` advertises that no tutorial teaches.**

## Pending

### 1. 🔴 The `substance_painter` Python API — **ZERO tutorials**

`SKILL.md` advertises "the Python scripting API" and "writing Painter Python
plugins" as a headline capability, and `references/substance-painter-python-scripting.md`
exists. **No ingested tutorial mentions the `substance_painter` module at all**
(0 of 97). The reference file is therefore uncorroborated by any source in this
skill — exactly the profile that made `copernicus.md` wrong in `houdini-wand`.

- [ ] **Painter Python plugin basics** — plugin folder layout, `start_plugin` /
      `close_plugin`, the Python console, reloading during development
      Source: Adobe official — Substance 3D Painter Python API documentation
- [ ] **Automating exports with Python** — `substance_painter.export`, export
      presets driven from script, batch export across texture sets
- [ ] **UI + events** — `substance_painter.ui` menus/docks and the event
      callbacks (`ExportTexturesEnded`, project open/close)

### 2. Channel packing — **1 tutorial**

`SKILL.md` advertises "channel packing/export presets". Exactly one file covers
it (`optimizing-textures---how-to-pack-masks-like-a-pro.md`), and "export
preset|export template" matches only 5.

- [ ] **Channel packing for engines in depth** — building a packed ORM/RMA
      export preset from scratch, per-channel source mapping, sRGB vs linear
      per slot, and verifying the result in-engine

### 3. Unity and Godot export — **2 and 0 tutorials**

`SKILL.md` advertises export pipelines "for game engines (Unreal/Unity/Godot)".
Measured: Unreal **31**, Unity **2** (both incidental mentions inside broader
videos, not dedicated workflows), Godot **0**.

- [ ] **Painter → Unity** — Unity's metallic/specular setups, the Unity export
      preset, HDRP vs URP channel expectations
- [ ] **Painter → Godot** — Godot 4 material channels and the ORM convention

### 4. Substance Designer interop — **5 tutorials** (adjacent, low priority)

`substance designer|sbsar` matches 5. Designer is outside this skill's stated
scope, but authoring a custom `.sbsar` filter/generator *for use in Painter* sits
on the boundary and is thinly covered. Ingest only if a genuinely
Painter-focused source appears.

## Notes on what is NOT a gap

Measured and healthy, recorded so nobody "fills" a gap that does not exist:

| Topic | Files (of 97) |
|---|---|
| Displacement / height | 72 |
| Alpha / stencil | 69 |
| Layer stack / folders | 68 |
| Stylized / hand-painted | 68 |
| Generators | 67 |
| Curvature / thickness / AO | 64 |
| Filters | 60 |
| Iray / rendering | 58 |
| Hair / fur | 56 |
| Opacity / emissive | 55 |
| Texture sets | 53 |
| Baking / mesh maps | 44 |
| Anchor points | 44 |
| Smart materials | 37 |
| Unreal export | 31 |
| Skin | 25 |
| Triplanar | 24 |
| Subsurface / SSS | 19 |
| UDIM | 17 |
| Smart masks | 15 |
| Colour ID / ID maps | 11 |

## Completed

(none yet — this list was created 2026-08-20 and nothing on it has been ingested)
