# Foundations — PBR & Texturing Theory

## Physically Based Rendering, in brief
PBR shading models (metal/rough and specular/glossiness alike) aim to keep material response energy-conserving and physically plausible across arbitrary lighting, instead of hand-faking highlights per-scene like older Phong/Blinn workflows. Practically, this means: BaseColor should hold *only* the material's intrinsic reflectance (no baked shadows, no baked specular highlights, no baked ambient occlusion in the color itself for a fully PBR-correct asset), because AO/shadow/highlight are the renderer's job once real lighting is applied.

## Color Space Discipline
- **sRGB (gamma-encoded):** used for anything perceived directly as color — BaseColor/Albedo, Emissive. Textures painted or imported as color images assume sRGB by default.
- **Linear (raw/non-color):** used for anything that's actually a physical value being read by math, not perceived as color — Roughness, Metallic, Height, AO, Normal maps. Importing a linear-data map (e.g. a roughness mask) through an sRGB import setting double-encodes it and skews the math.
- Getting this wrong is the most common invisible bug in a texturing pipeline — the image can *look* plausible in Painter's viewport and still be numerically wrong once it hits a strict engine renderer.

## UVs & Texel Density
- **Texel density** (pixels-per-unit of UV-mapped surface) should stay consistent across an asset's shells unless a deliberate detail budget dictates otherwise (e.g. a hero character's face gets more texel density than the sole of a boot) — inconsistent texel density is visible as some surfaces looking noticeably blurrier/sharper than neighboring ones at the same camera distance.
- **UV seams** are where texture-space discontinuities live; Painter's projection/painting tools (especially the 3D viewport paint) mostly hide seams during authoring, but seams still show under close inspection if normal-map detail or a hand-painted stroke crosses one without matching on both sides.
- **Overlapping UVs** intentionally reuse UV space (common for tileable/repeated trims) — Painter paints onto all overlapping shells simultaneously in 3D-viewport mode, which is usually the desired trim-sheet behavior but can surprise a modeler who didn't expect a single stroke to hit multiple mesh islands at once.

## Procedural Materials & Generators
- Most of Painter's built-in "smart" behavior (Smart Materials/Masks, mask Generators) is powered by parametric **Substance** materials/filters (`.sbsar` — compiled Substance Designer graphs) rather than fixed bitmaps, which is why they adapt to a new mesh's bake data instead of looking pasted-on.
- A `.sbsar` exposes a fixed set of author-defined parameters (scale, contrast, color variation, etc.) in Painter's Properties panel — the underlying graph logic isn't editable inside Painter itself; deeper changes require Substance 3D Designer (a separate, related Adobe app, out of this skill's direct scope but worth knowing it's where custom `.sbsar` generators/materials are authored).

## Painting-Specific Considerations
- **Tri-planar projection** paints/generates by blending three world-axis-aligned projections (X/Y/Z), avoiding UV-seam artifacts for materials without clean UVs (or none at all) — common for quick environment blockouts or terrain-like surfaces, at the cost of visible blending seams on diagonal surfaces if projection settings aren't tuned.
- **Stencils** project a 2D image/alpha through the viewport camera onto the 3D mesh at a fixed screen position, useful for decals/logos/graphic damage that needs to read correctly from a specific angle rather than following the mesh's own UV layout.
