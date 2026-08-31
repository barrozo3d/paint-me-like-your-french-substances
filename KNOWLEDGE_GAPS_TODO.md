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

> 🔴 **D4b target 2 attempted 2026-08-31 — BLOCKED, and the reason is worth
> keeping.** The three items above cannot currently be filled from vendor docs.
>
> **1. The Python API documentation is not publicly reachable.** Adobe moved the
> Substance 3D docs to Experience League. `substance3d.adobe.com/documentation/ptpy/`
> and every path under it redirect to a **generic "General knowledge" page**.
>
> **2. ⚠️ The URL probe used throughout D4b gives FALSE POSITIVES on this site.**
> `curl -sL -o /dev/null -w "%{http_code}"` returned **200** for
> `ptpy/api-reference`, `ptpy/getting-started` and `ptpy/substance_painter.html`.
> All three are catch-all redirects to the same 1,262-char page with **zero**
> occurrences of `substance_painter`, `start_plugin` or `close_plugin`. On
> Foundry's docs a 404 was a real 404 and the probe was sound; **on Adobe's it is
> not.** Always confirm the *final* URL and measure the text for the topic —
> `-w "%{url_effective}"`.
>
> **3. Adobe says the docs ship inside the application.** The Experience League
> plugins page states the scripting documentation is *"available from the help
> menu of the application"*. It also describes plugins as *"wrote in Javascript
> and can be combined with the QML language"* — i.e. that page documents the
> **legacy JS/QML plugin API, not the Python API** the reference file is about.
>
> **4. Substance 3D Painter is not installed on this machine**, so the in-app
> documentation is not reachable here either.
>
> ✅ **Nothing was written from model knowledge**, deliberately. This gap is
> recorded as *"exactly the profile that made `copernicus.md` wrong"* — a
> reference file with no corroborating source — and filling it from memory would
> reproduce that failure rather than fix it.
>
> **How it could actually be closed:**
> * Open Substance 3D Painter on a machine that has it → **Help menu → scripting
>   documentation**, and ingest from there (the other device may have Painter).
> * Or capture the in-app doc pages and ingest them as pasted content via Mode 3.
> * Do **not** ingest a third-party mirror of the API docs — provenance for this
>   reference file is the entire point of the gap.

### 2b. 🔴 Texture transfer: scanned high-poly → retopologized low-poly — **found by a real question, 2026-08-31**

A user question F4 could not answer: *"how to correctly transpose a texture from a
3D-scanned asset to a retopologized asset (using Substance for example)?"*

Retrieval surfaced **39** baking entries, and the top hits are all about baking
**mesh maps** — normal, AO, curvature, skew. That is a **different operation**.
The question is about carrying an existing **albedo/colour texture** from a dense
photogrammetry scan onto a clean retopo mesh: cage/max-distance handling for a
noisy scan, `Bake Mesh Maps > Diffuse/Base Color from mesh`, UV correspondence
when the two meshes disagree, and what to do where the scan has holes.

**Adjacent material exists; the operation does not.** Recorded rather than
answered from model memory — this skill's Python-API gap is already the
`copernicus.md` profile and one uncorroborated area is enough.

- [ ] **Texture/colour transfer from a scanned mesh to a retopo mesh** — cage and
      max-distance for noisy scans, baking Base Color from mesh, UV mismatch,
      filling scan holes

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
