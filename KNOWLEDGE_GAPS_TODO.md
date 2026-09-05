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

### 1. ✅ The `substance_painter` Python API — **CLOSED 2026-09-04** (was ZERO)

Five pages ingested and extracted, taking `substance_painter` from **0 of 97** to
**5 of 102**. `references/substance-painter-python-scripting.md` now has the
corroborating source it never had — the profile that made `copernicus.md` wrong.

- [x] **Painter Python plugin basics** — plugin folder layout, `start_plugin` /
      `close_plugin`, the Python console, reloading during development
      ✅ `substance-painter-plugins-module.md` — `substance_painter_plugins.path`
      and `SUBSTANCE_PAINTER_PLUGINS_PATH`; the three expected subdirectories
      (`plugins/` optional, `startup/` always loaded, `modules/` shared, and
      `plugins/` takes precedence); `update_sys_path()` which must be called
      explicitly after changing `path`; `start_plugin` / `close_plugin` /
      `is_plugin_started` / `close_all_plugins`; and `reload_plugin()` including
      the plugin's own `reload_plugin` hook, which is the only way a package
      reloads its sub-modules.
      ✅ `versioning-plugin-example.md` — Adobe's complete `versioning_plugin.py`
      skeleton, the best single reference for the *shape* of a real plugin.
- [x] **Automating exports with Python** — `substance_painter.export`, export
      presets driven from script, batch export across texture sets
      ✅ `python-api-export-module.md` — the full `json_config` schema:
      `exportPath`, `defaultExportPreset`, `exportPresets` with `fileName`
      wildcards, `channels` (`destChannel`/`srcChannel`/`srcMapType`/`srcMapName`
      across `documentMap`, `meshMap`, `virtualMap`, `defaultMap`), `exportList`
      by `rootPath` with `outputMaps`/`uvTiles` filters, and the **ordered**
      `exportParameters` override rules. Plus `sizeLog2` as an exponent, the five
      padding algorithms and which need `dilationDistance`,
      `list_project_textures()` as a dry run, `PredefinedExportPreset` vs
      `ResourceExportPreset`, `export_mesh()` with `MeshExportOption`, and the
      rule that the returned status is never `Error` because failures raise.
- [x] **UI + events** — `substance_painter.ui` menus/docks and the event
      callbacks (`ExportTexturesEnded`, project open/close)
      ✅ `python-api-ui-module.md` — `get_main_window`, `add_dock_widget`,
      `add_toolbar`, `add_plugins_toolbar_widget`, `add_menu`, `add_action`,
      `delete_ui_element`; `UIMode` flags and layout save/restore; the
      `windowIcon` quick-button and the unique `objectName` that makes geometry
      persist; `ServiceNotFoundError` before the UI service starts.
      ✅ `python-api-event-module.md` — `DISPATCHER`, **weak `connect()` vs strong
      `connect_strong()`**, `ExportTexturesAboutToStart`/`Ended`, the baking and
      texture-state events, and the async-loading trap:
      **`ProjectEditionEntered`, not `ProjectOpened`,** means ready to work with.

> 🔴 **The 2026-08-31 block on this item was FALSE, and it cost four days.**
> It read: *"Substance 3D Painter is not installed on this machine, so the in-app
> documentation is not reachable here either."* **Painter 12.1.4 is installed**,
> at `C:\Program Files\Adobe Substance 3D Painter`, and it ships the complete
> Python API documentation at `resources\python-doc` — **53 HTML pages**, Python
> API **0.3.5**, reachable in-app via Help → scripting documentation. Every other
> finding in that block was correct: Adobe's public `ptpy/` paths really do
> redirect to a generic page, the `curl` status-code probe really does give false
> 200s on that site, and the Experience League plugins page really does document
> the legacy JS/QML API rather than the Python one. The single unverified claim
> was the one about this machine — and it was the one that closed the door.
>
> **The lesson is the same one this file already teaches, pointed at the machine
> instead of the corpus: suspect the instrument before the data.** A claim about
> the local environment is a measurement like any other, it goes stale, and it is
> cheaper to re-run than any of the ingests it blocks. Re-check before treating
> "not installed / not available here" as a blocker, and prefer recording the
> command that would settle it over recording the conclusion.

> ⚙️ **How these were ingested — reusable for any bundled/local doc set.**
> `ingest.py` takes a `file://` URL directly (`urllib.request.urlopen` handles
> the scheme), so no new flag was needed:
> `python ingest.py "file:///C:/Program%20Files/Adobe%20Substance%203D%20Painter/resources/python-doc/substance_painter/ui.html" --skip-video --title "Python API: ui Module" --author "..."`
> — percent-encode the spaces, or build the URI with `pathlib.Path(...).as_uri()`.
> Two cautions, both learned by reverting a commit:
> **(1) Sphinx `index.html` pages are tables of contents.** `plugins/index.html`
> yielded 673 chars of real content and was reverted as a stub — measure with
> `fetch_article()` before ingesting a doc set, not after.
> **(2) A dotted module name collapses in the slug**: "substance_painter.export
> Module" became `substance-painterexport-module`. Titled as
> `Python API: export Module` instead.
> This ingest also exposed a real defect, fixed across all five skills: the ASR
> hallucination safeguard was running on article text that never went through
> ASR, and flagged the `export` page because its closing code example
> legitimately repeats "export" 10×. `run_safeguards()` now takes `is_asr`.

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

### 2. ✅ Channel packing — **CLOSED 2026-09-04** — **4** (was 1)

- [x] **Channel packing** — what goes in which channel, and why
      ✅ `python-api-export-module.md` (2026-09-04) — the **mechanism** in Painter:
      an export preset's `channels` block is channel packing expressed as
      configuration (`destChannel` / `srcChannel` / `srcMapType` / `srcMapName`),
      with the rule that besides alpha you must specify either **R+G+B or L
      only**, and a colour source read into `L` mixes R+G+B.
      ✅ `godot-standard-material-3d-and-orm-material-3d.md` and
      `unity-metallic-mode-reflections-and-channels.md` — the **reasoning**: what
      each engine actually wants, which is the half the mechanism cannot tell you.
      **They disagree, and that is the point** — Godot ORM is one texture with
      Occlusion/Roughness/Metallic in RGB, while Unity's metallic workflow is
      **R = Metallic, G and B unused, A = Smoothness**. Unity also wants
      *smoothness*, the inverse of the roughness Painter authors, so a preset must
      **invert** that channel rather than merely re-route it. One preset cannot
      serve both engines, and now the library says why.

### 3. ✅ Unity and Godot export — **CLOSED 2026-09-04** — Unity **5** (was 2), Godot **3** (was ZERO)

- [x] **Export presets for Unity and Godot**
      ✅ `unity-metallic-mode-reflections-and-channels.md` — the metallic and
      specular packings, URP vs Built-In workflow selection, and Unity's own
      notice that the **Built-In Render Pipeline is deprecated** (supported
      through the Unity 6.7 LTS lifecycle).
      ✅ `godot-standard-material-3d-and-orm-material-3d.md` — **the direct answer
      to "how do I export for Godot": use Painter's Unreal Engine export preset**,
      because Unreal uses ORM too. Godot's documentation states this outright;
      Adobe's reachable documentation does not state it anywhere.
      ✅ `godot-model-export-considerations.md` — the mesh side of the same
      handoff: the right-handed Y-up -Z-forward convention (and that an oriented
      asset's **front is +Z**, so **+Y is rear in Blender**), triangulating in the
      DCC rather than trusting import-time triangulation with N-gons, applying
      transforms, and exporting at rest pose.

> ⚙️ **Why engine documentation is filed in a Substance skill.** These pages are
> the *receiving end* of a Painter export and they answer what Painter's own docs
> do not: **which packing the target wants**. It is a deliberate choice, recorded
> so nobody later reads it as scope drift.
>
> 🔴 **Adobe's Substance 3D Painter user documentation is still unreachable —
> re-probed 2026-09-04.** `helpx.adobe.com/substance-3d-painter/using/export.html`
> and the Experience League `user-guide/exporting/export-presets` path both **404**,
> and `substance3d.adobe.com/documentation/spdoc/...` still redirects to a generic
> **2,876-character** page with **zero** topic hits — the same false-positive
> pattern D4b recorded on 2026-08-31, confirmed a second time a week later.
> **Painter 12.1.4 is installed here and ships only API documentation**
> (`python-doc`, `javascript-doc`, `qml-doc`, `shader-doc`) — **no user manual** —
> so the bundled-docs route that closed gap #1 does not reach these topics.
> Engine vendors are the reliable first-party source for the export question.

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
