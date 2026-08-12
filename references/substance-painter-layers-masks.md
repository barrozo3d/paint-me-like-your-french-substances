# Layers, Masks & Smart Materials

## Layer Stack Fundamentals
- The Layers panel is a top-down stack per **Texture Set** (one stack per material/UDIM tile group, unless "Share layer stack across Texture Sets" is on).
- Two base layer types: **Fill Layer** (flat/procedural fill across every channel at once) and **Paint Layer** (raster strokes painted by hand, one bitmap per enabled channel).
- Layers composite top-to-bottom like Photoshop: top layer's mask/opacity/blend mode determines how much of the layers below shows through.
- **Folders/Groups** hold multiple layers and can carry their own mask — masking a group masks everything inside it at once without touching per-layer masks.
- **Instances** (Alt-drag a layer, or right-click → Instantiate) share the same content across texture sets/projects; editing one edits all instances. Useful for trims/decals reused across a hard-surface kit.

## Masks
- Every layer/folder can have a **black & white mask** (white = visible, black = hidden) plus **stacked mask effects** (Generators, Levels, Blur, Anchor Points) layered on top of the base mask paint.
- **Generators** (in the mask stack) auto-populate the mask from mesh data: `AO`, `Curvature`, `Position`, `Dirt`, `Edge Wear`, `Metal Edge Wear`, `Mask Editor` (combines multiple bakers with sliders). This is how "grime in the crevices" or "wear on the edges" masks get built without manual painting.
- Paint directly onto a mask (select the mask thumbnail, paint in black/white/grey) for hand-authored control layered on top of a generator.
- **Levels** and **Blur** mask effects (right-click mask → Add Effect) refine a generator's output the same way Photoshop Levels/Gaussian Blur would.

## Anchor Points
- An **Anchor Point** tags a specific layer/mask's output so any *later* layer can reference it as an input via the **Anchor Point** generator/filter, without duplicating the mask.
- Common use: bake a single "cavity + edge wear" combo mask once, anchor it, then reference that anchor from multiple fill layers above (scratches, dust, extra roughness) so they all stay in sync if the source mask changes.
- Anchor points only see layers *below* them in the stack at the time of evaluation — order matters.

## Smart Materials & Smart Masks
- A **Smart Material** is a saved combination of multiple fill layers + generator-driven masks (e.g. "worn painted metal") that adapts to the mesh it's dropped on, because its masks reference bake data (AO/curvature/position) rather than fixed pixel coordinates.
- A **Smart Mask** is the mask-only version — a saved generator/effect stack you drop onto an existing layer's mask, instead of a full material.
- Both live in the Shelf (`Assets → smart materials` / `smart masks`) and can be authored by building the effect once and right-clicking → "Create Smart Material/Mask".
- Smart materials depend on the mesh having valid bakes (AO/curvature/position at minimum) — a mesh baked with bad UVs or missing cage data will make a smart material look wrong even though the material itself is unchanged.

## Blend Modes & Opacity
- Standard Photoshop-style blend modes (Normal, Multiply, Add, Overlay, etc.) apply per-layer, and can be set **per-channel** (a layer can Multiply on Roughness while staying Normal on BaseColor) via the channel-specific blending icons next to each enabled channel.
- Layer **opacity** is a single slider that scales the whole layer's contribution uniformly, independent of the mask.

## Common Gotchas
- A fill layer with no channels enabled paints nothing — enable each channel it should affect (BaseColor, Roughness, Height, etc.) via the small channel icons in the layer row.
- Mask generators require bakes to exist first (Mode 1's "run baking before masks that use AO/curvature/position" rule) — an ungenerated bake shows a flat/grey result in the generator preview.
- Group opacity and per-layer opacity both multiply — a 50% group containing a 50% layer renders at 25% effective opacity.
