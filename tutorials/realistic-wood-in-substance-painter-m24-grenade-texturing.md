---
title: Realistic Wood in Substance Painter | M24 Grenade Texturing
source: YouTube
url: https://www.youtube.com/watch?v=I3v-ESX4DxQ
author: Dolinskyi
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not specified (modern UI, consistent with this creator's other M24 Grenade series videos)"
tags: [layers, fill-layer, masks, generator, anchor-point, blend-mode, ambient-occlusion, procedural, alpha, stencil, basecolor, roughness, height, metal-rough, color-management, advanced]
extraction_status: complete
frames_dir: tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/
frame_count: 13
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Realistic Wood in Substance Painter | M24 Grenade Texturing

**Source:** [YouTube](https://www.youtube.com/watch?v=I3v-ESX4DxQ)
**Author:** Dolinskyi
**Duration:** 17m55s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hello and welcome to the channel!
[0:02] Today we are going to texture wood step by step using a metal roughness workflow, using the handle of an M24 grenade as an example.
[0:10] In the next video, we will go through the rest of the grenade and after that I will upload this project so you will be able to explore every layer in detail.
[0:18] Make sure to subscribe so you don't miss it. Let's get started.
[0:22] I collected a few interesting photos of wood. If you analyze the texture, you can roughly divide it into three tones, dark, mid and light.
[0:30] Dark tones usually appear in joints or as spots on the surface. Mid tones are the base color of the wood.
[0:37] Light tones appear in damaged areas like cracks and worn parts.
[0:42] Let's start with the base wood. First we set up the mid tones and then we build everything on top of that.
[0:48] For this we need a texture. You can download one from textures.com or any other resource you prefer.
[0:54] Create a fill layer and plug this texture into color.
[0:58] Adjust the wood grain direction the way you like and add an anchor point.
[1:02] Then create another layer, call it wood material and insert a fill layer into it.
[1:08] Add the anchor point from the previous layer.
[1:13] Set metalness to black because this is not metal.
[1:17] Add a filter layer with color correction.
[1:21] Here we will adjust the base color of the wood.
[1:25] Tune it based on your references and your taste.
[1:29] Then create another fill layer and call it roughness.
[1:34] In the roughness channel, use information from the base layer but switch the reference channel to base color.
[1:42] So we take color data and use it as roughness.
[1:46] Use levels to increase contrast and make it more matte. Wood should not be shiny.
[1:58] This is our base material.
[2:03] Create a layer called height. Again, we take base color and use it as a height map.
[2:09] Adjust micro details to make the surface feel more natural.
[2:13] Sometimes I go back and tweak previous layers. It's normal if it doesn't look perfect right away.
[2:19] Now let's add color variation.
[2:23] Create a new layer. Use anchor point and color.
[2:28] Slightly adjust roughness and add HSL to shift the color.
[2:41] Add a mask with a grunge texture.
[2:45] This creates subtle color variation.
[2:49] Duplicate the layer, change the color and use a different grunge.
[2:53] This helps break the uniform look. Wood in real life is never perfectly even.
[3:09] Keep the variation subtle.
[3:13] Now let's enhance the grain using anchor data.
[3:17] Increase mask contrast and emphasize the fibers.
[3:25] Next, adjust roughness variation across layers.
[3:29] I'm setting up roughness variations across these three channels.
[3:33] You can experiment with different blending modes, opacity levels or anything that makes the roughness more interesting.
[3:37] And again, we can add a layer to the roughness.
[3:41] Create a new layer.
[3:45] Add anchor point to color and darken it using HSL or color correction.
[3:49] Add a layer to the roughness.
[3:53] Add a layer to the roughness.
[3:57] Add a layer to the roughness.
[4:01] Add a layer to the roughness.
[4:05] Add a layer to the roughness.
[4:09] Add a layer to the roughness.
[4:13] Add a layer to the roughness.
[4:17] Add a layer to the roughness.
[4:21] I add a dirt generator into the mask.
[4:25] I want to remove the dark tone from chipped and damaged areas.
[4:29] These damages were created in Z brush on the high poly, so they were baked into the ambient occlusion.
[4:33] Which the dirt generator uses.
[4:37] I add an anchor point on top so I can use this information in the next stages of the workflow.
[4:41] One is placed above the dirt and another above all layers.
[4:45] Next, I want to remove the micro detail from dark tones.
[4:49] I switch the height map blending mode to normal and set pass through on its folder.
[4:53] Then tweak the slider.
[4:57] The next step is to change the color of the layer.
[5:01] I'm going to change the color of the layer.
[5:05] Then tweak the slider. The darker areas will appear smoother compared to the lighter ones.
[5:09] Make dark areas slightly glossy.
[5:13] Like lacquer. This adds variation to glossiness.
[5:17] In some areas the surface will be matte in others glossy.
[5:21] This adds interest to the texture. Just like light and dark tones,
[5:25] the variation between matte and glossy gives the material a more appealing look.
[5:29] Next, I want to make dark variation from base texture.
[5:33] It brings more depth.
[5:37] I start by setting up a very dark color.
[5:41] Then I add a mask to this layer and insert an anchor from the base layer.
[5:45] I add a layer of dark color.
[5:49] I add a layer of dark color.
[5:53] Then I add a layer of dark color.
[5:57] I make the mask more contrasty
[6:01] and invert it.
[6:05] Add another fill layer and insert the mask from the previous layer into it.
[6:09] I want to exclude these dark tones from the damaged areas.
[6:13] I add another layer.
[6:17] These will also be dark variations.
[6:21] I add another layer. These will also be dark variations.
[6:25] I change the blending mode to overlay.
[6:29] I add a mask, then a fill layer into the mask
[6:33] and insert this kind of grunge texture.
[6:37] I add another layer.
[6:41] I add another layer.
[6:45] I add another layer.
[6:49] I add another layer.
[6:53] I add another layer.
[6:57] I add another layer.
[7:01] I add another layer.
[7:05] I add another layer.
[7:09] Next layer will add dark spots and imperfections.
[7:13] I add another layer.
[7:17] I add another layer.
[7:21] I add another layer.
[7:25] Better to use custom stencils, but in this tutorial I intentionally want to use only
[7:53] standard tools.
[8:23] Next we add light tones. As you remember, light tones represent our damage. I follow the same principle as with the previous layers. I add color information from the anchor point, insert a color correct and shift the wood color to a very light tone. Raw wood is very matte, meaning it will appear the brightest in roughness.
[8:53] I use a standard wood texture from Substance Painter as a stencil. Increase the contrast to achieve a familiar wood damage pattern to convey the wood grain. This is a bit of meticulous manual work. The main thing is not to overdo it. Sometimes less is more.
[9:23] So I add it along the edges, and also somewhere in the middle of the object, as if it fell or was hit and fresh wood was revealed.
[9:49] If you have good custom stencils, use them. Again, I'm intentionally using only standard Substance Painter tools.
[10:20] I also add slight wear.
[10:22] Next, in the light tone folder I want to add wood fibers.
[10:52] I also add a procedural texture with almost straight lines into the mask. On top, I also insert a mask that subtracts everything except the damaged areas.
[11:19] I want to make them slightly brighter and reduce saturation a bit so there is variation and the fibers are more visible.
[11:50] Next is dust. We'll add dust on top of the wood that has settled and hasn't been worn off.
[12:10] I add a grunge called Grunge Dusty into the mask.
[12:38] I clean up the tiling areas and remove more in the places where we hold it by hand.
[12:57] Another layer on top. I want to add slightly more defined spots.
[13:24] The dust is a bit too visible. If the style requires it, you can keep it, but I want to tone it down.
[13:37] I also want to exclude dust from damaged wood areas.
[13:54] On top of that, I add a layer with red paint, small subtle spots. I think it adds more interest to the texture. In general, you can add many things, stickers, decals, anything you find in references or come up with yourself.
[14:24] These kinds of things are probably best done with stencils. Just project the shapes you need onto the texture.
[14:51] Final layers. I apply sharpen on top to make the texture crisper and more realistic.
[15:02] I apply sharpen to both color and roughness. I switch it to pass through and right click Apply to all channels. By default, the value is quite high, so I reduce it.
[15:17] Too much sharpen looks noisy, so keep a balance.
[15:33] I notice something I really don't like. These fibers we added are too obvious. You can clearly see where they start and end. I want to break them up using grunge, making them less uniform.
[15:55] I'll experiment with different grunge textures. I want some areas to be stronger, others weaker, more realistic overall. The edge is too sharp, so I soften it with a brush.
[16:25] I also want to simplify the edge a bit. Remove some damage so some areas stay clean while others show wear, creating contrast.
[16:47] And the final layer is color correction. I want to tweak the overall color. Make it more saturated and more contrasty.
[16:58] I tweak the sliders, sometimes pushing them far left and right to find extremes, then settling on what I like. Small adjustments are sometimes hard to notice.
[17:26] Maybe brighten it a bit more.
[17:35] I think this is a good point to stop. This is a simple, but effective way to texture wood. Share your method in the comments or tell what can be done more better on this object.
[17:45] In the next video, we will make a painted metal for other parts of the grenade, then I share whole source files from the project. Thanks for watching and see you in the next video.



---

## Captured Frames

- [0:54] tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/frame_000.jpg
- [1:34] tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/frame_001.jpg
- [2:03] tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/frame_002.jpg
- [2:28] tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/frame_003.jpg
- [4:21] tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/frame_004.jpg
- [5:09] tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/frame_005.jpg
- [6:25] tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/frame_006.jpg
- [8:53] tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/frame_007.jpg
- [10:22] tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/frame_008.jpg
- [11:50] tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/frame_009.jpg
- [13:54] tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/frame_010.jpg
- [15:02] tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/frame_011.jpg
- [16:47] tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/frame_012.jpg

---

## Structured Notes

### Core Technique
Part 1 of the creator's M24 Grenade series (prequel to the already-ingested "Tempering Colors" and "Realistic Painted Metal" videos), texturing the wooden handle with a **dark/mid/light three-tone reference framework** (dark = joints/spots, mid = base wood color, light = damaged/worn/fresh-wood areas), where every subsequent layer group derives its mask from one shared **Anchor Point** captured off the base texture — the single throughline technique across the whole build.

### Summary
Starts from a downloaded tileable wood photo reference, analyzed into three tonal bands before touching Painter. **Base material**: a Fill layer with the wood photo plugged into BaseColor, grain direction adjusted, then an **Anchor Point** added on top of it. A separate "wood material" group's Fill layer references that anchor for Metallic (set to black/0), with a Color Correct filter above it for base-color tuning from references. Roughness is built by taking the *same* base Fill layer's data but switching its **Reference Channel to Base Color** (i.e. reusing color information as roughness input) then increasing contrast with Levels to push it matte (wood should not read shiny). Height is built the same way — reusing Base Color as the height source — with Micro Details tuned afterward for a more natural surface. **Color/roughness variation**: a new layer referencing the base anchor for color, slight roughness adjustment, then an **HSL** filter to shift hue, masked by a grunge texture for subtle color variation; duplicated with a different color and different grunge to avoid a uniform look ("wood in real life is never perfectly even"), kept deliberately subtle. Grain is reinforced by increasing mask contrast on anchor-referenced layers to emphasize fibers, and roughness variation is layered similarly across multiple channels with experimentation in blend modes/opacity. **Removing dark tone from damage**: since the model's chips/damage were sculpted in ZBrush and baked into the mesh's Ambient Occlusion map, a **Dirt generator** (AO-driven) is added to a mask specifically to *remove* the dark-tone treatment from those already-damaged areas (so damage doesn't get double-darkened) — the resulting mask is itself captured as two more Anchor Points (one directly above the Dirt layer, one above the entire stack) for reuse in later stages. The Height channel's blend mode is switched from its default additive mode to **Normal** (with the containing folder set to Pass Through) specifically to *remove* micro-surface detail from dark tones, since darker wood areas should read visually smoother/glossier than lighter ones — like a lacquer coating — adding a matte/glossy variation dimension on top of the light/dark color variation. **Dark variation from base texture** (added depth): a very dark color Fill layer masked by the base anchor, contrast-increased and inverted, with the resulting mask itself reused (inserted into another Fill layer) so dark tones are excluded from the damaged areas; further dark-spot/imperfection layers are stacked with **Overlay** blend mode and grunge-texture masks, deliberately using only Painter's stock grunge/stencil library rather than custom stencils (explicitly called out as an artificial constraint for the tutorial). **Light tones (damage)**: following the same anchor-plus-Color-Correct pattern, shifted to a very light/matte wood tone (raw exposed wood is the brightest in Roughness); masked using Painter's **stock wood texture as a stencil**, contrast-increased to get a recognizable worn-grain damage pattern, placed by hand along edges and at plausible impact points ("as if it fell or was hit and fresh wood was revealed") — deliberately restrained ("less is more"). A **wood fibers** sub-layer inside the light-tone folder uses a near-straight-line procedural mask, subtractively masked to only the damaged areas, brightened and desaturated slightly for visibility. **Dust**: a `Grunge Dusty` mask for settled dust, cleaned up around tiling seams and hand-grip contact areas (where dust would be worn off by handling), a second layer for more defined dust spots, toned down and excluded from already-damaged wood. **Extra detail**: a subtle red-paint-spot layer for visual interest, plus (visible in the captured frames though only briefly implied in narration — "stickers, decals, anything you find in references") a stenciled "1939" date stamp and small crest/icon stamp burned into the wood, explicitly recommended to place via stencils. **Finishing**: a **Sharpen** filter applied to both Color and Roughness channels via Pass Through + right-click **Apply to all channels**, default strength reduced (too much sharpen reads as noise); a self-critique pass revisiting the wood-fiber layer because its start/end points read too obviously artificial — broken up further with additional grunge variation and a hand-brushed soft edge; damage simplified in some areas to create contrast between clean and worn zones; and a final top-of-stack **Color Correct** for overall saturation/contrast, arrived at by pushing sliders to extremes first to find the range before settling on a value.

### Key Steps
1. Gather wood photo references and mentally sort the look into three tonal bands: dark (joints/spots), mid (base color), light (damage/wear/fresh wood) — plan the whole layer structure around this before starting.
2. Base material: Fill layer with a tileable wood photo in BaseColor, grain direction adjusted to the mesh, then add an **Anchor Point** on top of this layer.
3. In a separate "wood material" group, reference that anchor for Metallic (set to 0/black — wood isn't metal) and add a **Color Correct** filter above for base-color tuning against references.
4. Build Roughness by reusing the base layer's data with its **Reference Channel switched to Base Color** (color data reused as roughness input), then Levels to raise contrast/push it matte.
5. Build Height the same way — Base Color reused as the height source — then tune Micro Details for a more natural surface read.
6. Add color/roughness variation: new anchor-referenced layer, slight roughness tweak, **HSL** to shift hue, masked by a grunge texture; duplicate with a different color and different grunge for non-uniformity.
7. Reinforce grain by increasing mask contrast on anchor-referenced layers to emphasize fiber definition; layer additional roughness variation across channels, experimenting with blend modes/opacity.
8. Add a **Dirt generator** (AO-driven — reads baked-in ZBrush sculpted damage) specifically to *remove* dark-tone treatment from already-damaged areas so damage doesn't get double-darkened; capture the resulting mask as two more **Anchor Points** (one directly above Dirt, one above the whole stack) for reuse downstream.
9. Switch the Height channel's blend mode to **Normal** (folder set to Pass Through) to *remove* micro surface detail specifically from dark tones — darker wood should read smoother/glossier (like lacquer) than lighter, rougher areas, adding a matte/glossy dimension layered on top of the color variation.
10. Add "dark variation from base texture" depth: a very dark Fill layer masked by the base anchor, contrast-increased and inverted, its resulting mask reused in a further layer to exclude dark tones from damaged areas; stack additional dark-spot/imperfection layers on **Overlay** blend mode with grunge masks — deliberately restricted to Painter's stock grunge/stencil library only (no custom stencils, as a tutorial constraint).
11. Build light tones (damage): anchor + Color Correct shifted to a very light, matte wood tone (raw exposed wood reads brightest in Roughness); mask with Painter's **stock wood texture used as a stencil**, contrast-boosted for a recognizable worn-grain pattern, hand-placed along edges and at plausible impact points — kept restrained.
12. Add a **wood fibers** sub-layer (near-straight-line procedural mask) inside the light-tone folder, subtractively masked to only the damaged areas, slightly brightened/desaturated for visibility.
13. Add **dust**: `Grunge Dusty` mask, cleaned around tiling seams and hand-contact areas (dust worn off by handling); a second more-defined-spots dust layer, toned down and excluded from damaged wood.
14. Add small interest details: a subtle red-paint-spot layer, plus stenciled decals/stamps (a date-stamp number and small crest icon observed in the captured frames) — recommends stencils for this kind of precise placed detail.
15. Finish with **Sharpen** on both Color and Roughness (Pass Through + right-click **Apply to all channels**), default strength reduced to avoid a noisy look.
16. Self-critique pass: identify a too-obviously-artificial-looking layer (the wood fiber lines had visible start/end points), break it up further with additional grunge variation and a hand-brushed soft edge; simplify/remove some damage in places to create clean-vs-worn contrast.
17. Close with a top-of-stack **Color Correct** for overall saturation/contrast — push sliders to extremes first to understand the range, then settle on a balanced value.

### Layers / Tools / Settings
- `Anchor Point` (captured off the base texture layer; reused across nearly every subsequent group — color variation, dirt-generator-derived damage mask ×2, dark-variation exclusion mask)
- Reference Channel trick: Fill layer's Roughness/Height driven by reading its own **Base Color** data instead of a dedicated grayscale texture
- `Dirt` generator (Ambient-Occlusion-driven, reused here to *remove* dark tone from ZBrush-sculpted/baked damage areas, not to add dirt)
- Height-channel blend mode switched to `Normal` (folder `Pass Through`) to selectively strip micro-detail from dark tones for a smoother/glossier look
- `HSL`, `Color Correct` / `Levels` filters (color/roughness tuning and mask-contrast control throughout)
- Blend modes: `Overlay` (dark spots), standard subtract-style masking (excluding damaged areas from various effects)
- Painter's stock **wood texture used as a stencil** for light-tone damage patterning (explicitly not a custom stencil, by design)
- Procedural near-straight-line texture (wood fibers mask)
- `Grunge Dusty` (dust)
- `Sharpen` filter, Pass Through + **Apply to all channels**

### Difficulty
Advanced — the anchor-point-as-shared-foundation architecture (nearly every group in the stack ultimately derives from one base anchor) and the Reference-Channel color-as-roughness/height trick are non-obvious, efficient techniques beyond basic layer/mask work.

### App & Version
Not stated on screen; UI consistent with this creator's other ingested M24 Grenade series videos (modern, post-8.3-era baking-mode UI).

### Tags
`layers` `fill-layer` `masks` `generator` `anchor-point` `blend-mode` `ambient-occlusion` `procedural` `alpha` `stencil` `basecolor` `roughness` `height` `metal-rough` `color-management` `advanced`

---

## Related Tutorials
- [Tempering Colors in Substance Painter | Steel Heat Effects](tempering-colors-in-substance-painter-steel-heat-effects.md) — same creator (Dolinskyi), same M24 Grenade project series; this is the prequel video (Part 1: wood handle) to that steel-heat-effects video's metal parts.
- [Realistic Painted Metal in Substance Painter | M24 Grenade Texturing](realistic-painted-metal-in-substance-painter-m24-grenade-texturing.md) — same creator, same project series (Part 2 of the grenade, per this video's own closing statement: "next video, we will make a painted metal for other parts of the grenade"); shares the anchor-point-driven layer architecture and stock-grunge/stencil-only constraint.
- [Powerful Substance Painter Tricks That You Need To Know](powerful-substance-painter-tricks-that-you-need-to-know.md) — same creator; shares the Anchor-Point-as-reusable-mask-source philosophy this video builds its entire layer stack around, applied there to a weld-seam heat-tint effect instead of wood tonal variation.
