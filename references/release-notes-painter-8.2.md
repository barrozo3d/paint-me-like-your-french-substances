---
class: release-notes
verified: partial
sources:
  - https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
last_verified: never
version_basis: "painter 8.2"
---
# Substance 3D Painter 8.2 — Release Notes

**Released:** October 6, 2022
**Type:** Stable

## Added
- **Welcome screen** for new users and a **What's New** panel for feature discoverability (Home screen renamed from Welcome)
- High-DPI scaling improvements
- Save menu reorganization; UI-layout save/export/reload
- Blending-mode/opacity copy-paste for layers, and one-click application of a blending mode/opacity to all channels
- Mesh-reload keyboard shortcut (CTRL+SHIFT+R)
- Substance parameter reset button (including per-parameter reset via right-click); paint-brush default reset
- Favorite-asset pinning, and asset deletion/reload/rename directly in the user library (Assets panel)
- Color Selection blending modes; filter blending modes/opacity
- Increased tiling limits for fill layers/effects
- Cylindrical-projection cylinder-caps option
- SBSAR texture export option; EXR 16-bit/32-bit export options
- Python: `TextureStateEvent` for Texture Set modification; mesh-map resource queries; new `substance_painter.resource.Type` enum values; methods to query child/parent resources
- Roblox project template and export preset
- Substance Engine 8.6.3; Apple Silicon (M1/M2) optimization pass

## Changed
- Save menu structure reorganized (menu items users may know from pre-8.2 tutorials moved)
- UI layouts can now be saved/exported/reloaded as named presets rather than only the single built-in default

## Breaking Changes & Migration Notes
- **What breaks:** Tutorials pointing to specific Save-menu entries by position/wording from before October 2022 may be slightly off after the menu reorganization.
  **Workaround:** Use the menu search (or the What's New panel introduced in this same release) to relocate the renamed/moved item.

## Known Issues
- 16K EXR imports could crash on some configurations
- Ctrl+Z after shader-instance deletion could crash
- Iray IoR parameter could block render start in some material setups

## Sources
- https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
