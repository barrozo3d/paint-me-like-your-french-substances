# Substance 3D Painter 10.0 — Release Notes

**Released:** 10.0.0 — May 16, 2024 · Patch: 10.0.1 (June 11, 2024)
**Type:** Stable

## Added
- **Native Adobe Illustrator file support**, including artboard selection and Illustrator/SVG scope-selection previews
- **Substance 3D Assets panel** — browse, download, and reload assets directly from Adobe's library inside Painter (environments and materials included); a dedicated asset download manager
- Embeddable/custom font support: font and text-mesh rendering, user/shared font paths, advanced font properties, font search in mini-shelves
- Fill Area mask/color filter; Embroidery decal filter; 6 new generic Substance filters
- **Major Python API expansion**, most notably a **layer-stack Python "edition"** giving scripts direct control of the layer stack (create/select/reorder layers, effects, and masks) for building advanced plugins/custom tools, plus: blending-mode access from Python, fill-layer projection-settings access, Substance material color queries, uniform color/resource access in layers/effects, text-resource creation/editing, active-channel editing, batch undo/redo, vectorial-source parameter editing, color-property editing with color management, instanced-layer queries/creation, bitmap image color-management access, engine pause/unpause, sibling/parent navigation, filter/generator/Level effect creation from script, smart-mask creation, anchor-point creation/editing, layer-mask creation, compare-mask effect, Substance preset queries, export-preset listing/content retrieval
- Manipulator precision mode (hold CTRL) and improved manipulator surface stability
- 10.0.1: Substance-font-to-regular-font conversion; Illustrator/SVG scope-selection backgrounds; Python bitmap-source color-space queries

## Changed
- Substance Painter's Python layer-stack access moved from indirect/limited calls to a first-class, documented API surface — plugins that previously poked at internal structures or relied on workarounds to read/write layer-stack state should migrate to the new API.

## Breaking Changes & Migration Notes
- **What breaks:** Older custom Python plugins written before 10.0.0 that manipulate layers via undocumented/roundabout means may be superseded by (and should be rewritten against) the new layer-stack module — Adobe explicitly calls this out as the headline scripting change of the release.
  **Workaround:** Rebuild layer/effect/mask automation using the documented layer-stack API introduced in 10.0.0 rather than legacy workarounds.
- **What breaks:** Tutorials that manually download assets from the Substance Source website and import them by hand predate the in-app **3D Assets panel**; the panel is an additive convenience, so the manual method still works, but current tutorials increasingly assume the panel exists.

## Known Issues
- Shader-instance deletion could crash in some cases
- Save-project failures possible under specific network/disk conditions
- Linux/AMD Wayland drag-and-drop crashes
- MacOS Intel preset crashes (Apple Silicon unaffected)

## Sources
- https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
