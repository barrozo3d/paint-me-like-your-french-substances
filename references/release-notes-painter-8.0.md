---
class: release-notes
verified: partial
sources:
  - https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
last_verified: never
version_basis: "painter 8.0"
---
# Substance 3D Painter 8.0 — Release Notes

**Released:** 8.0.0 — March 8, 2022 · 8.0.1 — April 11, 2022 (patch)
**Type:** Stable

## Added
- 3DConnexion SpaceMouse support for 3D Viewport navigation (Windows only at this point; SpaceMouse 2D Viewport support followed in 8.0.1)
- SpaceMouse shortcuts/keys and a rotation-center icon
- Expanded OpenColorIO (OCIO) Color Management: configuration roles, default OCIO configurations, environment-variable override, color-space filename extraction, per-property color-space override
- Color Management extended to the Properties window (color widgets, material preview, swatches) and to the color picker (Display dropdown for color-space selection, gradient customization)
- Standard sRGB color-space definition
- Separate color management for the 2D and 3D viewports; environment-map color management/conversion
- Display-transform dropdown in the viewport and Iray rendering display transform
- Texture export color spaces exposed
- Python: OCIO environment-variable application
- Viewport 2D/3D undocking
- Auto Unwrap: elongated-island avoidance
- JavaScript can call Python functions
- New Project window: imported maps list made collapsible
- Projection/Warp: option to hide normals
- New content: grunge maps, tool presets, materials (scar, pocket, etc.), inflated shrinkwrap generator

## Changed
- Color management is now applied consistently across Properties, material preview, swatches, and both viewports rather than being limited to texture I/O

## Known Issues
- SpaceMouse not yet supported on macOS
- Color Management UI needs horizontal scrollbars in some layouts
- Normal mesh maps could bake inverted in certain configurations
- Substance angle-widget defaults inconsistent
- UV Tile overlay issues
- Python: some channel-query calls unreliable

## Sources
- https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
