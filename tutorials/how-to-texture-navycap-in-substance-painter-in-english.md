---
title: How to Texture NavyCap In Substance Painter in English
source: YouTube
url: https://www.youtube.com/watch?v=dGmVGU7aHb4
author: 3DRedBox
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated on screen; \"newest version\" name-checked for the duplicate-path-preserves-settings stitching feature, not otherwise pinned"
tags: [layers, fill-layer, paint-layer, masks, smart-material, generator, anchor-point, blend-mode, baking, mesh-maps, ambient-occlusion, curvature, thickness, high-to-low-poly, world-space-normal, texture-set, uv, pbr, basecolor, roughness, height, normal-map, alpha, procedural, particle-brush, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/how-to-texture-navycap-in-substance-painter-in-english/
frame_count: 11
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# How to Texture NavyCap In Substance Painter in English

**Source:** [YouTube](https://www.youtube.com/watch?v=dGmVGU7aHb4)
**Author:** 3DRedBox
**Duration:** 24m35s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hello everyone, welcome to this channel, my name is Mehdi from 3D Redbox. Today I'm going to show you how to text your Navy cap or military hat in Substance Painter. For a first step I'm going to export this model from 3ds Max as a FX file and import it in Substance Painter, so let's do it.
[0:22] Okay, now I'm going to drag and drop my FX file here and as you can see, for Substance FX is loading, the template should be on Unreal Engine 4 for this tutorial because I'm going to render it on MarbleSode Toolback and the Cuma Resolation is 2K and it's enough. The normal map format should be on DirectX and the rest of the options should be the same.
[0:47] Okay, so I'm going to press OK and clear this like here. So this is my UV and this is my 3D model. So the first step when you load the model in Substance Painter, you need to bake it. So I'm going to bake menu and output size should be on 4K until it is 64 inches enough and the bent normal should be turned on.
[1:14] And this is the setting that we have here, so let's bake it and see what is the result. So the baking process is finished and let's go back to painting mode and press F2 to have a viewport or 3D view.
[1:30] And let's go and check the bake channels. The ambient is good, the curvature, it's kind of, you know, there is an edge effect related to curvature mesh maps. It's not good for me and I'm going to show you a solution for that.
[1:47] And position is good, thickness. Oh, the thickness has some edge effect too. So maybe we should have another way to bake the curvature and the thickness to avoid this kind of effect. So for this solution, we need to go back to 3ds Max and create a hyperleversion of this model.
[2:10] Okay, we have a problem here in thickness and curvature map. And if I'm going back to Substance Painter, as you can see, this effect absolutely related to the wire and mesh wire.
[2:25] So what we can do here, for this solution, we have a cheat and a shortcut. So I'm going to add TurboSmooth modifier on the model and increase my iteration to something like this or maybe a little bit higher.
[2:43] And this model has the same UV that our low poly model has. Okay, so I'm going to bake this hyperleversion on itself and extract curvature and thickness map from the hyperleversion.
[2:59] The high poly model. And import it to the main Substance project. Okay, let's do that. I'm going to convert to edited poly. And after that, phi, export selected. And here, the name is high, broad substance.
[3:18] And press OK. So let's jump to a new project and bake this model. Okay, I'm here in a new Substance project, and I'm going to load high for Substance FX5 and press OK. The rest of the options is totally seamless to the previous one.
[3:40] And here, this is my UV, exactly the same UV that we have on the low poly model. And this is my hyperleversion. Okay, let's go and see what we have here. Turn mesh wire frame. That's it. Let's go to the bake menu. And I'm going to bake only curvature and thickness.
[4:07] Okay, the setting is 4K, until aging on 64X. And let's see what we have after the baking process. Okay, this is my hyperleversion of the Navy Cap. And this is the low poly version. So as you can see, the thickness map on the high poly model is very good.
[4:26] Very good. But on a low poly model is so edgy, and it's not good, especially when you want to have a smart material on your model. Okay, or use some generator. Okay, let's see on the curvature map, what we have here, the curvature map.
[4:44] Okay, it's absolutely better, the high poly version. So I'm going to export the texture with template mesh maps. Okay, so here, I have all the channels related to the mesh maps. But I only use thickness and curvature.
[5:07] If you have a good system, a good GPU, you can bake all the channels on the high poly version. It's going to give you a better result and import it to the main project and apply it on your low poly model. Okay, so I'm going to do that. I'm going to bake all the channels. And after that, import them into the low poly version project in substance painter.
[5:32] So let's do that and see what we have after that. Okay, I'm baked all the maps that I need, and I'm going to import resources, add resources. And in here, I'm going to select all the textures that I baked before. Okay, press open into project. All of them are textures. So I'm going to assign texture label on them and import.
[5:59] Okay, after that, I have them here. So let's go in a texture set setting and put the normal and normal, Benz normal on a Benz normal, thickness on a thickness and curvature on a curvature.
[6:15] And the last of them is ambient pollution. So, so let's go and check their thickness channel. Okay, this is the high poly version of the thickness mesh maps, and we have it on a low poly model. Okay, so the problem is solved. And we can continue our process for texturing these navy cap. So let's do that.
[6:40] Okay, let's create a three folder. The first one is a steel. I'm going to create a mask or that and the paint and going to element or the field selection. Press Alt and click on the black icon for the mask to go to the mask viewport. And now I can see what I'm masking on the model.
[7:06] Okay, that's it. So the second folder is leather part. Okay, for the leather part, I'm going to add black mask. And after that, let's add the paint and press Alt and the mask. Okay.
[7:25] And I'm not going to select this to a steam part. Okay, that's it. And let's go to UV. This icon is UV chunk field and press X to invert the selection and use this kind of selection to isolate my selection.
[7:49] Okay, that's it. The strap is select the front part of the cap is select. So everything is okay. And for the third one, I'm going to call it pop hat section.
[8:02] And actually, I can use anchor point here and use this anchor point in the fill layer on the top hat. And as you can see, I'm going to call the mask from leather part. Okay. And if I'm going to invert it. So the mask is okay. Right.
[8:27] But still, I need to subtract the steel part for fixing this issue. We have two ways. The first one is add an anchor point on steel part like this and load it here again. Okay.
[8:44] Okay. Oh, no, not the third at the field and load the steel mask and the blending mode of these steel mask. It should be on soft track. So in this way, we have a dynamic mask, which load the leather part mask and steel mask at the same time and create top hat mask section.
[9:09] Okay. The second way is to do it manually. You can add a paint paint layer. And after that, you can subtract these two little steel pot. Okay. So we have our categories and the folders. So let's load some smart material into these folders to increase our speed in texturing process.
[9:35] Okay. Let's see what we can add here on the folder to finish our texturing process. In the library, I'm going to search steel dark. So we have a steel dark edge. And it's very good for my steel section. And I'm going to add a little detail here. And for the leather part, I think I have something like V11 leather.
[10:06] The element volume of the smart material collection in the market. Okay. And yeah, I think 17 is good. Let's see. Yeah, it's perfectly fit on the model. So it's good here. Maybe I am going to add some brightness to the color, but now it's good.
[10:31] And for the top hat section, I'm going to use MK fabric. Yeah, this is the custom smart material, which I created, especially for this tutorial. Okay, so this is our base. And I'm going to continue the process.
[10:52] Okay, now I need some details like stitches and seams on the model. So let's create a paint layer over here and call it first layer stitches. And let's create a mask, a paint mask, and just select this part of the model, because I'm going to add the stitches and seams.
[11:22] Here. Okay, let's go back to the layer. And I'm going to add a seam. And let's pick some points on the model. Okay, that's good.
[11:40] Maybe change the environment map is the good solution. The exposure should on one. Yeah, it's better for my visual. Okay. And yeah. Yeah, it's okay. It should be straight.
[12:11] This one is good. This one is good. And I don't need this point. So I'm going to select it. And let's, I'm going to select this and press split. Okay. So it should be straight.
[12:36] And it's good. The position of the curve is good, but the effect and the normal intensity is so much. So let's go back to the path, select the path, and let's dive into the parameters.
[12:57] Okay, the technical parameters, normal intensity should be lower. The height range should be lower. Yeah, something like this is good. Yeah.
[13:12] So how can I use the same path, but not for the seam for the top of stitch. So it's so easy in the newest version of the substance painter. I'm going to duplicate the path, duplicate or control D, rename it to stitches.
[13:32] And I'm going back to my library and press top of stitching and boom, I have the same path. I have the same setting, but except for the seam, I have top of stitching now. So let's go to the classic stitches and press double stretch stitches.
[13:54] Okay, so it's good. And let's bring down the size. Yeah, three is good. The color should be soft light. The main color should be more brighter, like this. And thickness, I think 0.2 is better.
[14:16] And for the size, maybe one is very long. So I'm going to change it to 0.75. And yeah, so much better, so much better. And I'm going to use the same technique and the same setting for creating other stitches on the hat for avoiding longer video.
[14:40] I'm going to pause the video and do what I do, what should I do. And after that, I'm going to show you what's happening on the project. Okay, this is the result after adding stitches on the model. So let's have a breakdown and see what happened.
[14:55] The first one is cap stitches. I showed you how to do that. It's the first stitches layer. Okay, the second one is strap stitches. I just do a little renaming here. And the third one is top stitches. It's not too crazy, just a straight line goes around the model.
[15:18] So in here, I'm going to add some logo on the hat and finish my texturing process.
[15:27] Okay, now I'm going to create a fill layer here, call it patch. Okay, and load my texture on a base color. And let's see what happened if I change UV wrap to none and create a little patch here.
[15:48] Okay, so this is my end location of the UV cluster, as you can see, and if I bring down the texture, the texture is gone. And I don't see the continuous part of my patch. Okay, so this is the problem.
[16:11] And how can I solve this problem with the new feature in Substance Painter in the projection section? Okay, so let's go to projection and change UV projection to wrap projection.
[16:27] Okay, before doing anything else, I need to reset all settings in the UV transformations. Tiling should be on one. Okay, like this rotation should be on zero, offset should be on zero, zero, and that's it.
[16:46] So this is my projection window or section, and I need to go to this surface tool and just click and drag this window on my model.
[17:03] On the location that I want to projection goes over there. Okay, so for the scale, I'm not using tiling. I'm going to use a scale tool. So let's bring down the scale.
[17:16] Okay, like this, and fix this issue. Yeah, a little bit bigger. Again, on the surface mode. So it's not working well. We have some solution for that too.
[17:35] We should use edit vertices here. And after clicking the vertices, as you can see, I can control the vertices on the surface. Okay, just like that. So that's okay. And that's fine.
[18:01] So the projection, it's done. And I just need to use anchor point again to create dynamic mask for dispatch.
[18:12] So in the field layer, I'm going to turn off metal and normal. And for the height, I need to increase height amount, something like point three is good.
[18:26] But as you can see, the noise from under surface, it's going to show on my patch, but it's not what I want. Okay, so let's create mask first. And after that, we can take care about this matter.
[18:43] I'm going to add an anchor point and a black mask. And I'm going to load anchor point from the layer on its mask. So at the layer. And in the anchor point, I'm going to load patch. So it's good. And let's bring this slider here.
[19:08] Everything is okay here, but it should be invert. So I'm going to invert it. So that's it. It's okay. The mask is fully dynamic. If I'm going to move my projection, the mask should be following that.
[19:25] Okay, so everything is clear. And let's take care about the under surface noise. For that, you just need to right click on the blending mode, which is normal, and click apply to all channels and boom, everything is okay.
[19:44] So let's go back to mask and add a filter like Belair. So it's okay. We have blur, but I don't want to have this white outline. So let's add little and increase my black value. So easily I can fix this issue here.
[20:11] And if I want to add some noise on the surface, and I don't have any resources except that this texture, I can use this technique. I'm going to add a fill layer.
[20:24] This fill layer should have just height. And in height, I'm going to load the patch again. But the reference channel should be on base color. And boom, I have the noise. It's a random noise, depend on the RGB channel on the texture, but it's good enough for me right now.
[20:46] So let's play with this value. Yeah, I think it's okay, but it should be lower. So I'm going to maybe add level here, affected channel on height and decrease this effect. Something like this.
[21:12] Let's go back to the main channel, the main layer and decrease the roughness value. So it's done. And this is for the patch layer. And I'm going to add another layer, which is called logo and load my logo in black mask.
[21:37] The fill and the logo, it should be here. So it's my logo. You will have should be unknown. And I can decrease the scaling.
[21:49] Like this. And put it in this location. Smaller. Yeah, something like this. Okay, and let's go back to the layer. The height, it should be negative. And the roughness, it's something like this.
[22:17] For the base color, I'm going to use white value. And in the blending mode, it should be on the soft light. And boom, it's done. I'm going to pause the video and add extra details on the model. And after that, I'm going to break down what I did to reach the result.
[22:38] Okay, let's break down all the layers that we have now. For the first section, we have steel. The second stage, we have leather part. And for the third stage, we have top hat. Okay. And we have cap stitches. We have strap stitches. We have top hat stitches.
[22:59] And this little logo, which I played with the mask with the wrap filter. And I create a logo, which I use anchor point technique again. I load the logo, add some blur to increase the area. And again, load the logo anchor point and subtract it from itself.
[23:29] So I have these outline. And in the layer, we have a little height amount with the white value in the color. And the color blending mode is on the soft light. So it just bring more attention on the edge.
[23:49] And I have a scratch layer, which if I go here, you can see it's a random brush and use some stencil to have more variation in the color. It's not too fancy. The roughness is so high, it has some negative value in the height and white value in the base color.
[24:14] The point is the blending mode for the color should be on the soft light. So the last one is the patch, which we discuss about that. So this is the end of the story. Don't forget to hit the like button, subscribe and put your mind in the comment section for us. Be creative. Bye.



---

## Captured Frames

- [0:47] tutorials/frames/how-to-texture-navycap-in-substance-painter-in-english/frame_000.jpg
- [1:30] tutorials/frames/how-to-texture-navycap-in-substance-painter-in-english/frame_001.jpg
- [2:25] tutorials/frames/how-to-texture-navycap-in-substance-painter-in-english/frame_002.jpg
- [4:07] tutorials/frames/how-to-texture-navycap-in-substance-painter-in-english/frame_003.jpg
- [6:40] tutorials/frames/how-to-texture-navycap-in-substance-painter-in-english/frame_004.jpg
- [8:02] tutorials/frames/how-to-texture-navycap-in-substance-painter-in-english/frame_005.jpg
- [9:35] tutorials/frames/how-to-texture-navycap-in-substance-painter-in-english/frame_006.jpg
- [13:12] tutorials/frames/how-to-texture-navycap-in-substance-painter-in-english/frame_007.jpg
- [16:11] tutorials/frames/how-to-texture-navycap-in-substance-painter-in-english/frame_008.jpg
- [18:43] tutorials/frames/how-to-texture-navycap-in-substance-painter-in-english/frame_009.jpg
- [21:49] tutorials/frames/how-to-texture-navycap-in-substance-painter-in-english/frame_010.jpg

---

## Structured Notes

### Core Technique
Full military-cap texturing pipeline whose two throughline techniques are: (1) baking Curvature and Thickness from a separate **TurboSmooth-subdivided high-poly stand-in** (same UVs as the low-poly) to eliminate mesh-wire edge artifacts in those two mesh maps specifically, and (2) an anchor-point-driven **dynamic mask combination** (Soft Track blend of two loaded anchor masks) so a folder mask stays live even as the source masks it depends on change.

### Summary
Imports an FBX from 3ds Max into a new Unreal-Engine-4-template project (2K resolution, DirectX normal format), bakes standard mesh maps at 4K/64x AA with Bent Normal enabled, then discovers both Curvature and Thickness show a visible mesh-wire edge artifact from the low-poly's faceted geometry. Fix: re-export the same mesh with a TurboSmooth modifier (same UVs preserved) as a separate high-poly FBX, bake a second throwaway project against itself, export just Curvature+Thickness (or all channels, GPU permitting) as Template Mesh Maps textures, then re-import those as resources into the main low-poly project's Texture Set Settings so the clean high-poly-baked maps drive the same generators the low-poly's own bake would have. Sets up three base folders (Steel, Leather Part, Top Hat) using black masks + Paint sub-layers with Alt-click Polygon/UV-chunk-fill selection (X to invert). The Top Hat mask is built without any hand-painting: an Anchor Point loads the Leather Part mask (inverted), and a second Anchor Point loads the Steel mask set to **Soft Track** blend mode on top — combining two anchors this way keeps the resulting mask fully dynamic (edits to either source folder's mask propagate automatically), as an alternative to the equivalent manual fix (adding a Subtract paint layer). Smart materials (Steel Dark Edge, a marketplace V11 Leather, and a custom "MK Fabric" material) are dropped onto each folder for a fast base look. Stitches/seams are placed with the **Path/Stitching tool** (adjust Normal Intensity and Height Range after placement to tone down an overly strong initial result); a key workflow shortcut in "the newest version" of Painter is that duplicating a placed path (Ctrl+D) preserves its exact geometry, letting you swap only the stitch-style preset (Seam to Top Stitching, brush size/color/thickness tuned) rather than re-drawing the curve from scratch. A "USS Independence CV-62" fabric patch decal is placed with **Wrap Projection** (Projection = Wrap Projection, UV Transformations reset to Tiling 1 / Rotation 0 / Offset 0,0, then Surface tool click-drag to place the projection window, Scale tool instead of Tiling for sizing, and Edit Vertices for local correction when Surface mode alone doesn't fit the curved cap surface) — the earlier plain-UV attempt failed because the patch fell across a UV-island seam and broke continuity. The patch's own Anchor Point (loaded from itself, inverted) drives a dynamic Height-based emboss mask that follows the projection if it's moved later; **right-click blend mode → Apply to all channels** is used to fix a case where an unwanted under-surface noise pattern was bleeding through only some channels. A from-scratch fabric-noise trick: an extra Fill layer with only the Height channel enabled, loaded with the patch texture again but with its **Reference Channel set to Base Color** instead of Height, produces a random RGB-driven bump pattern usable as free surface noise when no other resource is on hand — toned down with a Levels filter on Height. The Logo layer (also anchor-point-driven, self-referencing outline via Blur + Subtract for an embossed edge) uses negative Height + white Base Color in Soft Light blend mode to read as a debossed/inked mark rather than raised geometry. Closes with a hand-painted scratch layer (stencil-varied brush, high Roughness, negative Height, white Base Color in Soft Light) for wear accents.

### Key Steps
1. Import the FBX with the Unreal Engine 4 starter-assets template (2K Document Resolution, DirectX Normal Map Format), bake standard mesh maps at 4K/64x AA, Bent Normal enabled.
2. Inspect the bake result per-channel: Curvature and Thickness both show a hard mesh-wire edge artifact traceable directly to the low-poly's facets.
3. Back in the DCC app, add a **TurboSmooth** modifier to the same mesh (same UVs preserved), export as a separate high-poly FBX.
4. In a throwaway new Substance project, load the high-poly FBX and bake only Curvature + Thickness (or all channels if GPU allows) against itself.
5. Export those bakes as Template Mesh Maps textures, then **Import Resources** them into the real low-poly project; in **Texture Set Settings**, manually wire Normal→Normal, Bent Normal→Bent Normal, Thickness→Thickness, Curvature→Curvature, AO→Ambient Occlusion — the low-poly model now reads the clean, artifact-free high-poly-baked Curvature/Thickness.
6. Build 3 base folders (Steel, Leather Part, Top Hat) via black mask + Paint sub-layer, Alt-click to preview the mask, Polygon/UV-chunk Fill selection with X to invert for fast region isolation.
7. Build the Top Hat mask without hand-painting: add an Anchor Point, load the Leather Part folder's mask into it (inverted), then add a second Anchor Point loading the Steel folder's mask with blend mode **Soft Track** — the combined result is a live, self-updating "everything except leather and steel" mask (equivalent manual alternative: a plain Subtract-mode paint layer).
8. Drop Smart Materials onto each folder (Steel Dark Edge, marketplace V11 Leather, custom MK Fabric) for the fast base look; nudge individual channel values (e.g. brightness) afterward as needed.
9. Place stitches/seams with the **Path/Stitching tool**, click points along the model, then reduce Normal Intensity and Height Range in the path's Technical Parameters if the initial result reads too strong.
10. To reuse a placed stitch path with a different stitch style, **Ctrl+D to duplicate the path** (geometry preserved exactly), rename it, then swap the stitch preset from the library (e.g. Seam → Top Stitching / Double Stretch Stitches) and retune size/color/thickness — much faster than re-drawing the curve.
11. Place a fabric patch decal with plain UV projection first — note the failure mode (patch straddles a UV-island seam, breaks continuity at the edge) — then fix by switching **Projection → Wrap Projection**: reset UV Transformations (Tiling 1, Rotation 0, Offset 0/0), use the Surface tool to click-drag the projection window onto the target spot, the **Scale** tool (not Tiling) to size it, and **Edit Vertices** to hand-correct local fit on curved geometry the Surface tool alone can't match.
12. Give the patch layer a dynamic emboss mask via its own Anchor Point (load the layer's own result, inverted), enable Height and set a small amount (~0.3); if an unwanted under-surface noise leaks into only some channels, **right-click the blend mode → Apply to all channels** to normalize it across the whole layer.
13. Clean the emboss mask edge with a Blur filter, then raise the filter's black-point slightly to remove an unwanted white outline artifact from the blur.
14. Free procedural noise trick: add a Fill layer restricted to Height only, load the same patch texture into Height but set its **Reference Channel to Base Color** (not Height) — produces a random RGB-derived bump pattern usable as surface noise without a dedicated resource; tone down with a Levels filter on the Height channel.
15. Build the Logo layer the same anchor-point way (self-referencing outline via Blur + Subtract for a debossed rim), set Height to a negative value, Base Color to white, blend mode **Soft Light** — reads as an inked/debossed mark rather than raised geometry.
16. Finish with a hand-painted Scratch layer: randomized stencil-varied brush strokes, high Roughness, negative Height, white Base Color, Soft Light blend for wear accents.

### Layers / Tools / Settings
- `Baking → Common Settings`: Output Size 4K, Anti-Aliasing 64x, Bent Normal enabled
- High-poly rebake workaround: TurboSmooth-subdivided duplicate mesh (same UVs) → separate throwaway project → bake Curvature+Thickness only → export as Template Mesh Maps → re-import as resources → wire in Texture Set Settings
- Folder masks: black mask + Paint sub-layer, Alt-click for isolated mask preview, Polygon/UV-chunk Fill (X = invert)
- `Anchor Point` (folder mask), second Anchor Point with blend mode **Soft Track** for dynamic multi-source mask combination
- Smart Materials: Steel Dark Edge, V11 Leather (marketplace), MK Fabric (custom)
- `Path`/Stitching tool: Normal Intensity, Height Range (Technical Parameters); Ctrl+D duplicate-path-preserve-geometry for stitch-style swaps (Seam, Top Stitching, Double Stretch Stitches — size/color/thickness tuned per style)
- `Fill layer → Projection = Wrap Projection`: UV Transformations reset (Tiling 1, Rotation 0, Offset 0/0), Surface tool (placement), Scale tool (sizing, not Tiling), Edit Vertices (local correction)
- Blend-mode right-click → **Apply to all channels**
- `Blur` filter (mask edge cleanup) + raised black point to remove blur-induced white outline
- Height-from-Base-Color noise trick: Fill layer, Height channel only, texture loaded with **Reference Channel = Base Color** instead of Height; `Levels` filter to tone down
- Logo/Scratch layers: negative Height, white Base Color, blend mode **Soft Light**

### Difficulty
Advanced (the TurboSmooth hi-poly rebake workaround and the two-anchor Soft-Track dynamic mask combination are non-obvious techniques beyond basic layer/mask work)

### App & Version
Not stated on screen. The path-duplication-preserves-geometry stitching workflow is explicitly called out as "the newest version of the Substance Painter" at time of filming, but no numeric version appears in transcript or captured frames.

### Tags
`layers` `fill-layer` `paint-layer` `masks` `smart-material` `generator` `anchor-point` `blend-mode` `baking` `mesh-maps` `ambient-occlusion` `curvature` `thickness` `high-to-low-poly` `world-space-normal` `texture-set` `uv` `pbr` `basecolor` `roughness` `height` `normal-map` `alpha` `procedural` `particle-brush` `intermediate` `advanced`

---

## Related Tutorials
- [Using UV set and Stencils In Substance Painter -- English version](using-uv-set-and-stencils-in-substance-painter----english-version.md) — same creator (3DRedBox); shares the theme of solving a projection/UV-space rendering problem with a dedicated Painter tool (UV-set-to-UV-set projection there, Wrap Projection here) rather than hand-painting around it.
- [Texturing Tactical Boots In Substance Painter](texturing-tactical-boots-in-substance-painter.md) — same creator; shares the same anchor-point-driven decal/patch workflow (Anchor Point + Extract Alpha style dynamic transparent masking) and stitching-tool usage.
- [How to texture a realistic slipper model](how-to-texture-a-realistic-slipper-model.md) — same creator; shares the Paint-Along-Path/stitching-tool technique and stacked anchor-point-referenced mask layers as the core organizing principle.
- [How to Create a Realistic Poison Bottles Material Using Substance Painter](how-to-create-a-realistic-poison-bottles-material-using-substance-painter.md) — same creator; shares the anchor-point mask-reuse-across-folders pattern (a Pass-Through collector layer there, direct multi-anchor Soft-Track combination here).
