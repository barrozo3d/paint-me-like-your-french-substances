# Substance 3D Painter 10.1 — Release Notes

**Released:** 10.1.0 — September 17, 2024 · Patches: 10.1.1 (November 5, 2024), 10.1.2 (December 3, 2024)
**Type:** Stable

## Added
- New filters: Fill Area mask/color, Embroidery decal, and 6 generic Substance filters (FXAA, pixelate, highpass, posterize, smoothstep, threshold)
- **USD material/shader property export and import**
- Optimized layer-stack thumbnails and faster project-file opening
- **VFX Platform 2024 compliance**: Python bumped to **3.11**, OpenEXR 3.2, OpenSubdiv 3.6.0, OCIO 2.3.2
- **Linux distribution migrated to RedHat-based** packaging
- GLTF normal-map flip option
- New splash-screen format; Python "layer stack" example link added to docs; JavaScript plugins folder reorganized
- 10.1.1: asynchronous baking save for UV Tiles; Auto Unwrap 1.3.2 with seaming; multiple-UV-set support with sparse data; OpenEXR bumped to 3.4.4
- 10.1.2: fixes only (image-input deletion crash, Smart Material layer-stack addition, `GroupLayerNode` effects retrieval)

## Changed
- Linux build now targets a **RedHat-based** distribution rather than the previous base — Linux install/dependency instructions from before September 2024 may not apply as-is.
- Bundled Python runtime moved to **3.11** (from 3.9 in the 8.x line) to match VFX Platform 2024 — custom plugins relying on 3.9-only syntax/stdlib behavior should be re-tested.
- JavaScript plugins folder layout reorganized.

## Breaking Changes & Migration Notes
- **What breaks:** Linux users following pre-10.1 installation guides (targeting the old Linux base) may hit missing-dependency issues after upgrading, since the app package itself moved to a RedHat-based build.
  **Workaround:** Follow current official Linux installation instructions for the RedHat-based package rather than a pre-2024 guide.
- **What breaks:** Custom Python plugins pinned to assumptions about Python 3.9 behavior (bundled in the 8.x/9.x line) should be checked against 3.11 semantics.
  **Workaround:** Re-test plugins under the bundled interpreter after upgrading; the `substance_painter` module API itself did not remove functionality in this release, but the underlying interpreter did change.
- **What breaks:** JavaScript plugin folder paths referenced by older automation/setup scripts changed due to the reorganization.
  **Workaround:** Re-locate plugin folders under the current documented path before assuming a script's hardcoded path is still valid.

## Sources
- https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
