---
class: operational
verified: n/a
sources:
  - https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/release-notes
  - https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/beta
  - https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes
last_verified: never
version_basis: "unknown"
---
# Version Tracker

Tracks the known version history of Adobe Substance 3D Painter and when this file was last checked against Adobe's release-notes pages. Mirrors the Auto-Changelog Rule in `SKILL.md` (Mode 0).

- **last_checked:** 2026-08-12

## Known Versions (as of last_checked)

Newest first. `Details` links to the per-version release-notes file in this folder, or says "folded into vX.Y" when a patch release has no substantial changes of its own (see that parent file's "Patch notes" content within its Added/Changed/Fixed sections).

| Version | Release Date | Type | Headline Changes | Details |
|---|---|---|---|---|
| 12.1.2 | 2026-08-03 | Stable (patch) | Stability-only patch: crash fixes across rendering, baking, texture/mask export | folded into v12.1 |
| 12.1.1 | 2026-07-09 | Stable (patch) | Skew Base Normal Mode exposure, OpenPBR channel grouping by category, **fixes the 12.1.0 save/load performance regression** | folded into v12.1 |
| 12.1.0 | 2026-06-23 | Stable | **OpenPBR 1.1 becomes the default new-project workflow** (old projects keep their original shader — not auto-converted); Skew Painting/baking with Edge Protection; Auto rebake; Hard Surface Auto Unwrap; Baking Mode UI split into Mesh Map/Common Settings; **macOS minimum raised to 13.0 (Ventura)**; Shader API changed to support OpenPBR | [release-notes-painter-12.1.md](release-notes-painter-12.1.md) |
| 12.1 beta ("Skew & OpenPBR") | ~2026-04-07 (unverified — secondary source) | Beta | Open beta preview of the 12.1.0 feature set; **project save format not compatible with 12.0** | [release-notes-painter-12.1-beta.md](release-notes-painter-12.1-beta.md) |
| 12.0.3 | 2026-05-05 | Stable (patch) | Performance/stability; Python smart-material saving to specific locations | folded into v12.0 |
| 12.0.2 | 2026-04-07 | Stable (patch) | OCIO color-space picker for color picker; Auto-unwrap Python API exposure | folded into v12.0 |
| 12.0.1 | 2026-03-18 | Stable (patch) | Critical hotfix: export crash/freeze on specific projects | folded into v12.0 |
| 12.0.0 | 2026-03-09 | Stable | **Flatten Layers** in-stack (Ctrl/Cmd+M); Warp-to-Geometry auto-warping; entirely new post-processing effects system; redesigned New Project window; **Python bumped to 3.13**; AMD GPU driver minimum raised | [release-notes-painter-12.0.md](release-notes-painter-12.0.md) |
| 11.1.3 | 2026-02-12 | Stable (patch) | Stability patch (stencil/symmetry, Path smudge, color picker) | folded into v11.1 |
| 11.1.2 | 2026-01-13 | Stable (patch) | Performance/crash fixes; async UV Tiles baking save | folded into v11.1 |
| 11.1.1 | 2025-12-09 | Stable (patch) | UV Tiles performance; Bakers 3.15.4 | folded into v11.1 |
| 11.1.0 | 2025-11-18 | Stable | **Ribbon tool** (new seamless-stroke path tool); Fill symmetry support; **full Vulkan support (Windows/Linux)**; Tool Properties panel reorganized | [release-notes-painter-11.1.md](release-notes-painter-11.1.md) |
| 11.0.3 | 2025-08-05 | Stable (patch) | ACES 2.0 config, OCIO 2.4.2, Nvidia driver minimum raised | folded into v11.0 |
| 11.0.2 | 2025-06-10 | Stable (patch) | Import/export fixes, multi-UV-set sparse-data support | folded into v11.0 |
| 11.0.1 | 2025-04-10 | Stable (patch) | Qt 6.5.8, various fixes | folded into v11.0 |
| 11.0.0 | 2025-03-11 | Stable | Auto-update for modified assets; **Filled Path tool** (replaces 9.0's Path tool); experimental Auto-cage generation; **macOS Intel (x86_64) support dropped — Apple Silicon required from here on** | [release-notes-painter-11.0.md](release-notes-painter-11.0.md) |
| 10.1.2 | 2024-12-03 | Stable (patch) | Fixes only | folded into v10.1 |
| 10.1.1 | 2024-11-05 | Stable (patch) | Auto Unwrap seaming, async UV Tile baking save | folded into v10.1 |
| 10.1.0 | 2024-09-17 | Stable | **VFX Platform 2024 compliance** (Python bumped to 3.11); **Linux migrated to RedHat-based packaging**; USD material/shader property import/export | [release-notes-painter-10.1.md](release-notes-painter-10.1.md) |
| 10.0.1 | 2024-06-11 | Stable (patch) | Fixes; Substance-font-to-regular-font conversion | folded into v10.0 |
| 10.0.0 | 2024-05-16 | Stable | Native Adobe Illustrator support; Substance 3D Assets panel; **major Python API expansion — layer-stack "edition" module** for scripted layer/effect/mask control | [release-notes-painter-10.0.md](release-notes-painter-10.0.md) |
| 9.1.2 | 2024-01-30 | Stable (patch) | Performance optimizations | folded into v9.1 |
| 9.1.1 | 2023-12-05 | Stable (patch) | After Effects export bumped to AE 24.1 stable | folded into v9.1 |
| 9.1.0 | 2023-11-07 | Stable | SVG (vectorial) file import; After Effects interoperability; drag-and-drop overhaul across Assets/viewport/layer stack | [release-notes-painter-9.1.md](release-notes-painter-9.1.md) |
| 9.0.1 | 2023-09-19 | Stable (patch) | Fixes; baking-parameter reset defaults | folded into v9.0 |
| 9.0.0 | 2023-06-20 | Stable | **Paint along Path tool** (first version — later replaced by Filled Path in 11.0, then Ribbon in 11.1); base materials refresh | [release-notes-painter-9.0.md](release-notes-painter-9.0.md) |
| 8.3.1 | 2023-04-27 | Stable (patch) | Baking Mode polish; GLB (binary glTF) import support | folded into v8.3 |
| 8.3.0 | 2023-01-10 | Stable | **Dedicated Baking Mode (F8)** replacing the old inline "Bake Mesh Maps" dialog; USD import/export; new Python `baking` module | [release-notes-painter-8.3.md](release-notes-painter-8.3.md) |
| 8.2.0 | 2022-10-06 | Stable | Welcome screen + What's New panel; Save menu reorganized; blending-mode/opacity copy-paste for layers | [release-notes-painter-8.2.md](release-notes-painter-8.2.md) |
| 8.1.3 | 2022-08-25 | Stable (patch) | Bugfix release | folded into v8.1 |
| 8.1.2 | 2022-07-19 | Stable (patch) | Auto Unwrap organic-mesh segmentation option | folded into v8.1 |
| 8.1.1 | 2022-06-28 | Stable (patch) | Hotfix | folded into v8.1 |
| 8.1.0 | 2022-06-07 | Stable | **ICC profile support / Adobe Color Engine (ACE)** introduced alongside Legacy color management; new **Height, Bent Normals, Opacity** bakers (native, replacing manual workarounds) | [release-notes-painter-8.1.md](release-notes-painter-8.1.md) |
| 8.0.1 | 2022-04-11 | Stable (patch) | SpaceMouse 2D Viewport support; fixes | folded into v8.0 |
| 8.0.0 | 2022-03-08 | Stable | 3DConnexion SpaceMouse 3D navigation; expanded OpenColorIO (OCIO) Color Management across Properties/viewports/color picker | [release-notes-painter-8.0.md](release-notes-painter-8.0.md) |

### Historical context (pre-8.0, out of deep-research scope)
Not covered by dedicated files — mentioned here only because they're commonly asked about:
- **"Substance Painter" (Allegorithmic) → "Adobe Substance 3D Painter" rebrand:** happened in **version 7.2.0 (June 23, 2021)** per Adobe's official all-changes log — new name, icons, executable/package names, and a standalone "Substance edition" concept were introduced then, well before the 8.x line covered above.
- **Metal/Roughness becoming the default PBR workflow** (vs. the older Specular/Glossiness path) predates the 8.x–12.x window covered here by several years; by the time of 8.0.0 (2022) MetalRough/ASM was already the long-standing default. Not independently re-verified in this research pass — flag as **background knowledge, not confirmed against a specific dated source in this pass**.
- **OpenColorIO (OCIO) color management** was first introduced in **7.4.0 (November 24, 2021)**; 8.0.0 and 8.1.0 (covered above) then expanded and layered ICC/Adobe Color Engine support on top of it.

## Related Apps (out of this skill's direct scope, but adjacent)
- **Substance 3D Designer** — node-graph authoring tool for the `.sbsar` materials/generators Painter consumes. Not covered in depth here; a separate skill would be needed for Designer-graph-authoring questions.
- **Substance 3D Sampler** — photogrammetry/scan-to-material tool, produces materials importable into Painter. Not covered in depth here.

## URL Patterns for Auto-Update
- Painter release notes: `https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/release-notes`
- Painter beta release notes: `https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/beta` (note: as of this check, this page only reflects the *current* beta state relative to the latest stable — it does not retain a history of past betas, so past-beta research has to go through search engines / Adobe Community announcements instead)
- Painter "All Changes" changelog (best single source — full per-version Added/Fixed history in one page): `https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes`
- Individual version pages follow the pattern `https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/version-<major>-<minor>` (e.g. `version-12-1`, `version-12-0`) — more detailed than the all-changes entry for that version, worth fetching directly when researching one specific release
- Python API changelog (fetch is slow/times out on the full page — expect to need retries or to rely on the per-version Python bullets inside the all-changes page instead): `https://helpx.adobe.com/substance-3d-painter-python/api/changelog.html`
- Adobe Substance 3D blog (feature announcements, less granular than release notes): `https://blog.adobe.com/en/publish/`
- Adobe Community announcements (semi-official; useful for beta-era details and staff commentary not in the formal release notes): `https://community.adobe.com/announcements-57/`

## Auto-Changelog Rule (Mode 0 — Version Check)

See `SKILL.md` for the full trigger/steps. Summary: if `last_checked` is more than 7 days old at the start of a consultation, fetch the URLs above, diff against the Known Versions table, and if a new version is found, create/update a `references/release-notes-painter-<version>.md` file, then update this table and `last_checked`.
