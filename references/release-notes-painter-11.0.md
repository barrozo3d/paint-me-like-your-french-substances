---
class: release-notes
verified: partial
sources:
  - https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
last_verified: never
version_basis: "painter 11.0"
---
# Substance 3D Painter 11.0 — Release Notes

**Released:** 11.0.0 — March 11, 2025 · Patches: 11.0.1 (April 10, 2025), 11.0.2 (June 10, 2025), 11.0.3 (August 5, 2025)
**Type:** Stable

## Added
- **Auto-update** feature for modified assets (optional parameter-matching), exposed to Python
- **Filled Path tool** — supersedes the original 9.0 "Paint along Path" tool: path snapping to polygons, path-type switching, copy/paste of vertex data, angle/line constraints, single-click shape closing, vertex scale/rotate, transformation gizmos, path preview (Shift+P), improved tangent editing, 3D path focus, persistent path list, duplicate-on-copy renaming
- Experimental **Auto-cage generation** for baking (Python API included)
- 6 new filters: stylization, quantize, anisotropic Kuwahara, bevel smooth, directional distance, grayscale conversion; updated Noises/Grunges; 3 new texture generators
- Unreal Engine project template **renamed**
- Python: Smart Material/Smart Mask saving; Auto-cage API; Texture Set/UV Tiles name & description editing; Auto-update exposure
- Vector & Font source resolution sharing
- Nvidia driver minimum-version warning; UV Tiles custom naming
- macOS: **Metal rendering**; **macOS Intel (x86_64) support dropped — Apple Silicon only from this release forward**
- 11.0.2: multi-UV-set support with sparse data; Auto-unwrap 1.3.2 with seaming
- 11.0.3: ACES 2.0 config; OCIO 2.4.2; Iray 2024.10; Nvidia driver minimum raised again

## Changed
- Path-based painting is now the **Filled Path** tool, replacing the original 9.0.0 Path tool's UI and interaction model (snapping, constraints, gizmos are new; some 9.0-era shortcuts/behaviors do not carry over)
- The Unreal Engine export/project template was renamed — export presets or documentation referencing the old template name by exact text will not find it under that name
- **macOS Intel builds are no longer supported or shipped** — this is a hard platform cut, not a deprecation warning

## Removed / Deprecated
- macOS Intel (x86_64) support removed entirely; Apple Silicon (ARM64) required on Mac from 11.0.0 onward

## Breaking Changes & Migration Notes
- **What breaks:** Any tutorial demonstrating Path-tool workflows using 9.0-era gestures/shortcuts will look and behave differently under the 11.0 Filled Path tool (new snapping/constraint/gizmo behavior).
  **Workaround:** Treat pre-11.0 Path-tool tutorials as conceptually valid but expect different tool options and shortcuts; consult current in-app tooltips for the Filled Path tool.
- **What breaks:** Users on an Intel-based Mac cannot run Substance 3D Painter 11.0.0 or later at all.
  **Workaround:** Apple Silicon (M-series) Mac required, or stay on the last 10.1.x release if hardware can't be upgraded.
- **What breaks:** Export presets/scripts that hardcode the old Unreal Engine template name will not match after the rename.
  **Workaround:** Re-select the Unreal Engine template/preset by browsing the current list rather than relying on a saved exact name string.

## Known Issues (11.0.0)
- HDR color-space conversions could be inconsistent
- Right-click context-menu sizing issues
- USD export from `TextureStateEvent` unreliable
- Clone tool could shift colors on the normal channel
- "Ghost" UI widgets could persist after certain actions
- RedHat: color-picker issues

## Sources
- https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
