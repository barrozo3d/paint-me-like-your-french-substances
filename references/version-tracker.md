# Version Tracker

Tracks the current known version of Adobe Substance 3D Painter and when this file was last checked against Adobe's release-notes pages. Mirrors the Auto-Changelog Rule in `SKILL.md` (Mode 0).

- **last_checked:** 2026-08-12

## Known Versions (as of last_checked)

| App | Latest stable | Notes |
|---|---|---|
| Substance 3D Painter | 12.1 (released 2026-06-22) | Reworked baking workflow (continuous rebaking, on-mesh skew-correction painting, edge protection, redesigned mesh map list), **OpenPBR** shading model now supported and set as the default workflow (see `substance-painter-shaders-channels.md`), new hard-surface automatic UV-unwrapping mode. Raises minimum macOS to 13.0 (Ventura). Previous release: 12.0 (2026-03-09) — texture flattening directly in the layer stack, automatic warp-projection mode, revamped post-processing effects, improved project creation/settings workflow. |

## Related Apps (out of this skill's direct scope, but adjacent)
- **Substance 3D Designer** — node-graph authoring tool for the `.sbsar` materials/generators Painter consumes. Not covered in depth here; a separate skill would be needed for Designer-graph-authoring questions.
- **Substance 3D Sampler** — photogrammetry/scan-to-material tool, produces materials importable into Painter. Not covered in depth here.

## URL Patterns for Auto-Update
- Painter release notes: `https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/release-notes`
- Painter beta release notes: `https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/beta`
- Painter "All Changes" changelog: `https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/release-notes/all-changes`
- Adobe Substance 3D blog (feature announcements, less granular than release notes): `https://blog.adobe.com/en/publish/`

## Auto-Changelog Rule (Mode 0 — Version Check)

See `SKILL.md` for the full trigger/steps. Summary: if `last_checked` is more than 7 days old at the start of a consultation, fetch the URLs above, diff against the Known Versions table, and if a new version is found, create/update a `references/release-notes-painter-<version>.md` file, then update this table and `last_checked`.
