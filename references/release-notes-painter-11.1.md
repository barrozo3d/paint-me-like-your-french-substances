# Substance 3D Painter 11.1 — Release Notes

**Released:** 11.1.0 — November 18, 2025 · Patches: 11.1.1 (December 9, 2025), 11.1.2 (January 13, 2026), 11.1.3 (February 12, 2026)
**Type:** Stable

## Added
- **Ribbon tool** — a new dedicated tool for painting seamless strokes/paths, with its own preset shortcuts, 75 new presets, per-vertex opacity/size adjustment, closed-path end removal, alpha/channel blending modes, and Gradient Builder compatibility
- **Fill symmetry support**, with viewport and Properties UI
- Normal-texture reorientation in Warp mode; physical-size displacement units
- **Full Vulkan rendering support (Windows/Linux)**, alongside the existing DirectX/OpenGL backends
- Tool-properties panel reorganization
- Substance resolution override specifically for Tools/Fills
- Mesh Maps export preset updated (again)
- Python: fill-symmetry exposure
- 11.1.1: UV Tiles partial-texture computing (performance); Bakers updated to 3.15.4
- 11.1.2: asynchronous baking save for UV Tiles refined further; OpenEXR 3.4.4

## Changed
- Path/stroke painting gains a **second** dedicated tool (Ribbon) alongside the 11.0 Filled Path tool — Path and Fill tools' preview options were also removed/consolidated in this release ("Path/Material preview removal for paint tools")
- Tool Properties panel layout reorganized — controls tutorials describe by position/tab may have moved
- Rendering backend now includes **Vulkan** as a full option on Windows and Linux, not just DirectX(Windows)/OpenGL — default backend selection dialogs/behavior can differ from pre-11.1 setups

## Breaking Changes & Migration Notes
- **What breaks:** A tutorial showing the **Ribbon** tool assumes 11.1.0+; on earlier versions this tool does not exist — use Filled Path (11.0+) or the original Path tool (9.0+) instead, understanding neither has Ribbon's stroke/alpha-blending feature set.
  **Workaround:** Map "Ribbon" tutorial steps conceptually onto whichever path/stroke tool actually exists in the target version.
- **What breaks:** Old troubleshooting advice that says "switch to OpenGL if you have rendering issues" predates full Vulkan support; on 11.1+, Vulkan is often the better first thing to try instead, especially on Windows/Linux with recent GPU drivers.
  **Workaround:** Check Edit > Settings > Rendering backend and try Vulkan if a pre-2025 tutorial's OpenGL/DirectX troubleshooting step doesn't apply cleanly.
- **What breaks:** Tool Properties panel screenshots/step references from before November 2025 may not match current tab/control placement.
  **Workaround:** Use the in-app tool tooltip/search rather than relying on exact panel position from an older screenshot.

## Known Issues (11.1.0 / 11.1.1)
- Ribbon tool: reduced performance specifically on UV Tiles projects
- Path overlapping artifacts after corners in certain stroke configurations
- Long text input could crash the app in some dialogs
- HDR color-space conversion inconsistencies persist
- Right-click menu sizing issues persist
- USD export from `TextureStateEvent` still unreliable
- Clone tool could still shift colors on the normal channel
- "Ghost" UI widgets could still persist after certain actions

## Sources
- https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
