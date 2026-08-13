---
title: Advanced Peeling Paint Effect in Substance 3D Painter
source: YouTube
url: https://www.youtube.com/watch?v=VE8aILV053Y
author: Javad Rajabzade
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated on screen; UDIM workflow explicitly mentioned (multi-tile projection handling required) and modern generator/anchor-point UI, consistent with recent versions, tentative"
tags: [layers, fill-layer, paint-layer, masks, generator, anchor-point, blend-mode, height, roughness, basecolor, alpha, procedural, udim, texture-set, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/advanced-peeling-paint-effect-in-substance-3d-painter/
frame_count: 10
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Advanced Peeling Paint Effect in Substance 3D Painter

**Source:** [YouTube](https://www.youtube.com/watch?v=VE8aILV053Y)
**Author:** Javad Rajabzade
**Duration:** 11m27s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hello everyone, this is Javad and today I'm going to show you how to create a peeling
[0:12] paint effect in Substance Painter.
[0:15] As you can see I'm already imported my model and baked the textures, so the model is ready
[0:22] to go.
[0:23] And let's get started.
[0:27] So in games and 3D props we usually deal with the three main types of paint damage,
[0:32] HVIR, peeling or police streaming, paint and cracking.
[0:37] HVIR is what you normally see on things like weapons or tools where the paint naturally
[0:44] drops around the edges.
[0:46] But in this video I want to focus more on the peeling paint and show you how to make
[0:51] a more advanced version of it in Substance Painter.
[0:56] If you're interested in learning more about all these types of paint damage, I actually
[1:01] wrote an article that explains each one in detail.
[1:06] You can check it out and download it from my Patreon.
[1:11] It will help you figure out which type of paint damage fits the best for your assets.
[1:20] Alright let's start by creating a new fill layer and adding a black mask.
[1:26] Next I'll apply a generator to control where the paint starts to peel off.
[1:32] Now depending on the look you want you can use different generators, for example the
[1:36] edge damage mask, builder or even curvature mask.
[1:39] Each of them gives you a slightly different result.
[1:43] So it really depends on your material and what kind of VIR effect you are going for.
[1:48] Here I'm using the Metal HVIR generator, I don't want any extra grunge in this case
[1:52] so I reduce the grunge amount and then increase both the VIR level and the contrast to make
[1:57] the effect a bit sharper.
[1:59] Okay now I'm going to add a blur filter and slightly increase its value.
[2:07] Then I'll change the blending mode to Lighten.
[2:12] What the Lighten mode does it keeps the maximum color value between the top and the bottom
[2:17] layer.
[2:18] In this case it means we are keeping our sharp edge VIR mask while blending the blur mask
[2:26] on top of it.
[2:27] We'll start with two values here.
[2:32] The first value is the sharp, completely white mask.
[2:36] This means that the paint will be fully removed in that area and we won't see any paint there
[2:42] at all.
[2:44] In other words that sharp white mask completely erase the paint.
[2:48] On the other hand the blurred mask or the softer edge will add a more gradual grunge
[2:54] effect creating a natural worn look.
[2:57] For adding edge damage I usually use a cell texture however in this case I'm using a 3D
[3:03] Perun effectal that gives me more control over the parameter.
[3:08] Also since we are working with UDIM we need to adjust the projection to feel.
[3:15] Next we'll adjust the 3D Perun effectal parameter until we achieve the desired look.
[3:26] After that we'll change the blending mode to Divide.
[3:31] The result you'll notice the effect primarily appears under softer blurry edges while the
[3:39] sharp white mask remain unchanged.
[3:42] Then I'm using a level to invert the mask.
[3:45] Next we'll add a histogram shift.
[3:48] What this does is shift any black values in the mask to white without altering other values.
[3:57] After that histogram shift we'll add another level and invert the mask to finalize it while
[4:04] we could use an invert filter.
[4:09] Invert filter actually doesn't offer as much control over the mask values by using the
[4:17] level we can fine tune the edges and get more precise results.
[4:22] The height value to bring out the age damage.
[4:25] This increase our height value to bring out the age damage effect.
[4:30] As you can see everything looks good and the age detail are no visible.
[4:35] The next step is to create our paint mask.
[4:37] To do that we'll add an anchor point between the level and the histogram shift.
[4:42] This will give us a mask that we can later on use to mask our paint layer.
[4:50] Now I'm going to add another layer.
[4:54] Place it inside the group.
[4:56] Let's rename this layer to paint layer.
[5:01] I pick a color and adjust roughness.
[5:10] Inside the group I'll add a black mask for paint layer.
[5:16] I'll reference it using the anchor point and apply a level adjustment.
[5:25] By tweaking the level we can control how and where the paint becomes visible.
[5:31] Now we can go back and use the belayer filter to either enhance or soften that age damage
[5:38] effect.
[5:39] Letting it gradually grow and blend more naturally.
[5:44] The cool thing about this setup is that by tweaking the parameters you can achieve a
[5:49] completely new look and effect on your material.
[5:52] As you can see I already inverted this 3D VOR effectal noise.
[6:00] That gives me this beautiful blistering effect.
[6:04] But the effect looks a bit too perfect to be realistic.
[6:09] So what I'm going to do is add a belayer filter on top of my layers.
[6:16] This is gonna be a solid effect but it gives a sort of erosion to this blistering effect
[6:23] and making the blistering look more natural and realistic.
[6:31] Let's duplicate our belayer filter using CTRL T and place it below the histogram shift.
[6:37] And by tweaking the parameter we can achieve more variation and enhance the overall effect.
[6:48] It actually doesn't look very natural when the paint damage shows up all over the entire
[6:52] model.
[6:53] In real life this kind of wear only happens in certain spots.
[6:58] So we need a way to control where it appears.
[7:02] So here is a cool trick.
[7:04] Add a paint layer and place it under the generator.
[7:09] Then switch the generator blending mode to multiple light.
[7:13] And now the magic happens.
[7:15] Whenever we paint on that layer, paint layer, it only reveals the edge wear effect exactly
[7:22] where we want.
[7:32] Okay, so here I'm adding another paint layer right above the metal edge wear generator.
[7:50] If I paint in black it will add the peeling paint effect to those areas.
[7:56] You can also press X to invert the mask.
[7:59] So painting in white will remove the effect from the spots that are already peeling.
[8:07] Okay here I want to add more details to my edge paint.
[8:10] So I'm creating an anchor point on top of my mask layer.
[8:16] Okay let's name it edge paint.
[8:19] And then I'll make a new layer with a black mask.
[8:27] And okay add a fill layer.
[8:32] And inside that fill layer I reference the anchor point.
[8:37] As you can see the mask shows up automatically because it's pulling the information from
[8:42] that anchor point.
[8:46] In a real world scenario the color on the edge of peeling paint usually fades a bit.
[8:52] So here I'm picking a slightly brighter color and setting blending mode to soft light.
[9:03] Okay let's duplicate this 2DVoronai fractal.
[9:09] And this time I'm switching to the regular 2DVoronai.
[9:12] I'm just going to grab the cell tiles preset and as you can see it gives me the sharp,
[9:19] cracking effect on the edges of my peeling paint.
[9:23] It's nice ways to break up the surface and make those edges feel more detailed.
[9:29] This kind of sharp cracking usually happens when the paint surface is constantly exposed
[9:34] to the sun.
[9:36] So if you are texturing a prop for an environment like a desert turn or somewhere with a really
[9:41] harsh sunlight, this type of cracking makes a lot of sense.
[9:46] It helps sell that dry sun beaten look.
[9:50] Before I even start texturing I always try to understand the story behind the asset.
[9:55] Like where is this thing actually sitting?
[9:58] What kind of place is it in?
[10:01] Has it been there for a few months or for decades?
[10:05] All those legal details actually decide how the surface should look.
[10:11] So it was thinking about them first.
[10:13] So for example if the asset is in a humid area, the type of damage you expect is totally
[10:19] different.
[10:20] In humidity you usually get moss slowly growing from the bottom up wart.
[10:25] And instead of this sharp cracking effect you'd probably go for a blistering effect
[10:32] because the humid environment traps moisture underneath the paint.
[10:37] But that trap butter pushes the paint out fart and creates those bubbles.
[10:43] So always think about the environment first.
[10:46] It makes your texture way more believable.
[10:48] To keep things organized I will place my mass layer inside this folder.
[10:52] My goal is to create a folder that contains my paint layer and any details I want to add
[10:58] will be created inside this folder.
[11:00] Anything placed underneath this folder will then be revealed as the underlying material.
[11:06] Then I'm going to drag and drop a metal rust material underneath my paint folder.
[11:11] As you'll notice here the height of the rust material is affecting the paint layer.
[11:15] So to fix that you're first going to change the channel from roughness to height and
[11:19] then we'll switch the blending mode from linear to normal.



---

## Captured Frames

- [1:20] tutorials/frames/advanced-peeling-paint-effect-in-substance-3d-painter/frame_000.jpg
- [1:59] tutorials/frames/advanced-peeling-paint-effect-in-substance-3d-painter/frame_001.jpg
- [2:57] tutorials/frames/advanced-peeling-paint-effect-in-substance-3d-painter/frame_002.jpg
- [3:42] tutorials/frames/advanced-peeling-paint-effect-in-substance-3d-painter/frame_003.jpg
- [4:37] tutorials/frames/advanced-peeling-paint-effect-in-substance-3d-painter/frame_004.jpg
- [6:09] tutorials/frames/advanced-peeling-paint-effect-in-substance-3d-painter/frame_005.jpg
- [7:02] tutorials/frames/advanced-peeling-paint-effect-in-substance-3d-painter/frame_006.jpg
- [8:07] tutorials/frames/advanced-peeling-paint-effect-in-substance-3d-painter/frame_007.jpg
- [9:03] tutorials/frames/advanced-peeling-paint-effect-in-substance-3d-painter/frame_008.jpg
- [11:06] tutorials/frames/advanced-peeling-paint-effect-in-substance-3d-painter/frame_009.jpg

---

## Structured Notes

### Core Technique
An advanced, fully-procedural peeling/blistering paint mask built by layering a sharp edge-wear generator with a 3D Voronoi-fractal-driven blurred variant (combined via `Lighten`/`Divide` blend-mode math, then `Levels` invert + `Histogram Shift` cleanup), converted into an anchor point so a separate paint-color layer, an edge-detail layer, and an underlying rust material can all reference the exact same mask shape — plus a manual-paint-driven "reveal window" trick (a black-mask paint layer set to `Multiply Light` under a generator) that confines otherwise-uniform procedural wear to only the areas the artist actually paints.

### Summary
Demonstrated on a pre-baked fire hydrant model (three real-world paint-damage categories named up front: edge wear/chipping, peeling/blistering, and cracking — this video focuses specifically on peeling). Builds the peel mask from a Metal Edge Wear generator (grunge amount reduced, wear level/contrast raised for a sharp result) blurred and blended with `Lighten` so the sharp mask stays intact while gaining a softer gradient halo; layers in a 3D Voronoi Fractal noise (chosen over a cell texture for finer parameter control; UDIM tile projection adjusted since the asset uses multiple UV tiles) combined via `Divide` so the noise only appears within the softer blurred-edge halo, not the sharp core; cleans the resulting mask with `Levels` invert -> `Histogram Shift` (pushes black values to white without touching the rest of the range) -> a second `Levels` invert (preferred over a plain Invert filter for finer edge control) -> a Height boost to physically raise the damage. That finished mask is captured as an **anchor point** placed between the Levels and Histogram Shift layers, then referenced by: a new paint-color layer (masked via the anchor point + a Levels adjustment to control paint coverage) inside the same group, an additional Bevel filter (used non-standardly, purely for its erosion-like distortion to break up the procedural mask's "too perfect" look — duplicated via Ctrl+T and placed at a second position in the stack for compounding variation), and later an "edge paint" detail pass (fresh anchor point + Fill layer referencing it, brighter color, `Soft Light` blend, plus a duplicated-and-reconfigured Voronoi — switched from 3D Fractal to a plain 2D Voronoi with a Cell-Tiles preset — for sharp sun-cracked-edge detail). A key spatial-control trick is introduced twice: (1) a black-mask Paint layer placed *under* the wear generator with the generator's own blend mode switched to `Multiply Light` so hand-painting only reveals the procedural wear where painted; (2) a second, simpler paint layer placed directly on the mask (paint black to add peeling, press `X` to invert the brush and paint white to remove it) for direct manual spot-control. Closes on process philosophy (always decide the asset's backstory/environment first — humid climates favor moss + blistering from trapped moisture, arid/sun-exposed environments favor sharp Voronoi cracking) and a folder-based organization pattern: group the paint layer + all its detail layers together, then drop supporting materials (a Metal Rust material) underneath the folder so they show through in the "revealed" areas — fixing an issue where the rust material's Height channel was bleeding into/deforming the paint layer by switching the affected channel from Roughness to Height and its blend mode from Linear to Normal.

### Key Steps
1. **Build the sharp edge-wear base mask:** add a new Fill layer, add a black mask, add a generator to it — Metal Edge Wear generator used here (Curvature or a plain Edge Damage mask/builder are named as valid alternatives depending on the desired look); reduce the generator's Grunge Amount, raise Wear Level and Wear Contrast for a sharp, clean result.
2. **Create a soft companion mask and combine with Lighten:** add a Blur filter on a copy/companion of the mask and slightly increase its value, then set that layer's blend mode to `Lighten` (keeps the maximum value between the sharp and blurred masks) so the sharp white core stays fully intact while gaining a soft gradient border — the sharp white area means "paint fully removed here," the blurred border means "gradual worn transition."
3. **Layer in 3D Voronoi Fractal noise for organic edge detail:** add a `3D Voronoi Fractal` (chosen over a 2D Cell texture for finer parameter control), adjust its projection to the correct **UDIM tile** since the asset spans multiple UV tiles, tune its parameters to taste, then set its blend mode to `Divide` — this makes the noise appear predominantly in the softer blurred-edge region while leaving the sharp white core unaffected.
4. **Clean up the combined mask with a Levels -> Histogram Shift -> Levels chain:** add a `Levels` filter and invert it; add a `Histogram Shift` filter (shifts black values toward white without disturbing the rest of the histogram); add a second `Levels` filter and invert again to finalize — explicitly preferred over a plain `Invert` filter because Levels gives finer control over exactly where the edge falls.
5. **Push the mask into visible surface Height** by raising the channel's Height value so the age/damage reads as physical relief, not just a flat color mask.
6. **Capture the finished mask as a reusable Anchor Point:** add the anchor point layer positioned specifically between the (second) Levels layer and the Histogram Shift layer in the stack, so downstream layers can reference this exact intermediate mask state.
7. **Build the paint-color layer from the anchor point:** add a new layer, place it inside the same group, rename it (e.g. "paint layer"), pick a paint color and adjust roughness, add a black mask, reference the earlier anchor point on that mask, then add a `Levels` adjustment on top to fine-tune exactly how much of the referenced mask becomes visible paint.
8. **Break up the mask's "too perfect" procedural look with a Bevel filter used for erosion, not bevelling:** add a Bevel filter on top of the layer stack purely for the organic distortion/erosion side-effect it produces on a mask, not for its literal bevel use case; duplicate it with Ctrl+T and place the duplicate at a different position (e.g. below the Histogram Shift layer) for additional compounded variation.
9. **Add a paint-driven "reveal window" for spatial control (technique 1):** add a Paint layer with a black mask placed *underneath* the wear generator in the stack, then switch the generator's own blend mode to `Multiply Light` — hand-painting on that paint layer now reveals the procedural wear effect only in the painted areas, instead of the wear showing uniformly across the whole model.
10. **Add a second, simpler manual paint layer for direct spot control (technique 2):** add another paint layer above the metal-edge-wear generator; painting in black adds the peeling-paint effect at that spot, pressing `X` inverts the active color so painting in white removes/erases the effect from already-peeling spots.
11. **Add finer edge detail via a second anchor point + referenced fill layer:** create a new anchor point on top of the existing paint-mask layer, name it (e.g. "edge paint"), then build a new layer with a black mask + Fill sub-layer that references that anchor point (the mask auto-populates from the referenced anchor data); pick a slightly brighter fade-toward-edge color and set blend mode to `Soft Light` to simulate how real peeling-paint edges lighten/fade.
12. **Add sharp sun-cracking detail:** duplicate the existing 2D/3D Voronoi Fractal noise, switch the duplicate from 3D Fractal to a plain **2D Voronoi** using the **Cell Tiles** preset — produces sharp cracking lines along the peeling-paint edges, appropriate for assets in harsh/sun-exposed environments (contrasted with a humid-environment look, which favors blistering/moss instead of sharp cracking).
13. **Organize with a folder, then reveal an underlying material through it:** group the paint layer and all its detail layers into one folder; anything placed *underneath* that folder in the stack shows through wherever the folder's own masking reveals it — demonstrated by dragging a `Metal Rust` material below the paint folder so it appears in the peeled-away areas.
14. **Fix a rust-material channel conflict:** when the dropped-in Metal Rust material's Height channel was found to be visibly deforming/affecting the paint layer above it, change the conflicting channel from Roughness to Height and switch that channel's blend mode from `Linear` to `Normal` to resolve the interaction cleanly.

### Layers / Tools / Settings
- **Base wear mask:** Fill layer + black mask + `Metal Edge Wear` generator (Grunge Amount down, Wear Level/Contrast up); alternates named: Curvature mask, Edge Damage mask/builder
- **Soft companion mask:** `Blur` filter, blend mode `Lighten`
- **Organic edge noise:** `3D Voronoi Fractal` (UDIM tile projection adjusted), blend mode `Divide`
- **Mask cleanup chain:** `Levels` (invert) -> `Histogram Shift` -> `Levels` (invert again) -> Height value increase
- **Anchor Point:** placed between the second Levels layer and the Histogram Shift layer, referenced by multiple downstream layers/masks
- **Paint-color layer:** inside the group, black mask referencing the anchor point + `Levels` adjustment
- **Erosion trick:** `Bevel` filter (non-standard use for organic mask distortion), duplicated via Ctrl+T and placed at a second stack position
- **Spatial-control trick 1:** black-mask Paint layer placed under the wear generator; generator blend mode switched to `Multiply Light`
- **Spatial-control trick 2:** Paint layer above the generator, black = add peeling, `X` to invert brush, white = remove peeling
- **Edge detail pass:** second Anchor Point ("edge paint") + Fill layer referencing it, brighter color, blend mode `Soft Light`
- **Sun-cracking detail:** duplicated Voronoi switched from 3D Fractal to 2D Voronoi, `Cell Tiles` preset
- **Organization:** paint layer + detail layers grouped in a folder; `Metal Rust` material placed underneath the folder to show through revealed areas; conflicting channel switched Roughness->Height, blend mode Linear->Normal

### Difficulty
Advanced — assumes comfort with generators, filters, and blend-mode math (Lighten/Divide/Multiply Light/Soft Light used deliberately for their exact mathematical behavior, not just visual trial-and-error), and introduces the anchor-point-as-shared-mask-source pattern applied across three separate downstream layers in one build.

### App & Version
Not stated on screen in any captured frame — no visible version-number UI element. The UDIM multi-tile workflow explicitly called out, plus the modern generator/anchor-point/Bevel-filter UI, are consistent with the same recent-version era as this skill's other ingested tutorials, but not independently version-pinned here.

### Tags
layers, fill-layer, paint-layer, masks, generator, anchor-point, blend-mode, height, roughness, basecolor, alpha, procedural, udim, texture-set, intermediate, advanced

---

## Related Tutorials
- [How to TEXTURE like a PRO with ANCHOR POINTS | Substance Painter Tutorial](how-to-texture-like-a-pro-with-anchor-points-substance-painter-tutorial.md) — different creator (Jared Chavez); the anchor-point-as-shared-mask-source pattern used throughout this hydrant video (one mask referenced by paint color, edge detail, and generator-reveal layers) is exactly the modular-reuse philosophy that anchor-points video teaches as its core lesson.
- [SUBSTANCE PAINTER: Building Masks Explained](substance-painter-building-masks-explained.md) — different creator (Jared Chavez); shares the blend-mode-stacking-as-mask-math approach (multiple generators/filters combined via specific blend modes to sculpt one final mask) though this hydrant video pushes further into Voronoi-noise and histogram-shift-specific tricks.
- (Wes McDermott's "How to create a paint peeling effect in Substance Painter" covers the same core subject — cross-link will be added here once that video is ingested.)
