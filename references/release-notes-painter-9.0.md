---
class: release-notes
verified: partial
sources:
  - https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
last_verified: never
version_basis: "painter 9.0"
---
# Substance 3D Painter 9.0 — Release Notes

**Released:** 9.0.0 — June 20, 2023 · Patch: 9.0.1 (September 19, 2023)
**Type:** Stable

## Added
- **Paint along Path** tool — the first version of a dedicated vector-path painting workflow: create/edit path points, per-vertex pressure, smooth/corner point conversion, automatic tangent adjustment, surface-point snapping, path reversal, marquee/CTRL+A point selection, path panel (create/rename/delete/copy/cut/duplicate), paint/erase/smudge modes along the path, path direction indicator and line-thickness display
- Dynamic Strokes: distance, size/spacing, and start/middle/end properties
- New content: path tool presets, base materials
- Python: 3D-view camera manipulation; mesh export scripting; USD project-configuration/creation/path-export parameters
- Substance Engine 9.0
- 9.0.1: default import location; baking-parameter reset; paint-resolution baking default; symmetry-manipulator unbinding from the Q key; "show log" option; Sbsar decal usage auto-warp; Path-tool interaction message

## Changed
- Symmetry manipulator no longer hard-bound to the Q shortcut by default (9.0.1) — old muscle-memory shortcuts may not respond the same way.

## Breaking Changes & Migration Notes
- **What breaks:** This is the *first* version of the Path tool. Tutorials describing painting along a path in Painter 9.0 use a tool that was substantially reworked twice later (**Filled Path** in 11.0.0, then replaced by the **Ribbon** tool in 11.1.0). Point/vertex editing gestures and the Path panel described here do not match 11.x+.
  **Workaround:** For any tutorial demonstrating "Paint along Path," check the Painter version in the video/article; on 11.1+ use the Ribbon tool instead (see `release-notes-painter-11.1.md`) — same conceptual goal (stroke-along-a-curve), different tool and UI.

## Known Issues
- GLB texture-import issues on AMD hardware
- 3D projection artifacts on AMD hardware
- Texture could appear empty when toggling layer visibility or certain blending modes/warp projection combinations

## Sources
- https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
