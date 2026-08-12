# Substance 3D Painter 8.3 — Release Notes

**Released:** 8.3.0 — January 10, 2023 · Patch: 8.3.1 (April 27, 2023)
**Type:** Stable

## Added
- **Dedicated Baking Mode** (new top-level mode, shortcut **F8**) — replaces the old inline "Bake Mesh Maps" workflow embedded in Texture Set Settings
  - New Baking Mode UI: Start/Cancel buttons, Texture Set list, Mesh Map windows, Baking Log, breadcrumb navigation, mesh-map thumbnails
  - Visualization toggles: show/hide meshes, cage, wireframe, low-poly, hard edges; implicit-cage display; neutral-material viewport display during baking
  - Baker-settings synchronization across Texture Sets, with copy/paste of baker settings and per-Texture-Set baker/common settings management
  - Baking Log errors jump directly to the offending setting
  - Asynchronous mesh loading and a viewport progress bar during bakes; baking order follows visibility order
  - Anti-aliasing labels/multipliers exposed; bakers updated to 2.5.7
- **USD import/export** support, including Scope and Variants selection, subdivision-levels option, skinned-mesh frame selection, a renamed USD PBR export preset, and a dedicated USD mesh export format
- Lock Orientation option for UV packing
- Automatic Physical Size switching for fills; Physical Size support in UV projection
- Python: application-version query; JavaScript API baking updates; new Python **baking module** — parameters, launch/cancel, curvature method, baker/tile selection, baking-settings synchronization
- AMD GPU: Sparse Virtual Textures support
- Cylindrical-projection parameters renamed
- 8.3.1: Baking-mode visualization show/hide shortcut; persistent Low Poly display; "Matching By Name" Texture Set suffix; **GLB (binary glTF) import support**; Texture Set resolution quick-change; Python baking-event exposure, bake cancellation, export-template bit-depth exposure, `TextureStateEvent` refresh-time control

## Changed
- Baking is no longer a dialog reached from Texture Set Settings — it is a **full dedicated application mode** with its own navigation, log, and per-Texture-Set/per-baker settings management.
- Cylindrical projection parameter names changed (existing scripts/presets referencing the old parameter names need updating).

## Removed / Deprecated
- The old inline "Bake Mesh Maps" panel/dialog embedded in Texture Set Settings is superseded by the dedicated Baking Mode.

## Breaking Changes & Migration Notes
- **What breaks:** Any tutorial from before January 2023 that says "open Texture Set Settings and click Bake Mesh Maps" is describing a UI that no longer exists in this form.
  **Workaround:** Press **F8** (or use the mode switcher) to enter the dedicated Baking Mode; Texture Set selection, baker settings, and the Start button all live there now. The underlying bakers and their parameters are the same — only the surrounding UI moved.
- **What breaks:** Python plugins/scripts that drove baking via pre-8.3 API calls should be checked — the Python `baking` module was introduced fresh in this release to match the new Baking Mode (parameter access, launch/cancel, baker/tile selection, settings sync).
  **Workaround:** Re-point custom baking scripts at `substance_painter.baking` (module introduced 8.3.0) rather than any pre-8.3 ad-hoc baking calls.
- **What breaks:** Cylindrical projection presets/scripts using the old parameter names will not map 1:1.
  **Workaround:** Re-check cylindrical projection parameter names in the Properties panel after upgrading and re-save any affected presets.

## Known Issues
- Crashes possible when: changing channels on a filter; creating a fill layer on Apple Silicon; calling `ui.add_dock_widget()` from Python; freeing memory after baking; toggling effect visibility with a cached texture
- Incomplete/unclear baking error messages in some failure cases
- TAA (temporal anti-aliasing) artifacts visible while painting

## Sources
- https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
