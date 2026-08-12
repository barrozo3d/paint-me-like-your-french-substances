# Substance 3D Painter 12.1 — Release Notes

**Released:** 12.1.0 — June 23, 2026 · Patches: 12.1.1 (July 9, 2026), 12.1.2 (August 3, 2026)
**Type:** Stable

## Added
- **OpenPBR 1.1 support**, available as the **default shading workflow** for new projects/materials — a new entry in the New Project window is labeled "OpenPBR" (replacing ASM as the first/default entry), OpenPBR material/texture import/export via USD, new OpenPBR project templates, updated sample projects
- **Skew Painting** workflow inside Baking Mode: paint skew-correction maps directly on the mesh using brush or Polygon Fill tools, with a dedicated Skew Preview shader/direction vectors and an **Edge Protection** option
- **Auto rebake**: toggle per mesh map to automatically and incrementally rebake just the affected region whenever a baking setting changes (auto-enabled in Skew Painting mode, toggleable elsewhere)
- Reworked Baking Mode UI: mesh-map list redesigned, settings split into **Mesh Map Settings** vs **Common Settings**
- Unified undo history between Baking Mode and painting mode
- **Hard Surface Auto Unwrap** — a new automatic-UV-unwrapping mode tuned for mechanical/hard-surface meshes; distortion-minimizing and orthographically-aligned, and noticeably faster than the default (organic) auto-unwrap algorithm
- Symmetry toggle added to the toolbar; grayscale color-picker variant
- Geometry Mask API expanded to support inclusion/exclusion modes matching the UI
- Adobe Color Engine bumped to v7.0
- **Minimum macOS version raised to 13.0 (Ventura)**
- 12.1.1: Skew Base Normal Mode exposure (mesh-based or per-triangle); uniform colors reset to channel defaults; OpenPBR channels now grouped by category in the UI; Substance engine 9.4.5
- 12.1.2: stability-only patch (crash fixes — see Known Issues note below)

## Changed
- **OpenPBR is now the default workflow for new projects and templates without an explicit template chosen.** Existing/older projects are **not** auto-converted: they keep whichever shader (ASM / PBR MetalRough / custom) they were authored with when reopened.
- Importing a USD or glTF file now sets the shader from the **project template** rather than being guessed from file content; a log message is emitted when a material's workflow and the project template's workflow mismatch.
- The Export Textures window now defaults to the OpenPBR channel scheme when at least one shader in the project uses OpenPBR; the selected channel scheme is shown per Texture Set in the map list.
- The **Shader API changed to support OpenPBR** — author-written custom shaders using the Shader API may need updating to remain compatible.
- Baking Mode's mesh-map settings UI reorganized a second time (first overhaul was the 8.3.0 dedicated Baking Mode) — split into Mesh Map Settings and Common Settings panels.

## Breaking Changes & Migration Notes
- **What breaks:** A tutorial made before June 2026 that starts a "New Project" and expects the default/first template to be ASM / PBR Metal Roughness will instead land on **OpenPBR** by default.
  **Workaround:** Explicitly pick a PBR Metal Roughness / ASM template from the New Project window if the tutorial's channel names (e.g. `baseColor`, `metallic`, `roughness`) and shader parameters need to match an ASM-era workflow. OpenPBR uses a different channel/parameter set (grouped by category as of 12.1.1) — do not assume 1:1 channel-name parity with ASM/MetalRough tutorials.
- **What breaks:** Old projects are safe to open — Painter does **not** silently convert an existing ASM/MetalRough-authored project to OpenPBR. But re-exports or new materials added inside that project may default to OpenPBR channel schemes unless the user deliberately keeps the original shader/template.
  **Workaround:** When continuing an old project, check which shader each Texture Set/material actually uses (Texture Set Settings) before assuming it's on OpenPBR just because the app version is new.
- **What breaks:** Any custom shader written against the pre-12.1 Shader API (`.glsl`-based custom shaders, common in advanced pipeline tutorials) may not load/behave correctly until updated for the OpenPBR-era Shader API.
  **Workaround:** Re-check custom shader code against the current Shader API reference; expect required updates if the shader predates June 2026.
- **What breaks:** Baking Mode's settings panel (introduced 8.3.0) is now split into "Mesh Map Settings" and "Common Settings" — screenshots/steps from 8.3.0–12.0.x tutorials referencing a single combined settings panel will not match.
  **Workaround:** Look for the setting under both sub-panels; per-mesh-map options moved to Mesh Map Settings, shared options to Common Settings.
- **What breaks:** macOS users on 12.x (Monterey) or older cannot run 12.1.0+.
  **Workaround:** Upgrade to macOS 13 (Ventura) or later, or remain on 12.0.3 if the OS cannot be upgraded.
- **Performance note (12.1.0 only, fixed in 12.1.1):** Multiple users reported severe project save/load/close slowdowns after upgrading to 12.1.0, described by Adobe as hardware-dependent. This was addressed in the **12.1.1** patch ("Fixed: Project opening/saving delays"). If a tutorial or forum post from June–early July 2026 mentions this issue, it does not apply once on 12.1.1+.
  **Workaround:** Update to 12.1.1 or later if still on 12.1.0 and experiencing slow save/load.

## Known Issues
- 12.1.0 (pre-12.1.1): significant save/load/close performance regression on some hardware (fixed in 12.1.1 — see above)
- 12.1.2 was released specifically to fix crashes in: Substance rendering, mesh reimport during baking, graphics initialization, texture export, baking with environment maps, baking freezes on high-poly file changes, Photoshop layer-mask export, and anchor-point rendering between masks and color channels — treat any of these symptoms on 12.1.0/12.1.1 as resolved once updated to 12.1.2

## Sources
- https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/version-12-1
- https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
- https://community.adobe.com/announcements-57/substance-3d-painter-12-1-is-here-auto-rebake-openpbr-support-and-more-1629231 (official Adobe Community announcement — secondary confirmation of migration/shader behavior)
