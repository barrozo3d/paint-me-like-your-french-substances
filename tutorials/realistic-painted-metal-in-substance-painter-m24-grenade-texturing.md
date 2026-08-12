---
title: Realistic Painted Metal in Substance Painter | M24 Grenade Texturing
source: YouTube
url: https://www.youtube.com/watch?v=SAI-lrWrtKg
author: Dolinskyi
ingested: 2026-08-12
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/realistic-painted-metal-in-substance-painter-m24-grenade-texturing/
frame_count: 0
frame_status: pending-selection
---

# Realistic Painted Metal in Substance Painter | M24 Grenade Texturing

**Source:** [YouTube](https://www.youtube.com/watch?v=SAI-lrWrtKg)
**Author:** Dolinskyi
**Duration:** 16m33s | 8 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py realistic-painted-metal-in-substance-painter-m24-grenade-texturing <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Introduction [0:00]
**Transcript (timestamped):**
[0:00] Welcome to part 2 of our M24 Steel Hand Granite Texturing Series.
[0:16] And for those who haven't watched the first part yet, please do so, because I will use
[0:20] some techniques that I explained there.
[0:22] If any part of the process seems unclear, you can open the project itself and inspect
[0:27] every single layer.
[0:29] All project materials are available on my ArtStation page, including the Substance Painter project
[0:34] file, stencils, and the textures I used.
[0:37] It's like having the final answer key to the tutorial.
[0:40] Today we're tackling painted metal.
[0:42] This stage is more complex and involves several key techniques and a solid understanding of
[0:47] the PBR workflow.
[0:48] I'll break it all down step by step in simple terms.


### Paint [0:51]
**Transcript (timestamped):**
[0:52] Well, I'll start demonstrating the layers in the order I created them.
[0:56] First of all, I created paint.
[0:58] Turning on paint, and the first layer in this folder is just a fill, a dark green color.
[1:03] Roughness at 42, metallic at 0, because it's not metal.
[1:06] And this will be the base, which I will then apply in variation 1, 2, 3, 4, and all subsequent
[1:12] variations.
[1:14] I create variations in the following way.
[1:16] I duplicate this base layer.
[1:18] For example, I write that this is paint variation 01.
[1:21] I add a mask here, a fill layer, and in the fill layer, I insert for example some procedural
[1:27] texture.
[1:28] And now I just change their color.
[1:30] For example, I'll make it a little light yellow.
[1:33] This in essence will be the variation.
[1:35] This is exactly how I create all these subsequent layers.
[1:39] But I tweak not only the color, I also tweak roughness and height.
[1:43] Height variations are very important.
[1:46] This grenade is quite old.
[1:47] It has been lying around since World War II.
[1:50] If you look at photos, there are a lot of different imperfections, damages, scratches.
[1:55] The paint is not as sharp as they paint it now.
[1:58] That is, such things, old vintage objects, weapons have a very saturated height map.
[2:03] That is, it's not worth leaving such a simple surface.
[2:06] It will look unrealistic.
[2:07] So the first layer with the variation is these kinds of stripes.
[2:11] These are paint application marks.
[2:13] I add a base procedural texture, crystal 2, then blur it, then a warp filter, which gives
[2:18] a bit of life to these lines.
[2:20] With a histogram scan, I make the mask more contrasty and readable.
[2:24] We must remember that we will be looking from this distance.
[2:27] Thin, indistinct lines simply won't be visible.
[2:31] Next, I remove the uniformity.
[2:33] I add the next fill layer, insert a grunge map here and through the subtract blending
[2:37] mode.
[2:38] Next, with paint, I clean up those details where I don't want to see the mask.
[2:42] I also add an ambient occlusion generator, which also cleans up the mask where I don't
[2:47] want to see it.
[2:49] And this is how such a layer appears.
[2:51] It is darker in diffuse.
[2:53] That is, it's such a dark green color.
[2:55] Its roughness is slightly different and it has height.
[2:59] The next layer is very similar.
[3:02] In essence, the same lines, but they are blurred.
[3:04] They are bigger.
[3:06] This adds a bit of a variety.
[3:08] Because in nature, when something is painted or worn down, it cannot be uniform, meaning
[3:14] it needs to be broken up a bit.
[3:16] Somewhere it will be sharp, somewhere it will be blurry, somewhere the lines are wide,
[3:20] somewhere narrow.
[3:22] This non-uniformity is exactly what gives the effect of authenticity.
[3:26] Next layer, variation number three.
[3:29] Also differs in color.
[3:30] It is already a bit yellowish.
[3:33] Roughness is already more matte.
[3:35] Medallness is still zero, because it is still not metal.
[3:38] Next layer.
[3:39] These are already more specific yellow spots, seemingly looking like traces of rust.
[3:45] Such a contrasty dark dark orange or closer to brown color is already even more matte.
[3:50] The next variations are interesting in the sense that they work like a gradient.
[3:55] A gradient adds realism to an object, and such an object reads well from a distance.
[4:01] The layer is very simple.
[4:03] In essence, these are all masks that I take from the procedural textures library of Substance
[4:08] Painter.
[4:09] I use this mask as a stencil.
[4:11] Through the Subtract mode, I subtracted grunge plaster paint from it.
[4:15] Here, it adds such a texture overlay blending mode.
[4:20] The next layer, paint variation 07 simulates paint in the lower part.
[4:25] Such paint can be seen on references, painted simply with a standard brush.
[4:30] Next is white dirt.
[4:31] This is, in essence, white paint matte.
[4:35] This is what the main mask looks like.
[4:37] Next layer, light edges.
[4:39] Light edges adds a bit more volume.
[4:42] Often paint either wears away in contact areas or fades.
[4:47] Created very simply using metal edge wear.
[4:50] In custom grunge, this grunge is added.
[4:53] The next layer is just a variation in glossiness.
[4:56] These are fingerprints.
[4:57] The next folder is micro surface.
[5:00] Micro surface is variations in the height map.
[5:03] The first variation is the unevenness of the paint, made using a standard procedural
[5:08] texture on the height channel.
[5:10] So, the next layer is hair, as if we have a hair stuck under the paint.
[5:14] The hair mask can be found on the textures.com website.
[5:19] It looks pretty cool, especially in renders.
[5:21] Next is scratches.
[5:23] I drew them by hand, projecting them from a scratch mask.
[5:26] Next layer, separation.
[5:28] We have 01 and 02.
[5:30] They separate the details from each other by color.
[5:32] This head is made of three details and they must differ from each other.
[5:36] They cannot just be filled with a single paint.
[5:39] In an empty layer, I add an HSL perspective filter, set the blending mode to pass through.
[5:45] I isolate the needed detail with a mask and change its color.
[5:49] This is for realism.
[5:51] Next folder, metal cap, for the back part.
[5:54] The first layer changes the color of the paint, gives a more bluish tint.
[5:59] This one separates this detail.
[6:01] The next layer adds dust.
[6:03] It is made using a grunge dust white map on top.
[6:10] Dust layer settings, roughness matte, base color gray, slightly with a bluish tint without
[6:15] a height map.
[6:17] The next layer is also a color change based on curvature.
[6:20] We make it of a more gray shade like that.
[6:24] The next layer is a dirt layer.
[6:26] Well, not like dirt, but variations in color on the paint.
[6:30] A dark brown color and slightly different roughness.
[6:38] Next layer dirt, light and dark.
[6:43] This is its mask.
[6:48] Next light dirt made using a generator.
[6:57] Directional noise to give it a bit of direction.
[7:00] Such things look good on cylinders.
[7:02] We add these stripes and clean up with a brush where they are not needed.
[7:07] And right here, I add such spots under the bolts.
[7:10] Yes, and the last layer in this folder is also color variations.
[7:15] Only color, just a gray color.
[7:17] The mask is generated by this kind of generator.
[7:27] Next glossy scratches layer.
[7:29] These are glossy scratches like that, which also add variations.
[7:33] That is, our surface is matte and to make variations on this surface, you need to make them glossy.
[7:39] If our surface were glossy, I would conversely add matte variations.
[7:43] This is everything regarding this part.
[7:45] The next folder in the paint folder is extra details.
[7:49] Extra details are additional variations in the height map and color.
[7:53] Such irregularities that break through the paint.
[7:56] The mask looks like this.
[7:58] It is also created using a standard procedural texture, Rusty Leaks.
[8:02] Next, edges.
[8:04] Such a slight glossy effect.
[8:09] Also ambient occlusion slightly separates this part from the other.
[8:13] That is, in essence, these two layers just make this effect more voluminous.
[8:18] And that's all for the paint.
[8:20] All these layers need to be done very carefully.
[8:23] The main thing in the process of improvement is not to make it worse.
[8:26] Let's now create damages for our paint.
[8:28] This is a very important element.


### Paint Damage [8:31]
**Transcript (timestamped):**
[8:31] And so, the first layer I have is a generator.
[8:33] I want to add uniform wear in some places with the generator, but I will edit it very
[8:37] heavily.
[8:38] Here is the next layer.
[8:39] In essence, these are the main damages.
[8:41] I left damages from the generator only on this detail.
[8:44] I drew all these damages using a stencil.
[8:47] I will add a similar stencil to the pack with source files.
[8:51] You can use it.
[8:52] This is a real photograph of paint damages.
[8:54] We take the stencil and simply paint out these chunks of damaged paint.
[8:59] When painting, take into account such design principles as large, medium, small, that is,
[9:04] you, for example, create one large spot, create a medium spot next to it and add some tiny
[9:08] spots.
[9:09] But the mask must be contrasty so that it reads well from a distance.
[9:13] In this place, I don't have a very contrasty texture, so using blur and a subsequent histogram
[9:18] scan, I make it maximally contrasty and sharp.
[9:26] Next I created corrosion under the paint.


### Oxidized Metal [9:29]
**Transcript (timestamped):**
[9:29] This is what it looks like for me.
[9:34] If you remove paint, it looks like this.
[9:37] Let's show step by step how it was created.
[9:45] The base layer from which everything begins.
[9:48] It is set up as a grey-yellowish metal, roughness at 58 and an important point, metalness at
[9:54] 0.9.
[9:56] It's a light grey mask.
[9:57] It's not completely black because this is one of the basic principles of working with
[10:01] PBR.
[10:02] If you have metal that is not clean but oxidized, it shouldn't be clean metal on the metalness
[10:08] map.
[10:09] That is, you lower this slider a bit and then you can make the map darker.
[10:14] Next, microsurface.
[10:16] Metal is a very important element because this is old metal.
[10:19] It already has its own damages, corrosion, irregularities.
[10:23] Such grenades were made 80 years ago.
[10:25] They have survived until now.
[10:27] And metal cannot be perfectly smooth.
[10:30] Next, oxidized metal.
[10:32] Found a photo of metal on Texture.com, made a tile out of it and generated a normal map
[10:37] using bitmap to material.
[10:40] Also generated roughness, dropped it into base color, into roughness and into normal.
[10:46] This is the metal I have on top.
[10:49] Next rust.
[10:50] As you can see, it is already cut out under a mask.
[10:56] And this, if you turn off the layers, I will make the mask white to show what it looks
[11:03] like.
[11:06] This is a base rust material that can be found in the Substance Painter library.
[11:11] Here it is.
[11:13] But I changed it a bit.
[11:14] In some places I did desaturation.
[11:17] I added an empty layer and inserted an HSL into it.
[11:22] Added this kind of mask.
[11:25] Next, a yellowish layer on top.
[11:31] If you look at the damaged mask, you can see that it is added along the edges.
[11:36] This is also to vary the color of the rust a bit.
[11:39] Next, a dark layer.
[11:44] What does this dark layer represent?
[11:48] This is a fill layer, applied using this kind of mask.
[11:52] This is a standard grunge paint scratched.
[11:55] The mask is set up as oxide, a dark colored metal oxide, matte.
[12:00] And another one on top, a more spotty one like that.
[12:03] This adds contrast.
[12:05] If you look at the base color, it looks like this.
[12:09] Roughness.
[12:11] And metallic.
[12:13] And next, another folder, rust.
[12:19] The rust folder is the last one.
[12:20] It creates corrosion that breaks through the paint.
[12:24] That is, the paint wasn't damaged, but this corrosion ate it away from the inside.
[12:29] That is, a small gap got in somewhere and then the paint started to be eaten away by
[12:33] this corrosion.
[12:38] It was created using a standard procedural map, which is actually called rust.
[12:43] Here is this mask, but its contrast is turned up.
[12:47] That is, in this way.
[12:51] That's all with the corrosion.
[12:53] That is, we already have the paint, we have the corrosion underneath it.
[12:59] The surface still looks quite uniform for such an old thing.
[13:02] I add more information to the height map.
[13:06] Into the layer, I threw again this same height map generated from a photograph that I demonstrated
[13:13] earlier.


### Peeling Paint [13:17]
**Transcript (timestamped):**
[13:17] Next is the peeling paint effect.
[13:20] The first layer is anchor from the mask.
[13:25] The next one is grunge via multiply blending mode.
[13:31] Next is the blur filter to blur the edges.
[13:35] And the last layer is an inverted mask from the anchor via subtract blending mode.
[13:40] This way we get this kind of effect.
[13:44] Next, this layer is located inside a folder to which I added a mask and painted exactly
[13:52] where this effect should be.
[14:02] Let's break down how the decal was created.


### Decal [14:04]
**Transcript (timestamped):**
[14:05] As you can see, there are quite a lot of layers here.
[14:08] You can look into it in detail by opening the project.
[14:10] The link to it is below the video.
[14:12] The first layer is just the alpha of the text created in Photoshop.
[14:17] The next one is filter warp, which makes the edges ragged.
[14:21] Next is blur filter, anchor point, then procedural texture, contrast adjusting using histogram
[14:28] scan.
[14:29] And insert the information from this anchor, place it on top, meaning to remove the internal
[14:34] dots and leave them only along the edges.
[14:37] Then dirt again via multiply, then histogram to increase the contrast.
[14:43] Next is paint.
[14:44] I subtract the peeling paint mask.
[14:48] Grunge to create paint scuff slash wear in some places.
[14:55] Next is another grunge for the same purpose.
[14:58] And anchor point on top.
[15:02] The next layer.
[15:03] We insert the anchor point from the previous layer and add another grunge on top.
[15:08] This is what the final mask looks like.
[15:14] Next we have dirt.


### Dust&Dirt [15:15]
**Transcript (timestamped):**
[15:16] The first layer is grunge.
[15:18] This is from the standard procedural textures.
[15:22] Next is the dirt generator.
[15:24] Next I manually edit the mask.
[15:26] Then using curvature, I remove dirt from the edges.
[15:30] The next layer is fingerprints.
[15:34] I add high contrast spots using a stencil.
[15:44] The next layer, another dirt, but made slightly differently.
[15:48] The first layer is a generator.
[15:50] The next one is grunge via subtract mode.
[15:53] The next one is another grunge via linear dodge mode.
[16:01] Manually painting over the mask.


### Sharpen [16:08]
**Transcript (timestamped):**
[16:09] And as always, sharpen on top.
[16:12] To increase the texture sharpness, there are two sharpen filters here.
[16:17] One for roughness, the second sharpen is for color.
[16:21] That's all.
[16:22] Thank you for watching.
[16:23] You can find the project files via the link below the video.
[16:27] This pack will include stencils for making damaged paint.
[16:30] Thank you for watching.
[16:32] See you next time.



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
