# Substance 3D Painter 8.1 — Release Notes

**Released:** 8.1.0 — June 7, 2022 · Patches: 8.1.1 (June 28, 2022), 8.1.2 (July 19, 2022), 8.1.3 (August 25, 2022)
**Type:** Stable

## Added
- **ICC profile support** via the new **Adobe Color Engine (ACE)** — Adobe 98 RGB working color space, ACE/ICC configuration file, per-project color-profile selection for external color picking
- "Legacy" color-management mode retained alongside ACE, with linear color-value input available there
- **Physical Size** features: mesh extraction/computation, UI options, visual helpers (foundation for later physical-size-aware projection/displacement work in 9.x–11.x)
- Three new bakers: **Height**, **Bent Normals**, **Opacity**
- Color eyedropper overhaul: preview swatch, click-to-select, dedicated shortcut, panel-position retention, disabled-state handling
- glTF tangent-attribute export
- Substance Engine 9.1.2, Auto Unwrap 0.9.0, Qt 5.15.8, Python 3.9
- Bent Normals shader support; MacOS 3DConnexion SpaceMouse support
- New 3D noises with presets, grunge maps, cloth patterns; "Mesh maps" export preset updated
- 8.1.2: Auto Unwrap organic-mesh segmentation algorithm option; Physical Size unit options; GLTF Displacement export preset; Blender project template + export preset
- 8.1.3: Iray SDK 1.6 update (bugfix release)

## Changed
- Adobe Color Engine (ACE) becomes the primary/default color-management path introduced alongside — not replacing — the OCIO-based Legacy mode from 7.4/8.0. Projects and color pickers now distinguish explicitly between ACE and Legacy behavior.
- Height, Bent Normals, and Opacity mesh maps can now be baked **natively** with dedicated bakers instead of requiring manual workarounds (external DCC roundtrips or shader tricks) that older tutorials describe.

## Breaking Changes & Migration Notes
- **What breaks:** Tutorials that describe baking "height", "bent normals", or "opacity" maps via manual filter stacks, external tools, or `Ambient Occlusion` re-purposing (common in pre-2022 content) are describing a workaround that is no longer necessary.
  **Workaround:** Use the native **Height**, **Bent Normals**, and **Opacity** bakers directly in the Bake Mesh Maps settings — same place as Ambient Occlusion/Curvature/Normal bakers.
- **What breaks:** Color picked/typed values may look different than in pre-8.1 projects if a project or preference is using ACE instead of Legacy color management.
  **Workaround:** Check Edit > Project Configuration / Preferences for the active color-management engine (ACE vs Legacy) before comparing values against an older tutorial's screenshots.

## Known Issues (8.1.0)
- Special-character filenames could crash glTF export
- Anisotropy artifacts with Sparse Virtual Textures
- macOS Apple Silicon (M1) smart-material display issues

## Sources
- https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
