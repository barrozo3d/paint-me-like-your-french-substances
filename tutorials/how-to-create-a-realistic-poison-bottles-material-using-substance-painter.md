---
title: How to Create a Realistic Poison Bottles Material Using Substance Painter
source: YouTube
url: https://www.youtube.com/watch?v=386o64sxSpw
author: 3DRedBox
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated on screen; the Pass tool's panel is confirmed 'PAINT ALONG PATH' in a captured frame (same as this creator's slipper video) — per references/version-tracker.md this pins the tutorial to the Painter 9.x-10.x window, before the 11.0.0 rename to Filled Path"
tags: [layers, fill-layer, paint-layer, masks, generator, anchor-point, blend-mode, alpha, procedural, MatFX, texture-set, uv, pbr, metal-rough, basecolor, roughness, metallic, height, normal-map, opacity, ambient-occlusion, mesh-maps, export, export-preset, channel-packing, iray-render, advanced]
extraction_status: complete
frames_dir: tutorials/frames/how-to-create-a-realistic-poison-bottles-material-using-substance-painter/
frame_count: 10
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# How to Create a Realistic Poison Bottles Material Using Substance Painter

**Source:** [YouTube](https://www.youtube.com/watch?v=386o64sxSpw)
**Author:** 3DRedBox
**Duration:** 28m6s | 5 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Do you have asset or prop that you want to texture inside Substance Painter?
[0:15] And in that asset, you have glass material, I will show you how to create glass material
[0:20] inside Substance Painter and render it in other engines like Marmoset Toolbag.
[0:27] For this tutorial, I used some pre-made alpha from our collection that you can find the
[0:33] link in the description and you can download the 3D model, the brush preset and the brush
[0:40] tool and the smart material that I am going to use in this tutorial with the link in the
[0:46] description.
[0:47] So, follow the description, it's so important.
[0:50] And before jumping to the video itself, let me introduce you the brand new course that
[0:55] we release for Substance Painter.
[0:59] Learning Substance Painter is easier than ever.
[1:02] Hey all Substance Lovers, Tech Change Seekers and awesome future artists, welcome to ultimate
[1:08] course for learning Substance Painter from zero to hero.
[1:18] Ready to learn how to texture with different projects?
[1:21] Substance Master released a brand new course for those who want to learn to texture with
[1:27] Substance Painter.
[1:28] In this course, we cover from preparing the model to rendering different projects, different
[1:34] challenges.
[1:35] If you want to level up your skill in texturing, come and check the Substance Master Ultimate
[1:39] course for learning Substance Painter.


### Glass Shader [1:42]
**Transcript (timestamped):**
[1:42] Okay, so how to create glass shader inside Substance Painter?
[1:48] It's super simple.
[1:49] So for this model, I just want to create glass shader for the body and for the top and down,
[1:58] let's go for the metal, just for now.
[2:01] And we are going to add all the details after creating the basic information inside Painter
[2:07] and export it to Marms Toolbag and set up the shader over there.
[2:12] Okay, we need to go to the shader and be sure you select ASM Metal Rough shader in here
[2:22] and after that, just scroll down and enable translucency and we can enable absorption if
[2:30] we want to set the color inside Substance Painter, not in Marms or any other engine that
[2:37] we are going to use.
[2:39] So after setting up this translucency and absorption, we need to add the data channel to our project.
[2:49] So let's go to the texture setting and in the channel, we just need to add absorption
[2:55] color and in here translucency.
[3:00] And I just add ambient occlusion here because we are going to add details in the future.
[3:07] We are done in the setting and now let's create the basic information for each part of the
[3:12] model.
[3:13] So I'm going to create two folder, one for glass and one for metal section.
[3:22] And in the glass, I just want to put a single fill layer and call it glass.
[3:30] And in here, I'm going to turn on translucency and as you can see, we have the glass.
[3:38] Shader inside the viewport and let's bring down the roughness and boom, we have the glass.
[3:46] Okay.
[3:48] And let's add a black mask, go to the paint and select the middle part in here.
[3:56] That's great.
[3:58] And for the metal section, let's select these parts and now let's add something like bronze
[4:08] armor.
[4:10] Okay.
[4:12] That's great.
[4:15] And I'm going to export the textures and set up the shader inside.
[4:21] Marms the tool bank.
[4:22] So let's go here to the file, export texture, set the path and in output template, I'm going
[4:30] to select document channel plus normal plus AO.
[4:34] It means we are going to export all the channels that we set inside the texture set setting.
[4:42] Okay.
[4:43] So let's select it and the PNG is good.
[4:47] We can go for the 16 bits.
[4:49] It doesn't matter.
[4:51] I'm going to export it 4k and let's export and set up the shader inside Marms.
[4:56] Okay.
[4:57] Now we are in Marms the tool back.
[4:59] I just import the model and select the sky, increase the brightness, nothing too fancy
[5:05] and ray tracing feature should be on for the glass material inside Marms.
[5:12] Let's create the glass and I can create the glass material from here.
[5:18] Just easy.
[5:19] Okay.
[5:20] So we want to have something like the pure glass model in the top and the bottom section.
[5:27] We have different type of surface.
[5:29] For example, here we have the metal, but in other cases, maybe it's wood or any other
[5:35] type of surfaces.
[5:37] And now it's time to create the shader with the glass feature inside Marms with the textures
[5:45] that we exported already from Substance Painter.
[5:48] Okay.
[5:49] And now let's go here, select the glass and in the Albedo, we need to load the base color.
[5:58] In the roughness, we need to load the roughness.
[6:02] And in here, in the reflectivity, we need to load the metallic into the metalness map.
[6:12] Okay.
[6:13] That's it.
[6:14] And in transmission, in the mask, we need to load the translucency mask.
[6:21] Okay.
[6:23] Now we have the glass shader in the middle part and the metal shader in the top and the
[6:30] bottom part.
[6:31] Okay.
[6:32] And let's go for loading, I don't know, the normal map.
[6:38] Let's check the flip why because we have the direct X normal format.
[6:44] And in the ambient occlusion, we just load the mix AO and that's it.
[6:55] And what about the absorption color?
[6:58] We can use absorption color in here, in the depth map, or we can leave it and select the
[7:05] color inside the base color because we have this feature, use Albedo.
[7:11] Okay.
[7:12] Now we are done.
[7:14] Inside Marmoset, we just set up the shader and put all the mask and texture into the
[7:22] right slot.
[7:23] And now it's time to going back to Substance Painter and create the details and the textures
[7:30] that we want and bring it back inside Marmoset and render it.
[7:35] Let's do that.
[7:37] Okay now it's time to create the details inside Substance Painter and creating a beautiful
[7:44] design with the pre-made alpha and alpha that we already have inside the Substance Painter.
[7:52] And let's do that.
[7:53] So I'm going to skip all the repetitive parts.
[7:57] For the first section, I'm going to create a fill layer and call it ornament number
[8:04] one.
[8:05] Okay.
[8:08] And let's just keep the height and let's add a black mask and for the height, I'm going
[8:14] to set something like 0.5 and in the mask, let's go and add a fill layer and let's load
[8:24] one of the alpha that I previously added to the project and let's go to the 2D and 3D.
[8:34] Okay and let's bring down the size and put it on the location that we want.
[8:44] For example here, it's good.
[8:49] Now we are going to remove all the unnecessary part here and how we are going to do that.
[8:58] For example, we have other UV island here so I can go here and add paint and just select
[9:09] all the UV islands and deselect the UV island that I need and change the blending mode to
[9:18] subtract and in this way, as we can see, we just have the alpha here on this UV island
[9:28] because in the next one, we just subtract all the other parts from the whole texture.
[9:36] Okay.
[9:37] Now let's go back to the fill and change the UV wrap to repeat vertically and now we have
[9:45] this one.
[9:46] Okay.
[9:47] That's great.
[9:50] Let's bring it down a little because I need some small dots in the top part and the bottom
[9:58] part here.
[10:00] Okay.
[10:02] Like this.
[10:03] Okay.
[10:04] Now it's time to add another fill layer here and load the shape alpha and just change the
[10:11] UV wrap to repeat vertically and bring down the size and put it in the right position.
[10:24] Okay.
[10:27] Like this and we can play with the hardness and let's add a level here and bring up this
[10:35] slider.
[10:37] Okay.
[10:38] As you can see, we can define the space between each dot.
[10:43] Okay.
[10:44] And we have a nicer shape on this alpha too.
[10:49] That's great.
[10:53] And this is the workflow that I'm going to follow and we can add a filter like player
[11:00] and put it on value like 15.
[11:07] Okay.
[11:09] That's great.
[11:10] And I'm going to pause the video, add all the details with this technique and we can
[11:16] continue after that.
[11:18] Okay.
[11:19] Now I'm done with this part, adding details in three different layers.
[11:25] So let's check it.
[11:27] The first one is like adding all the details here and as you can see, I just follow the
[11:35] exactly same method that I show you before and for the second layer, it's so similar.
[11:45] As you can see, we have a paint layer to control which UV island should be show the details.
[11:52] Okay.
[11:53] Like this.
[11:55] I just simply use the trim ornament alpha from our collection to add the details here.
[12:04] And for the third one, I just follow the same, but in the last detail, I mean this one, I
[12:15] just change the projection to cylindrical to have the seamless transition between this
[12:23] to UV island.
[12:24] Okay.
[12:25] So now I can control it.
[12:29] As you can see, like this.


### Adding Filters [12:31]
**Transcript (timestamped):**
[12:31] Okay.
[12:32] The normal effect that we have already, it's not so strong and enough for me.
[12:40] So I'm going to add a paint layer here and let's call it filter, change the blending
[12:47] mode to pass through and apply it to all channel.
[12:50] I'm going to add filter here and let's load height to normal filter.
[12:57] Okay.
[12:58] As you can see, I have a stronger normal intensity and I want to control that.
[13:05] So let's keep just the normal channel and turn up the use word units.
[13:12] So I have a single slider called normal intensity and I can increase or decrease the intensity
[13:20] of the normal.
[13:21] So let's go for the five.
[13:23] I think five is good and enough.
[13:26] Okay.
[13:27] The next filter that I'm going to add here is Matefix HPAO.
[13:34] Okay.
[13:37] It's like creating AO from the all the details that we add inside the height and normal at
[13:45] the same time.
[13:46] Okay.
[13:47] So let's keep just AO here and I'm going to change the height depth.
[13:56] Okay.
[13:58] To something like this.
[14:01] That's great.
[14:02] So we have the normal, we have the height, we have the AO and everything that we need.
[14:09] And for the last filter, let's add the shark and filter and we want that in the color,
[14:17] roughness and middle.
[14:19] Okay.
[14:20] And let's bring it to 0.5 and that's enough for the filter.
[14:27] Okay.
[14:28] So let's add the other details in here on the glass body.
[14:34] And for this purpose, I'm going to create another ornament layer here.
[14:41] Let's add a black mask.
[14:42] Go here and keep height.
[14:45] Bring it up to something like 0.5 and in here, I'm going to add a paint layer.
[14:55] And now it's time to load the brush preset that I created for you and you can download
[15:02] it from the link in the description.
[15:05] After downloaded, you just need to import them to the library.
[15:10] One of them is the 3D Red Box Path Alpha Roll.
[15:16] It's a brush preset for the pass tool.
[15:20] And the other one is 3D Red Box Dynamic and it's a base material.
[15:25] So let's import it to the project.
[15:27] And now in the paint layer, I go to the pass tool and double click it and everything is
[15:34] okay.
[15:35] So we just need to load this 3D Red Box Dynamic to the grayscale area and now we can load
[15:44] any alpha that we want here and we can use it as a roll brush.
[15:50] And now it's time to use it.
[15:52] And let's use this alpha here.
[15:55] Okay.
[15:56] And I'm going to create the brush here like this.
[16:02] Okay.
[16:03] Let's change the size to something like 50 and I think it's too big.
[16:11] So let's decrease the size to 40 and I think it's okay.
[16:19] Maybe 30 is much better.
[16:23] Yeah.
[16:24] And we can change the pressure from the upside.
[16:29] Okay.
[16:31] That's so much better.
[16:36] Okay.
[16:39] That's great.
[16:41] And let's go to the symmetry option.
[16:45] Change it to radial symmetry.
[16:48] Okay.
[16:50] And let's go for the mirror Y.
[16:55] And I think we can increase the angle span and maybe count.
[17:03] Yeah.
[17:05] Seven is good because we have the match with this ornament here.
[17:14] Okay.
[17:15] That's great.
[17:16] We just create the detail that we want here and let's go to the next one.
[17:25] Okay.
[17:26] Let's add another paint layer.
[17:30] I'm going to load another alpha here and let's create the detail that we want.
[17:43] Change the blending mode to linear dodge.
[17:46] Okay.
[17:48] That's great.
[17:50] And I'm going to fill this side.
[18:13] Now we need to polish the result.
[18:16] And the first one is add the paint layer, change the blending mode to subtract and go
[18:23] to the polygon field, use UV Chong, turn off the symmetry and select all the UV islands
[18:31] and press X, select the UV island that we need.
[18:36] Okay.
[18:37] And in this way, you just control the result.
[18:41] That's great.
[18:43] And now it's time to remove the intersection here.
[18:48] And how we are going to do that, okay, it's related to the ornament number two.
[18:55] We just add anchor point here and come back here to ornament number four and add a fill
[19:02] layer and load the anchor point ornament number two mask.
[19:08] Okay.
[19:10] Let's go back here.
[19:11] Let's go back to the keep alpha and bring up the slider.
[19:16] That's great.
[19:17] And change the blending mode to subtract and now it's fixed.
[19:22] Okay.
[19:23] That's great.
[19:24] And as you can see, we don't have any intersection here right now.
[19:31] That's great.
[19:32] Okay.
[19:34] Actually we are done in a detail part.
[19:37] So we can skip and go to the material creation part.


### Adding Glass [19:41]
**Transcript (timestamped):**
[19:41] Okay.
[19:42] Now let's focus on the glass.
[19:44] And if I turn on the glass folder and as you can see, there is no sign of the details
[19:50] on the glass part.
[19:51] So we need to subtract all the mask that we create from the mask on the glass folder.
[20:00] So how we can do that?
[20:03] Let's add anchor point on each layer like this.
[20:10] Okay.
[20:13] Go back here.
[20:16] We have four different layers.
[20:18] So let's duplicate four different fill layer and change the blending mode to subtract for
[20:26] all of them.
[20:28] Okay.
[20:30] Like this.
[20:32] And in the first one, let's load the ornament mask number one, ornament mask number two,
[20:41] number three, and number four.
[20:45] Okay.
[20:46] Like this.
[20:48] And we need to bring up these sliders.
[20:51] Okay.
[20:53] Like this.
[20:57] And as you can see, we have the white part top on the glass part.
[21:12] Okay.
[21:13] That's great.
[21:15] And we can continue our way on the glass material.
[21:20] And for the glass, let's pick a dark gray color.
[21:25] Okay.
[21:26] We can turn off the absorption color.
[21:32] Okay.
[21:34] Let's remove absorption color here.
[21:38] Let's add a fill layer.
[21:40] And I'm going to call it color variation.
[21:43] Let's keep color and roughness.
[21:45] For the roughness, let's pick the amount like 0.05.
[21:53] And for the color, let's go for the dark.
[21:56] Okay.
[21:57] And I'm going to add a black mask, add generator here, and 3D linear.
[22:05] Okay.
[22:06] I can invert it.
[22:09] Okay.
[22:10] That's great.
[22:12] We couldn't see inside the substance painter viewport, but we are going to get the same
[22:21] color transition on the marble set.
[22:24] Okay.
[22:25] That's great.
[22:27] And let's add another layer.
[22:30] I'm going to call it roughness variation.
[22:35] And let's add a black mask.
[22:37] Go to the fill and search about the fingerprint.
[22:42] Okay.
[22:43] Something like this.
[22:46] It could be great.
[22:51] Bring up the tiling amount.
[22:55] That's great.
[22:57] Okay.
[22:58] We can go back to the grunge and play with the balance.
[23:05] That's great.
[23:07] And let's keep just roughness.
[23:10] And yeah, that's it.
[23:12] We can change the grunge here to something like this.
[23:18] It should be better.
[23:21] Okay.
[23:22] Yeah.
[23:23] Yeah.
[23:24] That's so much perfect.
[23:27] And yeah, that's it.
[23:30] Let's go and add the final layer here.
[23:37] And I'm going to call it scratches.
[23:41] Let's add a black mask.
[23:43] Go here and search about the scratches.
[23:48] Okay.
[23:49] We have the scratches here.
[23:53] So let's bring up the tiling.
[23:57] And after that, let's decrease the balance.
[24:01] Okay.
[24:02] Maybe lower.
[24:05] That's great.
[24:07] And go back here.
[24:10] You just need to have negative height, small amount, and roughness, maybe 0.5.
[24:20] And we have the imperfection on the surface.
[24:25] And that's enough for the glass.
[24:27] Okay.


### Adding Metal [24:28]
**Transcript (timestamped):**
[24:28] Now, for the metal section, I will give you in a smart material that you can import it
[24:34] to your folder.
[24:37] And it's working.
[24:39] But we need to set up a small step to work perfectly with your project.
[24:45] The first one is to select this area for the metal folder, because we need to have color
[24:54] on these details too.
[24:57] And it's kind of hard and useful to add all the mask again here and add to the mask that
[25:06] we have.
[25:07] So we simply add the whole area and it's much better.
[25:13] And after that, we need to create a paint layer here and call it ornament plus and change
[25:20] the blending mode to pass through and apply to all channels.
[25:24] And we can add an anchor point to ornament plus.
[25:29] And this layer is going to collect all the data from the previous layers.
[25:35] And we can use that data inside the material that we have.
[25:41] So let's do that.
[25:43] I'm going to turn off all the layers and let's...
[25:46] Okay, that's fine.
[25:48] Let's go and turn on the oxidation and let's go to the generator.
[25:54] And in the macro height, we are going to load the ornament plus and change the reference
[26:01] channel to hide.
[26:03] And now we have the effect on the dirt.
[26:07] And let's go to the edge worn.
[26:11] Let's go to the metal edge and come here and again load the ornament plus and reference
[26:19] it to the hide channel.
[26:21] And I'm going to do that for the all generator that we have here.
[26:28] And this is the final result after setting up all the generator and connected to the
[26:33] ornament plus anchor point.
[26:36] And I think that's enough.
[26:38] And we can export the textures and see what we have inside the Marmoset.
[26:45] Okay, now we are in Marmoset tool bag.
[26:49] And as you can see, everything is working probably except glass.
[26:55] And in the glass section, if you get this kind of dark and non-glass effect, you need
[27:02] to bring the color to white, near to white in the substance painter.
[27:10] And after that, you can go to the transmission and increase the depth.
[27:16] And as you can see, we have the glass inside the Marmoset and it's working well.
[27:23] If I duplicate this model and bring it back, as you can see, we can see through the glass
[27:31] and everything works properly.
[27:34] And that's it.
[27:36] We are done.
[27:37] And it's enough for this tutorial.
[27:39] I hope you learned something new here.
[27:42] And if you like this video, please hit the like button.
[27:47] And don't forget to go to the Substance Master website and see the course and the other stuff
[27:54] over there.
[27:55] You can download all the necessary files inside the description and you can read the description
[28:02] to learn more information.
[28:04] Be creative.
[28:05] Bye.



---

## Captured Frames

- [2:12] tutorials/frames/how-to-create-a-realistic-poison-bottles-material-using-substance-painter/frame_000.jpg
- [3:00] tutorials/frames/how-to-create-a-realistic-poison-bottles-material-using-substance-painter/frame_001.jpg
- [5:49] tutorials/frames/how-to-create-a-realistic-poison-bottles-material-using-substance-painter/frame_002.jpg
- [9:09] tutorials/frames/how-to-create-a-realistic-poison-bottles-material-using-substance-painter/frame_003.jpg
- [12:57] tutorials/frames/how-to-create-a-realistic-poison-bottles-material-using-substance-painter/frame_004.jpg
- [13:34] tutorials/frames/how-to-create-a-realistic-poison-bottles-material-using-substance-painter/frame_005.jpg
- [16:45] tutorials/frames/how-to-create-a-realistic-poison-bottles-material-using-substance-painter/frame_006.jpg
- [19:02] tutorials/frames/how-to-create-a-realistic-poison-bottles-material-using-substance-painter/frame_007.jpg
- [20:53] tutorials/frames/how-to-create-a-realistic-poison-bottles-material-using-substance-painter/frame_008.jpg
- [26:01] tutorials/frames/how-to-create-a-realistic-poison-bottles-material-using-substance-painter/frame_009.jpg

---

## Structured Notes

### Core Technique
Glass-bottle texturing built around a Painter-side Translucency/Absorption-channel glass shader, a Marmoset Toolbag glass-material handoff, ornate ornament detail built from alphas and a custom Pass-tool brush with radial symmetry, and anchor-point-driven mask reuse across folders (metal generators referencing height data collected from the ornament layers, and the glass folder subtracting all four ornament masks so glass and metal read as one continuous carved surface).

### Summary
Starts by establishing the base glass/metal split before any detail work: switch the shader to `PBR Metal Roughness`, enable `Translucency` and `Absorption`, add the `Absorption Color`, `Translucency`, and `Ambient Occlusion` channels via Texture Set Settings, then build two single-fill-layer base materials (a Translucency-enabled `Glass` fill for the body, a `Bronze Armor`-based `Metal` folder for the neck/base) masked by paint selection. Exports a first pass (Document Channels + Normal + AO, PNG, 4K) purely to prototype the glass shader in Marmoset Toolbag: wiring Base Color→Albedo, Roughness→Roughness, Metallic→Metalness/Reflectivity, Translucency→Transmission mask, Normal (Y-flipped for DirectX), and AO→Ambient Occlusion, with Ray Tracing enabled for the glass to render correctly. Returns to Painter to build the actual ornamental detail: four numbered "ornament" fill/paint layers, each Height-only, masked by pre-made alphas positioned in the 2D/3D view and isolated to specific UV islands via a Paint layer using `Subtract` blend and manual island deselection; the third ornament switches its Fill projection to `Cylindrical` for a seamless wrap across a UV seam. A Pass-Through `Filter` layer stacks `Height to Normal` (World Units off, Normal Intensity ~5), `MatFX HBAO` (AO-only, generates ambient occlusion directly from the height/normal detail just painted), and a final `Sharpen` filter (Color/Roughness/Metal, ~0.5). A fourth ornament layer is hand-painted using the creator's own downloadable Pass-tool brush preset (`3D Red Box Path Alpha Roll`, loading `3D Red Box Dynamic` into the grayscale slot) with Radial Symmetry (Mirror Y, angle-span/count tuned to match the existing ornament, count 7). Overlap/intersection between ornament layers is cleaned up by anchor-pointing each ornament's mask and cross-referencing it as a Subtract layer in the others. The glass folder — which shows none of this ornament detail by default since it's a separate folder — gets four Subtract-blended Fill sublayers, each loading one ornament's anchor point, so the etched pattern reads through the glass too. Glass material finishing: dark-grey base with Absorption Color removed (color handled directly instead), a `3D Linear`-generator-masked color-variation layer (a gradient invisible in Painter's own viewport but visible once rendered in Marmoset), a fingerprint-alpha-driven roughness-variation layer, and a scratches layer (small negative height, ~0.5 roughness). The metal material is built from an imported smart material, whose mask is expanded to cover the full metal folder area (so ornament color reads on the metal too), then wired to a new Pass-Through `Ornament Plus` paint layer (anchor-pointed) that collects all the ornament height data — every relevant generator inside the metal smart material (oxidation dirt, edge wear, etc.) has its Image Input reference switched to load the `Ornament Plus` anchor point on the Height reference channel, so the metal's procedural wear responds directly to the carved ornament geometry. Finishes with a second Marmoset pass, including a troubleshooting note: if glass renders dark/opaque instead of clear, set its Base Color near-white in Painter and increase Transmission Depth in Marmoset.

### Key Steps
1. **Set up the glass shader in Painter first, before any detail work:** switch shader preset to `PBR Metal Roughness` (ASM), scroll down and enable `Translucency` (and optionally `Absorption` if color should be set in Painter rather than the render engine); add `Absorption Color`, `Translucency`, and `Ambient Occlusion` channels via Texture Set Settings.
2. **Build minimal base materials in two folders:** a single `Glass` fill layer (Translucency on, Roughness lowered) masked to the body by paint selection; a `Bronze Armor`-style `Metal` folder for the neck/base caps.
3. **Export a prototyping pass and build the glass shader in Marmoset Toolbag:** Export Textures with output template `Document Channels + Normal + AO`, PNG, 4K; in Marmoset enable Ray Tracing (required for correct glass), create a Glass material, and wire Base Color→Albedo, Roughness→Roughness, Metallic→Metalness/Reflectivity, Translucency mask→Transmission, Normal (Y-flip for DirectX format), Mixed AO→Ambient Occlusion, with Absorption Color optionally routed to the Depth map or skipped in favor of `Use Albedo`.
4. **Build ornament detail as a series of numbered Height-only fill/paint layers**, each masked by a pre-made alpha positioned via the 2D/3D view; isolate each ornament to the correct UV island using a `Paint` sublayer with `Subtract` blend (select all UV islands with Polygon Fill, then deselect/re-select the target island).
5. **Use `Cylindrical` projection instead of the default UV projection** on the third ornament layer specifically to get a seamless wrap across a UV seam that the default projection couldn't hide.
6. **Boost and consolidate the detail with a Pass-Through `Filter` layer** (applied to all channels): `Height to Normal` (Use World Units off, Normal Intensity tuned to ~5 for a stronger read than the raw height data alone), `MatFX HBAO` (AO channel only, height depth tuned) to generate believable ambient occlusion directly from the just-added height/normal detail rather than relying only on baked mesh-map AO, and a `Sharpen` filter applied to Color/Roughness/Metal (~0.5).
7. **Hand-paint the final ornament with a custom Pass-tool brush and radial symmetry:** import the creator's downloadable brush preset (`3D Red Box Path Alpha Roll` for the Pass tool, `3D Red Box Dynamic` loaded into the grayscale slot as the base), pick an alpha, tune brush size down from 50→40→30 and pressure falloff, switch Symmetry to `Radial Symmetry` with `Mirror Y`, and tune Angle Span/Count (7) to match the existing ornament's repeat rhythm.
8. **Clean up overlapping ornament intersections with anchor-point cross-referencing:** add an Anchor Point to an earlier ornament's mask (e.g. ornament #2), then in a later ornament (#4) add a new Fill sublayer loading that anchor point, raise its slider, and set the sublayer's blend mode to `Subtract` — removes the unwanted overlap without repainting either mask by hand.
9. **Propagate the ornament pattern into the glass folder via anchor points:** since the Glass folder is a separate mask/folder and shows none of the ornament detail by default, add four `Subtract`-blended Fill sublayers to the glass folder's mask, one per ornament, each loading that ornament's anchor point and its slider raised — makes the etched ornament pattern read through the glass material too, not just the metal.
10. **Finish the glass material:** pick a dark grey base color, remove/disable the Absorption Color channel on this layer (color handled via Base Color directly instead); add a `Color Variation` fill (Color + Roughness only, roughness ~0.05, dark color, black mask + `3D Linear` generator, inverted) — explicitly noted as invisible in Painter's own viewport but visible once rendered in Marmoset; add a `Roughness Variation` fill (Roughness only) masked by a fingerprint alpha (tiling raised) plus a grunge fill for extra breakup; add a `Scratches` layer (small negative Height, Roughness ~0.5) masked by a scratches alpha (tiling raised, balance lowered).
11. **Finish the metal material starting from an imported smart material:** first expand the metal folder's mask to cover the full intended area (needed so ornament coloring reads correctly on the metal, not just the smart material's own default mask); add a Pass-Through `Ornament Plus` paint layer (applied to all channels, anchor-pointed) purely to collect the combined height data from all the ornament layers already built.
12. **Rewire every relevant generator inside the imported metal smart material to read from the ornament geometry:** for each generator (oxidation/dirt, metal edge wear, etc.), open its Micro Details / Image Inputs section and load the `Ornament Plus` anchor point, setting its Reference Channel to `Height` — makes the smart material's built-in wear/dirt patterns respond to the actual carved detail instead of only the base mesh curvature/AO.
13. **Re-export and verify in Marmoset**, with a specific glass troubleshooting fix: if the glass renders dark/opaque rather than clear, set its Base Color to near-white back in Painter, then increase the Transmission Depth setting in Marmoset.

### Layers / Tools / Settings
- **Shader:** `PBR Metal Roughness` (ASM Metal Rough) with `Translucency` and `Absorption` enabled
- **Channels added via Texture Set Settings:** `Absorption Color`, `Translucency`, `Ambient Occlusion`
- **Smart material used:** an imported metal smart material (name not stated; generators rewired to reference the `Ornament Plus` anchor point), base metal starts from `Bronze Armor`
- **External brush/tool assets used:** `3D Red Box Path Alpha Roll` (Pass-tool brush preset), `3D Red Box Dynamic` (grayscale base material for that brush), plus several pre-made ornament alphas
- **Filters used:** `Height to Normal` (World Units off, Intensity ~5), `MatFX HBAO` (AO-only), `Sharpen` (Color/Roughness/Metal, ~0.5)
- **Generator used:** `3D Linear` (glass color-variation mask, inverted)
- **Fills/alphas used:** fingerprint alpha (roughness variation), grunge (roughness breakup), scratches alpha (glass imperfections)
- **Projection technique:** one ornament layer's Fill `Projection` switched to `Cylindrical` specifically to hide a UV seam
- **Blend modes used:** `Subtract` (UV-island isolation, ornament-intersection cleanup, glass-folder ornament propagation), `Linear Dodge` (mentioned as an alternative combine option), `Pass Through` (Filter layer, Ornament Plus collector layer)
- **Anchor Point usage (this video's throughline):** one per ornament layer's mask (referenced for intersection cleanup between ornaments and for propagating the pattern into the separate Glass folder), plus one `Ornament Plus` anchor point on a dedicated Pass-Through collector layer, referenced by every generator inside the metal smart material via their Image Inputs / Reference Channel = Height
- **Pass tool (Paint Along Path):** Radial Symmetry mode, Mirror Y, tuned Angle Span and Count (7) to match existing ornament rhythm
- **Export settings:** output template `Document Channels + Normal + AO`, PNG (16-bit optional), 4K
- **Marmoset Toolbag wiring:** Albedo=Base Color, Roughness=Roughness, Metalness/Reflectivity=Metallic, Transmission mask=Translucency, Normal (Y-flip for DirectX), Ambient Occlusion=Mixed AO, Ray Tracing enabled for glass; troubleshooting: near-white Base Color + increased Transmission Depth fixes dark/opaque glass

### Difficulty
Advanced — the core layer-building (ornament alphas, filters) is approachable, but the anchor-point cross-referencing across separate folders (Glass folder subtracting all four Metal-side ornament masks) and rewiring a smart material's internal generators to reference an external anchor point via Reference Channel = Height are genuinely advanced, non-obvious techniques; the glass shader also requires a two-application (Painter + Marmoset) mental model, not just Painter-side knowledge.

### App & Version
Substance 3D Painter — version not stated on screen. The Pass tool's properties panel is confirmed titled `PAINT ALONG PATH` in a captured frame, matching this same creator's slipper video. Per `references/version-tracker.md`, this tool name was only used from Painter 9.0.0 until its 11.0.0 rename to Filled Path — pinning this tutorial to the same Painter 9.x-10.x window as the creator's other videos using this tool.

### Tags
layers, fill-layer, paint-layer, masks, generator, anchor-point, blend-mode, alpha, procedural, MatFX, texture-set, uv, pbr, metal-rough, basecolor, roughness, metallic, height, normal-map, opacity, ambient-occlusion, mesh-maps, export, export-preset, channel-packing, iray-render, advanced

---

## Related Tutorials
- [How to texture a realistic slipper model](how-to-texture-a-realistic-slipper-model.md) — same creator (3DRedBox); both confirmed via the "PAINT ALONG PATH" panel to date from the same Painter 9.x-10.x window, and both use anchor-point-referenced placeholder/collector layers as reusable mask sources.
- [Texturing a Black Suit in Substance Painter](texturing-a-black-suit-in-substance-painter.md) — same creator; shares the Painter-to-Marmoset-Toolbag export/render handoff pattern and channel-packed texture wiring.
- [Texturing a Worn Wooden Stool in Substance Painter](texturing-a-worn-wooden-stool-in-substance-painter.md) — same creator; shares the Pass-Through "collector" layer pattern (Ornament Plus here, Edge Plus there) used to feed height/AO data into downstream generators via anchor points.
- [Texturing Women's Shorts with Lace Trim in Substance Painter](texturing-womens-shorts-with-lace-trim-in-substance-painter.md) — same creator; shares the Pass-Through Height-to-Normal effect-layer pattern for boosting normal intensity beyond what raw height data alone produces.
- [Speed Up Your Substance Painter Workflow with This Easy Trick!](speed-up-your-substance-painter-workflow-with-this-easy-trick.md) — same creator; also uses the Pass tool (Paint Along Path) with a custom brush preset for detail work, and shares this creator's habit of explaining a purchased smart material's internal labeled-layer structure before modifying it.
- [How to Texture NavyCap In Substance Painter in English](how-to-texture-navycap-in-substance-painter-in-english.md) — same creator; shares the anchor-point mask-reuse-across-folders pattern (a Pass-Through collector layer there, direct multi-anchor Soft-Track combination here).
