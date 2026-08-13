---
title: 🎨 Texturing Women's Shorts with Lace Trim in Substance Painter 🎨
source: YouTube
url: https://www.youtube.com/watch?v=6eRY49oxJNI
author: 3DRedBox
ingested: 2026-08-12
app: "Substance 3D Painter"
version: "not stated on screen; UI (Display Settings ACES tone-mapping, standard Shader Settings panel, no OpenPBR/Skew) consistent with the pre-12.1-era UI seen across this creator's other ingested videos"
tags: [layers, fill-layer, paint-layer, masks, generator, anchor-point, blend-mode, alpha, procedural, basecolor, roughness, height, normal-map, opacity, metallic, smart-material, texture-set, iray-render, viewport, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/texturing-womens-shorts-with-lace-trim-in-substance-painter/
frame_count: 10
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# 🎨 Texturing Women's Shorts with Lace Trim in Substance Painter 🎨

**Source:** [YouTube](https://www.youtube.com/watch?v=6eRY49oxJNI)
**Author:** 3DRedBox
**Duration:** 23m1s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hey everyone, I'm Mehdi from TD RedWax Channel and today we want to turn this to this in Substance Painter.
[0:19] Now let's go to the video itself, but before jumping to the video, let me introduce you the brand new course that we released for Substance Painter.
[0:30] The Learning Substance Painter is easier than ever. Hey all Substance Lovers, Tech Change Seekers and awesome future artists, welcome to ultimate course for Learning Substance Painter from Zero to Hero.
[0:46] Ready to learn how to texture with different projects? Substance Master released a brand new course for those who want to learn to texture with Substance Painter.
[1:00] In this course we covered from preparing the model to rendering different projects, different challenges.
[1:06] If you want to level up your skill in texturing, come and check the Substance Master Ultimate course for Learning Substance Painter.
[1:14] Okay, let's start the process. For the first step, I'm going to load the 3D model into Painter and the default setting is okay for me.
[1:22] I press okay and now it's time to jump to shader and viewport setting.
[1:27] Okay, now I'm going to display setting and change the environment map to a city automicle and for the environment exposure, I'm going to change it to one.
[1:38] And in camera setting, let's change the focal length to 75 and after that, I'm going to change the tune mapping function to aces and now we are done in display setting.
[1:53] Okay, let's go for the shader setting. In the shader parameters, I'm going to turn on double sided, enable alpha blending because I'm going to use alpha map and just enable bent normal.
[2:09] That's okay. And we are done in shader setting.
[2:13] Okay, now it's time to go for the main part. I'm going to turn off the lace texture set for a moment and now it's time to work on the main part.
[2:24] And I'm going to use, okay, let's start the process for the main part. I'm going to turn off the lace for a moment and now I'm going to use fabric canvas, smart material,
[2:37] from the library that it comes with the substance painter and I'm going to tweak it. Let's go here, turn off all the layers.
[2:48] I don't want sharpen layer here because I'm going to add the sharp filter at the end and for the base, let's change the color to something like light blue.
[3:01] I have it in the swatch section and yeah, this is good.
[3:09] Okay, let's go for the pattern and color adjustment. I don't want to have HSL filter here, so let's remove it and this is the pattern.
[3:24] It's okay for me. Let's change the size of the document to 2K to see and understand well this material.
[3:37] Okay, now I'm going to turn on the fibers. That's okay. And I don't want to have folds here because I'm going to add wrinkles in other way.
[3:47] And yeah, and this is the edge fold. I don't want it. That's okay and this is the dust.
[3:56] Okay, so we are good for the fabric canvas crease material here right now and let's go for add some touch on the material.
[4:07] For example, let's create a fill layer. Okay, I'm going to call it gradient color and I just need to have color, make it black, change the blending mode to soft light, add the black mask and in here I'm going to add generator and use 3D linear.
[4:29] Let's go to the mask and in here I'm going to invert it and play with the balance and contrast to have the effect that I want here on the model.
[4:41] As you can see, you can control it. Okay, that's great. Let's play with the contrast and I'm happy with the result.
[4:51] Okay, let's go and add a paint layer. I'm going to rename it to seam and stitches and I'm going to use the top stitching tool in the shelf for creating stitch on the model.
[5:22] Okay, now it's time to add the wrinkles to the model and on the surface.
[5:30] And it's time to add wrinkles to the surface. I'm going to use a different way. It's a similar way that we use in Zbrush to add wrinkles on the surface.
[5:42] In here I just create some fabric wrinkles in the Marvel's designer and bake it as an alpha and I'm going to use it in Substance Painter directly without using Zbrush or any third party software.
[5:57] So for the first step, let's import the wrinkles into the project and I'm going to use them and import them as alpha.
[6:08] Okay, you can download these two wrinkles with the link in the description and let's use it.
[6:16] I'm going to create a fill layer and put it after Fabric Canvas and change the name to the wrinkles and we need just height.
[6:29] Okay, let's change the height to something like 0.5 and I'm going to add black mask, add fill and now it's time to load these wrinkles to the grayscale input.
[6:48] Okay, let's go to the 2D view, the F3 on the keyboard and let's go to the mask, change the UV up to none and now I'm going to fix the position for this wrinkle.
[7:06] Okay, you can check it on the 3D view. Okay, that's great. Now we have some good wrinkles on the surface and yeah, but it's not as strong enough.
[7:23] Okay, and this is the highest amount of the height, but it's not as strong. How we can improve the visual quality here.
[7:35] We can go here after Siemens stitch, add the paint layer and let's change the name to effect layer.
[7:45] Okay, change the blending mode to pass through and right click and apply to our channel. Okay, and in here I'm going to add filter and in the filter we have height to normal.
[7:59] Okay, that's great. Change the use word you need option to the false and now we can control the normal intensity and let's disable fabric canvas for the moment and as we can see, yeah, it's super good to have height to normal effect on the wrinkles.
[8:25] Okay, that's great, but we need to control other layers, height intensity, but we can do a trick that effect and wrinkles and bring it back in the down of the list.
[8:41] But we couldn't see the effect here because we need to go to height channel and change the blending mode of fabric canvas crease to linear dodge.
[8:53] And after that we need to go to the normal and change the blending mode to normal map combine. And now we can see the effect of the wrinkle without any distortion from other layers.
[9:09] Okay, so let's change the normal intensity to something reasonable. And yeah, that's great. And in the wrinkle, let's duplicate change the blending mode to linear dodge. And yeah, go here and fix the position.
[9:28] Okay, that's great. Yeah, we have the wrinkle on the surface so much easy. Okay, let's add another fill layer and now it's time to add this kind of wrinkle here. Okay, that's great.
[9:59] Okay, now I think it's enough for the wrinkles and the details on the surface. It's time to create pattern for this project. Let's go for pattern creation section. Okay, now it's time to bring some pattern on the surface. And for this purpose, you can create your own pattern.
[10:18] You can search in the Google and use the resource out there, or you can use AI for pattern creation. Okay, so in this video I'm going to use low nodal AI for the pattern creation section. So let's go to the image creation.
[10:39] Okay, now we are in image creation section. And for the first step, you need to change the preset to whatever you want. For example, here I need to have a vibe of graphic design. Okay, so I change it to graphic design and in the preset style, I go for graphic design vector, you can choose whatever you want and test and have fun.
[11:04] Okay, and in generation mode, I choose fast because the quality is just only for premium feature and premium users. And in a dimension, I choose one-on-one and for the size, medium is enough for us. And in advanced setting, you need to turn on negative prompt and tiling.
[11:27] Tiling is super important when we want to create tiling pattern. Okay, and for the negative prompt, you can remove whatever you don't want in the pattern. Okay, so I will give you the pattern prompt for getting the same result and you have access to negative prompt too.
[11:48] Okay, and you just need to copy and paste prompt in here and negative prompt in here. And in here, you just need to hit on the generate. And after a short while, you have some pattern that you can actually use in Substance Painter. So I'm going to download some beautiful pattern here. And I'm going to test it in Painter.
[12:14] Okay, let's go back to the painter. Okay, now it's time to use the pattern inside Substance Painter. And for this purpose, we need to create a fill layer and let's call it pattern. We need just color, height and roughness. And in the base color, we are going to load the pattern that we create. Okay, like this.
[12:40] And let's change tiling to something like tree. Okay, that's great. I'm going to rotate it 90 degrees. We can rotate it again. And yeah, that's great. Let's add a black mask. And in here, I'm going to add a fill layer. Let's put it as one. And now I'm going to add a paint layer.
[13:09] Okay, and let's go to the UV chunk, select all the UV island here, change the blending mode to Subtract. That's great. I'm going to invert it with the X on the keyboard.
[13:28] Okay, and now let's select the island that we want to have. Okay, and this is the mask, the original mask, as you can see. Yeah, that's great. And I'm going to add an anchor point. Okay, and let's go back to the mask, add fill and use the anchor point here to create a specific mask for this layer.
[13:58] Okay, let's change the blending mode to multiply. Okay, so let's play with the slider here. We want to create a perfect mask for our layer. That's great. Okay. And we can add height amount.
[14:25] Okay, too perfect. Let's change the design and see what is the best. I think this one is better. You can change and play the pattern with different pattern and get your result. It's okay.
[14:50] And yeah, that's good. I think that's good. And it's enough. Okay, let's go here, change the roughness value to something like 0.8. And for the height, I'm going to put it at 0.3. And let's go here and add a filter like blur.
[15:13] Okay, and for the blur, let's choose something like 0.2 to avoid any aliasing effect on the edge. And for the lace part, I'm going to use a product from our market that you can find it with the link in the description.
[15:32] And you can download for free the material that I use here in this tutorial and use it on your works. Okay, for the lace part and for the top and strap, I use fabric canvas crease that we modified for the main body.
[15:51] And now I'm going to use it again and just I create a base to for create color variation for the lace and strap. Okay, that's great. Now it's time to import some resource and work on the lace part.
[16:08] And for importing these resources, you just need to select them and click and drag into the library and just import it to your project or you can import to your library. Okay, I'm going to import it. And now we have these two layers here. So let's use it.
[16:28] Before using the lace, we need to go to the texture set setting and add the opacity channel. Okay, and now it's time to use the tool that we imported before. I'm going to create a paint layer. Let's call it the lace and right click on the paint and add fill.
[16:51] So basically we use fill layer as a sub layer of the paint layer that we create and rename it to the lace. And let's load the tool that we create in the material mode. And let's turn off the color, roughness, metal, normal, and we just need to have height and opacity.
[17:15] Okay, let's rotate it and change the UV wrap to repeat horizontally. And for better controlling at the first step, I'm going to add a black mask and with the polygon mode and element mode or mesh fill, I select this one.
[17:33] Okay, that's great. Let's go back to the sub layer. I'm going to call it one. Okay, let's change the position and scale.
[17:44] And now it's time to add the second part. For the second part, I'm going to use the next tool. Yeah, that's great. And for seeing both layer together, we need to go to the data channel opacity and change the blending mode from normal to
[18:14] linear dodge. In this way, we can see both pattern together. Okay, let's keep the height and opacity. That's great. And fix the size of the lace and scale it down. And yeah, that's great. We are done.
[18:42] Okay, let's add a level and change the effect channel to opacity and play with the slider here to have a strong mask on the opacity. And yeah, that's great. This is what I want from the tool and the result is super good.
[19:06] But how we copy these lines on the other part, it's not a good idea to duplicate the layer because we always want to change the opacity, the pattern, the color and etc.
[19:23] So the best way is add an anchor point here and add another fill layer and just load anchor point of the lace in this fill layer as a sublayer, a paint layer that we create and rename it to the lace.
[19:42] Okay, and now we have this power to control this one. Okay, let's change the blending mode of the opacity to linear dodge. Okay, now we can see we can duplicate the layer. And let's go to the mask, select all the area here.
[20:10] Okay, you can see on the 3D model. And now it's time to put the layer where we want. Okay, for example, yeah, here. And that's great.
[20:31] And I'm going to pause the video and place all the strap on the position. Okay, now we are done and let's see what we have at the end. This is the number one. Okay, this is the number two. That's fine.
[20:49] This is the level that we increase the intensity of the opacity. And we create the anchor point and we duplicate this anchor point data on each strap. But we have some strange line here and how we can solve this in the one and two.
[21:12] In the channel mapping section in the mask, we can load the opacity and boom, everything works. Everything works well. Okay, so that's it. And we are done in a lace part. And for the last detail, I'm going to create another fill layer.
[21:40] And let's call it the strip, keep the height, increase the height amount, add a black mask, go to the polygon field and select this line here. Okay, add fill, search about the strip.
[22:03] That's great. In the pattern, I'm going to decrease the shift. And now let's increase the strip amount. Let's increase the tile and we are good. And let's change the blending mode to multiply.
[22:23] And in this way, we have only a strip on the mask selection that we did it already. Okay, let's go back to the material mode and boom, we have this effect on the top section. And we are done with this tutorial.
[22:40] I hope you liked it. Learn some new things here. Please don't forget to hit the like button, share your mind in the comment section and subscribe our channel. Please pay attention to the description. I put all the information that you need in the description for you.
[22:58] And for the last word, be creative. Bye.



---

## Captured Frames

- [1:53] tutorials/frames/texturing-womens-shorts-with-lace-trim-in-substance-painter/frame_000.jpg
- [3:24] tutorials/frames/texturing-womens-shorts-with-lace-trim-in-substance-painter/frame_001.jpg
- [6:29] tutorials/frames/texturing-womens-shorts-with-lace-trim-in-substance-painter/frame_002.jpg
- [8:53] tutorials/frames/texturing-womens-shorts-with-lace-trim-in-substance-painter/frame_003.jpg
- [12:40] tutorials/frames/texturing-womens-shorts-with-lace-trim-in-substance-painter/frame_004.jpg
- [13:58] tutorials/frames/texturing-womens-shorts-with-lace-trim-in-substance-painter/frame_005.jpg
- [16:51] tutorials/frames/texturing-womens-shorts-with-lace-trim-in-substance-painter/frame_006.jpg
- [18:42] tutorials/frames/texturing-womens-shorts-with-lace-trim-in-substance-painter/frame_007.jpg
- [21:12] tutorials/frames/texturing-womens-shorts-with-lace-trim-in-substance-painter/frame_008.jpg
- [22:03] tutorials/frames/texturing-womens-shorts-with-lace-trim-in-substance-painter/frame_009.jpg

---

## Structured Notes

### Core Technique
Garment texturing (women's shorts with a floral AI-generated pattern and a crochet lace trim) built from viewport/shader calibration, Marvelous-Designer-baked wrinkle alphas applied directly as height data (no ZBrush step), an AI-image-generator-sourced tiling pattern, and an opacity-channel-driven lace decal system duplicated across straps via anchor points.

### Summary
Opens with viewport/shader calibration rather than jumping straight into layers: environment map + exposure, camera focal length 75mm, tone mapping set to `ACES`, and Shader Settings with `Double Sided`, `Alpha Blending` (needed later for the opacity-channel lace), and `Bent Normal` all enabled. The main fabric body starts from the built-in `Fabric Canvas Crease(d)` smart material, pruned down (sharpen/HSL/folds/edge-fold sublayers removed in favor of building those effects manually later) and recolored. A `Gradient Color` fill (Soft Light blend, inverted 3D-Linear-generator mask) adds broad value variation, and a `Seam and Stitches` paint layer uses the shelf's stitching tool for visible seams. The video's signature technique is importing two Marvelous-Designer-baked wrinkle alphas directly as Height-only fill layers, then routing their effect through a top-of-stack Pass-Through "Effect" layer's `Height to Normal` filter — with the crucial detail of setting the *lower* wrinkle layers' own Height channel to `Linear Dodge` and Normal channel to `Normal Map Combine` so the wrinkle detail survives underneath the effect layer without being overwritten or distorted by layers above it. A base pattern is generated with an AI image tool (tiling explicitly enabled in the generator settings) and applied as a `Color+Height+Roughness` fill layer, masked via a UV-island paint selection refined with an anchor-point-referenced Multiply mask. The lace trim is built as a purchased/imported lace tool loaded into a Height+Opacity-only fill layer (after adding the `Opacity` channel via Texture Set Settings), with two overlapping lace-strip variants combined via `Linear Dodge` on the Opacity channel and sharpened with a `Levels` filter targeting Opacity specifically; the finished lace layer is then anchor-pointed so it can be duplicated onto every strap via lightweight anchor-referencing sublayers instead of copying the whole layer (with the mask's Channel Mapping set to reference Opacity directly to fix a stray-line artifact). A final `Strip` fill layer (Multiply blend, polygon-selected mask) adds a decorative stripe accent on the waistband trim.

### Key Steps
1. **Calibrate the viewport/shader before texturing:** Display Settings — environment map set to a city HDRI, exposure to 1, camera focal length 75mm, tone mapping `Function` set to `ACES`; Shader Settings — enable `Double Sided`, `Alpha Blending` (needed for the lace's opacity channel later), and `Bent Normal`.
2. **Start the main fabric from the built-in `Fabric Canvas Crease(d)` smart material**, then prune it: delete the built-in Sharpen sublayer (a Sharpen filter will be added manually at the end instead), recolor the base to light blue, remove the HSL adjustment sublayer, keep Fibers on, but turn off Folds and Edge Fold (wrinkles will be added separately via baked alphas), keep Dust.
3. **Add a `Gradient Color` fill layer** for broad value variation: black color, `Soft Light` blend, black mask + `3D Linear` generator, inverted, then balance/contrast tuned live against the model.
4. **Add a `Seam and Stitches` paint layer** using the shelf's stitching brush/tool to hand-place visible seam stitching along the garment's construction lines.
5. **Import Marvelous-Designer-baked wrinkle alphas as Height-only fill layers** (placed after Fabric Canvas Crease): Height set to ~0.5, black mask + Fill loading the wrinkle alpha into the grayscale input, UV Wrap set to `None` for 2D placement/positioning via the 2D view (F3).
6. **Boost wrinkle visibility with a Pass-Through "Effect" layer + Height to Normal filter:** add a paint layer named `Effect` above Seam and Stitches, blend mode `Pass Through`, apply to all channels; add a `Height to Normal` filter with `Use World Unit` off, tuning Normal Intensity until the wrinkle read strengthens dramatically (demonstrated by isolating with Fabric Canvas Crease disabled).
7. **Fix the "effect layer can't see the wrinkle layers below it" problem with a channel-specific blend-mode trick:** move the Effect + wrinkle layers back down the stack, then on the Fabric Canvas Crease layer specifically set its Height channel's blend mode to `Linear Dodge` and its Normal channel's blend mode to `Normal Map Combine` — this lets the wrinkle detail read through correctly without being distorted or hidden by the layers stacked above.
8. **Duplicate the wrinkle fill layer for a second wrinkle placement**, keeping it in `Linear Dodge` blend and repositioning independently in the 2D view.
9. **Generate a tiling base pattern with an AI image tool** rather than hand-painting or sourcing stock art: set a style preset (e.g. "graphic design vector"), 1:1 aspect, explicitly enable `Tiling` and a negative prompt in Advanced Settings (tiling is called out as essential for a seamless in-Painter result), generate, download.
10. **Apply the AI pattern as a `Pattern` fill layer** (Color + Height + Roughness only): load the downloaded pattern into Base Color, tiling ~3, rotated 90°; mask built from a UV-island paint selection (select all islands, `Subtract` blend, invert with X, then re-select only the desired island) captured via an Anchor Point, referenced by a separate Fill sublayer in `Multiply` blend so the pattern only appears within the selected UV region; roughness set ~0.8, Height ~0.3, finished with a `Blur` filter (~0.2) on the mask to soften pattern edges and avoid aliasing.
11. **Add the `Opacity` channel via Texture Set Settings** before starting the lace work — required because the lace decal relies on an alpha/opacity cutout rather than a solid fill.
12. **Build the lace trim as a paint layer with a fill sublayer:** create a `Lace` paint layer, right-click → Add Fill for a sub-layer, load the purchased lace tool material, disable Color/Roughness/Metal/Normal so only Height and Opacity carry data, set UV Wrap to `Repeat Horizontally`, mask via `Polygon Fill` (Element/Mesh Fill mode) to isolate the trim geometry, position/scale in 2D.
13. **Layer a second lace tool variant on top**, combined via the Opacity channel's blend mode set to `Linear Dodge` (Normal → Linear Dodge, not the layer's overall blend mode) so both lace patterns are visible simultaneously rather than one occluding the other.
14. **Sharpen the lace cutout with a `Levels` filter targeting the Opacity channel specifically** (`Effect channel` set to Opacity), pushing the slider until the opacity mask reads as a clean, strong cutout rather than a soft gradient.
15. **Duplicate the lace onto every strap via Anchor Point, not layer copies:** anchor-point the finished lace paint layer, then for each additional strap create a new fill layer that loads that anchor point as its mask source (so opacity/pattern/color edits to the original propagate everywhere) — explicitly framed as the correct approach because "we always want to change the opacity, the pattern, the color" and duplicating whole layers would break that; set each duplicate's Opacity-channel blend mode to `Linear Dodge` and manually place/select the correct area per strap.
16. **Fix a stray-line artifact on the duplicated straps via mask Channel Mapping:** in the mask's `Channel Mapping` section, explicitly set the mask to reference the source layer's `Opacity` channel — resolves an artifact that appeared on two of the strap instances.
17. **Add a final `Strip` fill layer for a waistband accent:** Height only, increased height amount, black mask via Polygon Fill selecting the trim line, Fill loading a `Strip` pattern (reduced Shift, increased Strip count/tiling), blend mode `Multiply` so the stripe only reads within the already-selected mask area.

### Layers / Tools / Settings
- **Smart material used:** built-in `Fabric Canvas Crease(d)` (heavily pruned — Sharpen/HSL/Folds/Edge Fold sublayers removed or disabled)
- **External content used:** two Marvelous-Designer-baked wrinkle alphas (imported as grayscale height alphas, no ZBrush step), a purchased lace "tool" material (loaded twice, two variants combined), an AI-generated tiling floral pattern image (image-generation settings: style preset, 1:1 aspect, Tiling + negative prompt enabled in Advanced Settings)
- **Generators used:** `3D Linear` (Gradient Color mask, inverted)
- **Filters used:** `Height to Normal` (World Unit off, tuned Normal Intensity), `Blur` (~0.2, pattern-edge anti-aliasing), `Levels` (Effect channel set to Opacity, lace cutout sharpening)
- **Fills/patterns used:** `Strip` (final waistband accent, reduced Shift, increased tiling)
- **Blend-mode tricks (channel-specific, not layer-wide):** Fabric Canvas Crease's Height channel set to `Linear Dodge` and Normal channel set to `Normal Map Combine` so wrinkle layers read through correctly from below a Pass-Through effect layer; lace Opacity channel set to `Linear Dodge` to combine two lace variants without one occluding the other
- **Layer-wide blend modes used:** `Soft Light` (Gradient Color), `Multiply` (AI-pattern mask layer, final Strip layer), `Pass Through` (top-of-stack Effect layer applied to all channels)
- **Anchor Point usage:** one on the UV-island pattern mask (referenced by a Multiply sublayer), one on the finished Lace paint layer (referenced by new fill-layer sublayers for every additional strap instead of duplicating the whole layer)
- **Mask tooling:** `Polygon Fill` (Element/Mesh Fill mode) for UV-island/geometry-based mask selection, mask `Channel Mapping` explicitly pointed at the source layer's `Opacity` channel to fix a strap artifact
- **Texture Set Settings:** `Opacity` channel added specifically to support the lace decal
- **Shader Settings:** `Double Sided`, `Alpha Blending`, `Bent Normal` all enabled
- **Display Settings:** ACES tone mapping, city-HDRI environment (exposure 1), 75mm camera focal length

### Difficulty
Advanced — the channel-specific (not layer-wide) blend-mode routing for the wrinkle/effect-layer interaction and the opacity-channel lace system (dual-variant Linear Dodge combine, Levels-on-Opacity sharpening, anchor-point-driven multi-strap duplication with Channel Mapping fixes) are genuinely advanced techniques; the AI-pattern-generation step is comparatively simple but assumes access to an external AI image tool.

### App & Version
Substance 3D Painter — version not stated on screen. Display Settings (ACES tone mapping, environment/exposure controls) and Shader Settings (Double Sided, Alpha Blending, Bent Normal) shown are long-standing features not tied to a specific version; overall UI is consistent with the pre-12.1-era (no OpenPBR/Skew) seen across this creator's other ingested videos.

### Tags
layers, fill-layer, paint-layer, masks, generator, anchor-point, blend-mode, alpha, procedural, basecolor, roughness, height, normal-map, opacity, metallic, smart-material, texture-set, iray-render, viewport, intermediate, advanced

---

## Related Tutorials
- [Texturing a Black Suit in Substance Painter](texturing-a-black-suit-in-substance-painter.md) — same creator (3DRedBox); both use UV-island/Polygon-Fill mask selection combined with anchor points to drive reusable, non-rendered mask sources.
- [How to texture a realistic slipper model](how-to-texture-a-realistic-slipper-model.md) — same creator; shares the anchor-point-as-reusable-mask-source philosophy (placeholder masks there, the multi-strap lace duplication here) and a Pass-Through "Effect" layer used to stack finishing filters at the top of the stack.
- [Texturing a Worn Wooden Stool in Substance Painter](texturing-a-worn-wooden-stool-in-substance-painter.md) — same creator; the wrinkle layers' Height-channel-to-Linear-Dodge trick here is the same channel-specific blend-mode approach used for the stool's border-effect layer.
- [Texturing a shawl in substance painter](texturing-a-shawl-in-substance-painter.md) — same creator; both duplicate a finished decorative layer (lace there, stitching/borders here) onto multiple garment locations via anchor points rather than copying whole layers.
