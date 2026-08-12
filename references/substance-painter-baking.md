# Baking (Mesh Maps)

## What Baking Does
Baking pre-computes per-pixel mesh data into textures ("mesh maps") that painting, generators, and masks read from. It happens once per Texture Set (or per UDIM tile) before serious mask/material work — most Smart Materials look wrong or flat until real bakes replace the placeholder data.

## Core Mesh Maps
| Map | What it encodes | Typical use |
|---|---|---|
| Ambient Occlusion | Contact/crevice darkening from the low-poly's own geometry | Grime/dirt masks, base shading |
| Curvature | Convex (edges) vs. concave (crevices) — signed, centered grey | Edge-wear and crevice-dirt masks |
| Normal (World Space) | Absolute surface direction in world space | Tri-planar projection, some generators |
| Normal (Tangent Space, from high poly) | High-to-low detail transfer — THE bake for hard-surface/organic detail | Baked into the final Normal channel output directly |
| Position | XYZ world position encoded as RGB | Height-band masks (e.g. "grime only near the ground"), the Position generator |
| Thickness | Approximate mesh thickness via inverted-normal ray casts | Subsurface/translucency masks, edge-highlight variants |
| ID (Material/Color ID) | Flat color-per-shell or per-material from the high poly or a dedicated ID mesh | Fast "select this shell" masking via the Color Selection generator |

## High-to-Low Poly Workflow
- Bakes transfer detail from a **high-poly** (or a separate high-poly-per-part set) onto the **low-poly**'s UVs, using ray casting along each low-poly vertex normal (or a **cage**).
- A **cage** is an offset shell around the low-poly that constrains the ray-cast search distance/direction — needed when parts are close together and default ray casting picks up the wrong high-poly surface ("bleeding"/misprojection between separate parts).
- **Max Frontal/Rear Distance** parameters bound how far the ray search reaches; too large picks up unrelated geometry, too small misses valid detail.
- **Match by Mesh Name** or **Match by ID** (bake settings) control how multiple high/low poly pairs get associated when baking several parts of one asset at once — mismatched naming is the most common cause of a bake picking the wrong high-poly source for a given low-poly shell.

## UDIMs & Multiple Texture Sets
- A mesh with multiple UDIM tiles or multiple materials becomes multiple **Texture Sets**, each baked (and painted) somewhat independently, though "Share layer stack across Texture Sets" can unify the layer stack while keeping bakes per-set.
- Bake **all** Texture Sets before starting mask work project-wide — a smart material dropped on a not-yet-baked tile will look broken until that tile's own bake completes.

## Common Gotchas
- A model with no UVs, overlapping UVs, or UDIM-tile-crossing UVs will bake incorrectly or refuse to bake — fix UVs before baking, not after.
- "By mesh name" bakes require the high-poly and low-poly objects to share matching names (often with a `_low`/`_high` suffix convention) — mismatches silently produce wrong or empty bakes for that shell.
- Baking is CPU/GPU-intensive; the in-app baker (default) is slower but simpler than exporting to an external baker (Marmoset, xNormal) — use the in-app baker unless there's a specific quality/speed reason not to.
- A visibly "grainy" AO or thickness bake usually means the sample count is too low — raise antialiasing/samples in the bake settings rather than trying to fix it in the mask stack.
