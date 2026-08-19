---
class: release-notes
verified: partial
sources:
  - https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/version-12-0
  - https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
last_verified: never
version_basis: "painter 12.0"
---
# Substance 3D Painter 12.0 — Release Notes

**Released:** 12.0.0 — March 9, 2026 · Patches: 12.0.1 (March 18, 2026, hotfix), 12.0.2 (April 7, 2026), 12.0.3 (May 5, 2026)
**Type:** Stable

## Added
- **Flatten Layers** directly in the layer stack (`Ctrl/Cmd + M`), with an option to export the flattened result to disk
- **Automatic warping for Warp projections** ("Warp to Geometry") — decals/projections adapt to complex surfaces without manual grid editing
- Entirely **new post-processing effects system**: depth of field, bloom, glare, lens flare, lateral (chromatic) aberration, vignette, sharpen, film grain, tone mapping, color correction — replaces and expands the previous post-effects set, with an updated tone mapper and a default post-effects asset library
- Redesigned **New Project** window and project-settings UI, with easier mesh re-importing
- `*.geo.usd` file support; USD library bumped to v25.05
- Substance Engine 9.3.4; Qt 6.8.6; JavaScript API 1.1.20; **Python bumped to 3.13**
- AMD GPU driver minimum requirement **raised** (25.3.1 / 25.Q2)
- Flatten instanced layers across Texture Sets; multi-channel selection in Texture Set settings; undo-entry wording updated; fill effects now default to white in masks; mesh hard-edges exposed as engine maps; shader-name collision prevention; shader import directly from project templates
- Python: smart-material saving to specific locations (from 12.0.3); Auto-unwrap Python API exposure and OCIO color-space specification for the color picker (from 12.0.2)

## Changed
- Post-processing effects were **replaced wholesale** with a new system and updated tone mapper — pre-12.0 post-effect stacks/parameter names do not map 1:1 onto the new set.
- Fill effects inside masks now default to **white** rather than whatever the previous default was — mask-authoring tutorials assuming the old default fill will look different on a fresh layer.
- Bundled Python runtime moved to **3.13** (from 3.11 in the 10.1/11.x line).
- AMD GPU driver minimum requirement raised — older-but-previously-supported AMD driver versions may now be flagged as unsupported.

## Removed / Deprecated
- The pre-12.0 post-effects stack is superseded by the new post-processing system (old individual effect nodes are not present under their old names).

## Breaking Changes & Migration Notes
- **What breaks:** Tutorials describing "flatten your layers by baking/re-importing textures as a new base layer" predate the native **Flatten Layers** command; the manual technique still works but is now unnecessary busywork.
  **Workaround:** Select the layers to merge and press `Ctrl/Cmd + M` (Flatten Layers) instead of the old bake-and-reimport dance.
- **What breaks:** A pre-12.0 tutorial's post-effects panel (names, sliders, tone-mapper controls) will not match 12.0+ — the whole post-effects pipeline changed.
  **Workaround:** Treat old post-effects tutorials as conceptual guidance only; rebuild the look using the new depth-of-field/bloom/glare/vignette/tone-mapping controls introduced in 12.0.0.
- **What breaks:** A fresh mask/fill-effect in 12.0+ starts **white** by default where an older tutorial may show/expect black (or vice-versa depending on the specific pre-12.0 default being referenced).
  **Workaround:** Explicitly check the mask's initial fill color rather than assuming it matches an older tutorial's starting state.
- **What breaks:** Custom Python plugins pinned to Python 3.11-only behavior (bundled through 11.x) should be re-tested under 3.13.
  **Workaround:** Re-test plugins after upgrading; check for use of any stdlib behavior removed/changed between 3.11 and 3.13.
- **What breaks:** AMD users on older GPU drivers may find Painter refuses to start correctly or warns about driver support after upgrading to 12.0+.
  **Workaround:** Update AMD drivers to at least the 25.3.1 / 25.Q2 line before troubleshooting further.

## Known Issues (12.0.0)
- Crash possible when changing a material channel's output assignment inside a mask
- EXR textures could be force-imported as sRGB instead of linear when going through USD
- Image sequences with a single image could incorrectly fill other UV Tiles
- AO baking could differ slightly between CPU and GPU results
- macOS: viewport BaseColor color management could mismatch export

## Sources
- https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/version-12-0
- https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
