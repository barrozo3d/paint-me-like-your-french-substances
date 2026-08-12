# Substance 3D Painter 9.1 — Release Notes

**Released:** 9.1.0 — November 7, 2023 · Patches: 9.1.1 (December 5, 2023), 9.1.2 (January 30, 2024)
**Type:** Stable

## Added
- **SVG (vectorial) file import**, with SVG-specific properties, proportion preservation, automatic alpha usage
- **After Effects interoperability** (AE 24.1, beta at first) with dedicated settings
- Drag-and-drop overhaul: auto-import on drag/drop, external-asset drag/drop into the layer stack, texture drag/drop from the Assets panel, generator/filter/asset drag/drop into the viewport, Smart Mask drag/drop, single-channel image drag/drop, CTRL/ALT drag/drop modifiers
- UV-set-to-UV-set projection mode
- Path tool: individual path visibility, transformation manipulators, manual per-vertex tangent control, copy/paste of path properties, break-tangent shortcut, persistent path preview (Shift+P)
- Adobe Standard Material (ASM) shader: Opacity & Translucency, Absorption color channel, parameter tooltips, default black Translucency, `ColorSpace` property support
- **Auto Unwrap texel-density control**
- Lossless 16-bit image compression
- Python: camera-manipulation API; mesh-export scripting; new SVG material filters (Custom Sticker, Custom Spray, Graphic to Material)
- Substance Engine 9.0.3
- 9.1.1: After Effects export bumped to AE 24.1 (stable)
- 9.1.2: fill-layer creation-time optimization; heavy environment-map loading optimization; project save/close without forced thumbnail generation

## Changed
- Drag-and-drop behavior across Assets panel, viewport, and layer stack was substantially expanded — many actions that previously required explicit menu commands (e.g. applying a texture, adding a Smart Mask) can now be done by dragging directly onto a target.

## Breaking Changes & Migration Notes
- **What breaks:** None severe; this is primarily additive. Tutorials showing manual "Add Layer > Import" style workflows for assets still work — drag/drop is an additional path, not a replacement.

## Sources
- https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
