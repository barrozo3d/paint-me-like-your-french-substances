# Substance 3D Painter 12.1 Beta ("Skew & OpenPBR" open beta) — Release Notes

**Released:** Announced ~April 7, 2026 (unverified — secondary source only, see note below), preceding the 12.1.0 stable release of June 23, 2026
**Type:** Beta (open beta, pre-release of 12.1.0)

## Added
- Early access to the same feature set that shipped stable in 12.1.0: Skew Baking/Painting (with Edge Protection helper), Auto-Rebaking, initial **OpenPBR** material-standard support with new channels/shader, and the **Hard-Surface Auto Unwrap** mode
- Bug reports collected via a dedicated Discord channel and the in-app crash-report window

## Breaking Changes & Migration Notes
- **What breaks:** Adobe explicitly warned that the beta **changes the project save format** in a way that is **not compatible with 12.0** — a project saved in the beta cannot be reliably reopened in 12.0.x, and the beta was not recommended for production work.
  **Workaround:** Keep separate backups of any project before opening it in a beta build; do not treat beta-era save files as safe to hand off to a 12.0.x-only collaborator. This concern is now moot once both sides are on 12.1.0+ stable, since the beta's format became the shipped 12.1.0 format.
- **What breaks:** A tutorial recorded during this open beta (roughly April–June 2026) may show UI or default behavior that shifted slightly before the final 12.1.0 stable release (betas commonly get last-minute UI polish).
  **Workaround:** Prefer treating any beta-era screen recording as "directionally correct for 12.1.0+" rather than pixel-exact; verify specific menu wording against the shipped 12.1.0 release notes.

## Known Issues
- General beta-quality caveat from Adobe: not recommended for production; expect instability

## Sources
- https://community.adobe.com/announcements-57/substance-painter-2026-skew-openpbr-beta-1556690 (Adobe Community announcement — official Adobe channel, but the exact April 7, 2026 date was extracted via automated page summarization and was not independently cross-checked against the official beta release-notes page, which at time of research only reflected the current/latest beta state rather than historical beta dates. Treat the exact date as **unverified — secondary source only**; the feature set and the 12.0-incompatibility warning are confirmed.)
