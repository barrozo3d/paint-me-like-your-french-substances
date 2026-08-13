---
title: Realistic Wood in Substance Painter | M24 Grenade Texturing
source: YouTube
url: https://www.youtube.com/watch?v=I3v-ESX4DxQ
author: Dolinskyi
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/realistic-wood-in-substance-painter-m24-grenade-texturing/
frame_count: 0
frame_status: pending-selection
---

# Realistic Wood in Substance Painter | M24 Grenade Texturing

**Source:** [YouTube](https://www.youtube.com/watch?v=I3v-ESX4DxQ)
**Author:** Dolinskyi
**Duration:** 17m55s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py realistic-wood-in-substance-painter-m24-grenade-texturing <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


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

## Structured Notes

### Core Technique
[PENDING EXTRACTION]

### Summary
[PENDING EXTRACTION]

### Key Steps
[PENDING EXTRACTION]

### Layers / Tools / Settings
[PENDING EXTRACTION]

### Difficulty
[PENDING EXTRACTION]

### App & Version
[PENDING EXTRACTION]

### Tags
[PENDING EXTRACTION]

---

## Related Tutorials
[PENDING EXTRACTION]
