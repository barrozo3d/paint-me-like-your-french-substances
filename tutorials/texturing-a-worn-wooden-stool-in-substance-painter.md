---
title: Texturing a Worn Wooden Stool in Substance Painter 🪑
source: YouTube
url: https://www.youtube.com/watch?v=sa_5vS4s_M0
author: 3DRedBox
ingested: 2026-08-12
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/texturing-a-worn-wooden-stool-in-substance-painter/
frame_count: 0
frame_status: pending-selection
---

# Texturing a Worn Wooden Stool in Substance Painter 🪑

**Source:** [YouTube](https://www.youtube.com/watch?v=sa_5vS4s_M0)
**Author:** 3DRedBox
**Duration:** 16m47s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py texturing-a-worn-wooden-stool-in-substance-painter <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hey everyone, welcome to another tutorial on 3D Redbox channel, my name is Mehdi and today
[0:14] we want to talk about how to texture this model inside Painter.
[0:18] But before that, let me introduce you the brand new course that we release for Substance Painter.
[0:25] Learning Substance Painter is easier than ever.
[0:27] Hey all Substance lovers, texture seekers and awesome future artists, welcome to ultimate
[0:34] course for learning Substance Painter from zero to hero.
[0:43] Ready to learn how to texture with different projects?
[0:46] Substance Master released a brand new course for those who want to learn to texture with
[0:52] Substance Painter.
[0:53] In this course, we cover from preparing the model to rendering different projects, different
[0:59] challenges.
[1:00] If you want to level up your skill in texturing, come and check the Substance Master Ultimate
[1:04] course for learning Substance Painter.
[1:07] Okay, before jumping to the texturing part, I need to explain something.
[1:11] In this model, we have different small pieces, so if we want to pack everything in one single
[1:17] UV space, it's not going to work for us because the texture quality at the end drops a lot,
[1:23] so I prefer to use overlapping technique.
[1:26] So basically, I choose some elements on the model, as you can see, and make the unwrapped
[1:32] for these parts.
[1:33] Okay, so this is the UV layout that I create for this model.
[1:37] And after that, I just duplicate the pieces in the way that I want.
[1:41] And I reach to this model.
[1:42] And if I go to the UV editor of this model, you can see we have the shapes that we want
[1:47] in the main UV tile.
[1:50] And in the overlap part, we have the others, and they are going to read the data from the
[1:55] main tile.
[1:56] Okay, so for baking and creating the mesh maps inside the painter, we need to bake this model.
[2:02] And after that, we can load this one.
[2:04] Okay, so let's go to the painter.
[2:06] And inside the painter, I'm going to load the model that we prepare for the baking phase.
[2:12] Everything here is okay.
[2:13] So let's press OK here.
[2:14] Okay.
[2:15] So we go down to the baking mode, change the output size to 4k, and change the antelasing
[2:21] to 64x.
[2:22] And we don't have any kind of hypoly here.
[2:25] So we can just check this.
[2:27] And we are done.
[2:28] And we can click on the bake selected texture and wait for the baking process done.
[2:32] Okay, the baking mesh maps is done.
[2:35] And right now we have all the mesh maps that we need.
[2:38] And we can change the model with a simple drag and drop.
[2:41] Okay, just press OK.
[2:42] And as you can see, everything is done and worked perfectly.
[2:46] That's great.
[2:47] And it's time to create different folders for different sections of the model.
[2:52] I have two different wood material, one for big pieces and one for smallest one.
[2:57] And the other one is the steel parts.
[3:00] Okay, for here and these connections.
[3:03] So I'm going to create the folder and create the mask.
[3:06] And after that, we create the wood surface and the steel part.
[3:08] Okay, now the masking part is done.
[3:11] As you can see, we have the folder related to wood pieces.
[3:15] And we have the folder related to wood small pieces.
[3:18] And we have the steel part too.
[3:21] And for wood pieces, I'm going to use a smart material from this collection that you can
[3:25] find the link for this collection inside the description.
[3:29] Right now I'm going to load the smart material into the folder.
[3:33] So if I bring my asset window, you can see we have different smart material.
[3:39] We can look at the time nail and choose the wood that we want.
[3:43] I think the number 15 is a great mood for starting.
[3:48] Yeah.
[3:49] And we need to go to the layers, turn off all the layers and just tweak a little.
[3:54] This is more material to fit in our project.
[3:57] So let's start with the first layer.
[3:59] This is the base and we can increase the quality inside the viewport with going to the texture
[4:04] set setting and increase the size from 1k to 2k.
[4:08] Okay, that's it.
[4:09] Okay, let's go to the base.
[4:10] Hey, that's great.
[4:11] I think the only problem here is the rotation so we can change the rotation.
[4:17] And that's it.
[4:18] And I'm going to add a fill here and just keep the roughness.
[4:21] And yeah, I think this kind of roughness is good for the base layer because we are going
[4:26] to add a lot of dirt layer.
[4:29] So basically this fill layer can control the roughness for us.
[4:32] Okay, that's great.
[4:34] Let's go for the next layer.
[4:35] And in the next layer, we have these details, the wood fibers.
[4:40] So let's go to the pattern.
[4:42] And I'm going to decrease the tiling from 4 to 3, maybe give rotation like 90.
[4:48] And we can play with the amount, increase the length, maybe a little thickness and put
[4:53] the random as high to something this and play with the warp option here.
[4:58] Okay, that's great.
[4:59] Right now we have a great wood fiber here.
[5:01] And that's great.
[5:02] Let's go to the next layer.
[5:04] Okay, and for the next layer, we can go to the mask and we can update the generator
[5:09] here.
[5:10] And yeah, this is good and enough for me for the edge wear because we just want to add
[5:15] some whiteness on the edges and in the overall shape so we can again go to the curvature
[5:20] and control the global balance.
[5:22] Okay, right now we have a good mask for that.
[5:25] And let's talk about the wood line.
[5:27] We need to change the rotation for the mask.
[5:30] So let's go to the mask.
[5:31] And in here we need to go to the wood pattern, change the projection to UV projection.
[5:36] Okay, increase the tiling to something like 2, increase the thickness.
[5:41] Maybe this one is good.
[5:42] Increase the random height or length.
[5:45] And yeah, this one is great.
[5:46] So let's go back to the layer itself and I'm going to increase the height amount to have
[5:50] more depth on this one.
[5:53] Something like negative 15 is good.
[5:56] That's great.
[5:57] At the end we are going to add ambient occlusion.
[6:00] So these are going to be more darkened and we can do it right now.
[6:03] Okay, let's add a paint layer here.
[6:06] I'm going to call it fact change the blending mode to pass through and apply it to all channel.
[6:11] And right now I'm going to add a filter and add the AO and we need to turn on the AO for
[6:16] our project.
[6:17] So let's go to the texture set setting, add the ambient occlusion channel here.
[6:21] Okay, that's great.
[6:23] And in here we just need to keep the AO and we can play with the height depth like this.
[6:28] That's great.
[6:29] This is the power of the ambient occlusion.
[6:30] So we just increase the visual look quality for our depth in the normal and the height.
[6:36] And we can add another filter here.
[6:38] Okay, height to normal, which helped me to increase the normal intensity because I'm
[6:43] not going to use the displacement or height when I export the texture from Substance
[6:47] Painter.
[6:48] So I need to some parameter to control the normal intensity to achieve the better look.
[6:54] So in the height to normal filter we need to turn off the use word units.
[6:58] And in here I can play with the normal intensity and I think two is enough.
[7:03] Okay, so yeah, let's go back to the wood line here.
[7:06] I think it's good enough.
[7:09] So let's go for the use damage layer.
[7:11] Okay, so for this layer I'm going to remove both of these sublayer and add another fill
[7:18] layer and use grunge like leaks.
[7:22] This one is great.
[7:23] And I'm going to increase tiling to three and change the rotation.
[7:27] It's great.
[7:28] We can play with the offset and I think this place is good.
[7:31] Okay, so let's go back to the material mode.
[7:34] And as you can see, we have a great result after adding the grunge inside the mask for
[7:40] huge damage.
[7:41] We can increase or decrease the opacity for this layer.
[7:44] Yeah, I think this is good.
[7:46] Maybe 80 is much better.
[7:48] Yeah, let's go for the edge damage.
[7:50] And I don't need this because we don't have actually edge on this wood.
[7:54] So we can just remove that and for spot damage, again, we can delete this one because we don't
[7:59] need this.
[8:00] Okay, and for the Z position, okay, yeah, we need this, but we need to decrease the opacity
[8:07] of the color to something like 30.
[8:10] This one, that's great.
[8:11] As you can see, we have the variation, darker variation of the color in here.
[8:15] Okay, let's go for the dirt and I'm going to change the generator to the dirt.
[8:20] Okay, that's great.
[8:22] And we can decrease the dirt level, or maybe we can increase the amount to something like
[8:27] this.
[8:28] Yeah, that's great.
[8:29] Okay, right now we have a good result, but I'm going to turn on the dirt number two.
[8:34] And in here, I don't need to have this generator so I can delete that.
[8:38] And for this grunge map, I'm going to increase the tiling amount and decrease the balance.
[8:43] Okay, that's great.
[8:45] So we have this dark spot on the color, as you can see, and we can control the amount
[8:50] of that balance.
[8:51] Okay, that's great.
[8:52] And we can add something like blur, like directional blur.
[8:56] Okay, this one.
[8:58] And we have this kind of effect of the color.
[9:00] That's great.
[9:01] Okay, I don't have this two layer here, so I'm going to delete that, but I want to add
[9:06] another fill layer to this wood material and make the surface more interesting.
[9:11] Okay, because it's old wood, we use it a lot and the environmental force make the surface
[9:17] color more darker.
[9:18] Okay.
[9:19] So I'm going to add another layer, let's call it dark area.
[9:23] And let's keep just color and the roughness.
[9:26] So for the roughness, let's put it on 0.8.
[9:29] And for the color, let's pick the dark one.
[9:32] And in here, I'm going to decrease the opacity to something like, for example, 60, or we
[9:38] can change it to 55.
[9:40] Okay, and let's add a black mask.
[9:43] Basically I want to create an interesting mask for this part.
[9:46] So let's add a fill layer.
[9:48] And in the leak search, we can choose this grunge leaky paint like this.
[9:54] And we can play with the balance.
[9:55] Okay, let's see what we have here.
[9:58] And right now I want to define two gradients from bottom to top and top to bottom.
[10:03] Okay, to control the area that piece mask should be appear over that.
[10:08] So let's create a generator here and use 3D linear gradient.
[10:13] Okay.
[10:14] So we have this one.
[10:15] This is the area that mask is going to be showed up.
[10:18] And I'm going to duplicate this one, press on invert, play with the balance.
[10:22] Okay, and this, this is fine.
[10:24] So let's put this two in here, change the blending mode to linear dodge to create this
[10:30] combination.
[10:31] I'm going to use an anchor point and it's probably gradient mask.
[10:35] Let's add a fill layer and load this gradient mask here.
[10:39] Okay.
[10:40] And now we can multiply this grunge mask to this area and we can control this area separately.
[10:46] Very easy.
[10:47] Okay, like this.
[10:49] And maybe we can increase the contrast in here again.
[10:52] Yeah, like this one.
[10:54] And we can add paint and change the blending mode of this paint layer to linear dodge or
[10:59] adding the detail and data that we create in this paint layer to what we have before
[11:05] that.
[11:06] And we can add the asset window and choose one brushes like this paint box.
[11:10] And I'm going to start painting in here to create more variation for this layer like
[11:16] this.
[11:17] Okay, we can increase the color intensity and adding more detail here.
[11:20] This great.
[11:21] Okay, that's great.
[11:22] So we create the interesting point on the surface and right now we need to create a bunch
[11:28] of layers for simulating the damage area.
[11:31] But before that, I'm going to duplicate this material and put it in small pieces.
[11:37] Okay.
[11:38] And in the small pieces, I don't want to have any kind of dark area.
[11:42] So I just removed that.
[11:43] And let's go to the base because I want to define the color, the new color for the material.
[11:49] Okay.
[11:50] And I'm going to pick some color from the reference for this.
[11:53] That's great.
[11:54] So we just duplicate the material that we create for the main part and with a small tweak in
[11:59] the color, create the material variation for small piece.
[12:03] Okay, that's great.
[12:04] So let's go back here and let's just create wood damage layer.
[12:09] So I'm going to create a new fill layer.
[12:11] Let's call it on your root layer.
[12:13] Let's load a material, the wood plane like this.
[12:17] Okay, because I don't want to receive anything from the height and the normal color, roughness
[12:23] and metallic from the layer that we have the blue of this layer.
[12:26] We need to change the blending mode of each channel of this layer to the normal.
[12:31] So let's apply to all channel and turn on all the channels that we have.
[12:36] Okay, that's great.
[12:37] And now it's time to play with the parameter that we have in here.
[12:41] I think we can increase the tiling to three.
[12:44] We can decrease the Google distortion.
[12:47] Maybe wood color should be changed some this.
[12:50] Okay.
[12:51] And for the veins density, I'm going to decrease it.
[12:54] Yeah.
[12:55] So we're going to add a main color fade.
[12:58] So we just fade the colors that we have here.
[13:02] And I'm going to decrease the fibers spread to the lower value.
[13:07] And yeah, I think I create a great underlayer wood surface for this object.
[13:12] And now it's time to add a black mask.
[13:14] That's great.
[13:15] So in the mask, I'm going to use a paint layer to paint some area, for example, in here,
[13:21] but there is no surface height difference.
[13:24] So I'm going to add a layer to the layer at a sublayer, keep the height and give the
[13:28] negative height.
[13:29] I think around negative 0.1 is good.
[13:33] And it's enough.
[13:34] Yeah.
[13:35] And let's add an anchor point here.
[13:37] Now I'm going to create another layer order effect.
[13:40] And let's add black mask, add a field, load the underwood layer mask, duplicate it, change
[13:46] the blending mode to subtract, add a filter here, choose the blur and increase the blur.
[13:51] Okay.
[13:52] And for the border effect, I'm going to increase the height or something like this.
[13:57] Or maybe we can go for the lower value for the roughness.
[14:01] Let's choose one.
[14:02] We don't need to have the metallic normal aile, just color, height and rough for the color.
[14:08] Let's peak the pure white and change the blending mode to soft light.
[14:11] Okay, that's great.
[14:13] So we create the damage like this.
[14:15] And the damage has the border effect.
[14:17] This one.
[14:18] Great.
[14:19] Let's go back to the mask and just remove everything here.
[14:23] And let's go choose a better brush like this one.
[14:26] I'm going to increase the white value for the brush.
[14:30] Okay.
[14:31] And let's paint damage to you all like this.
[14:33] And we can use some stencil for helping to achieve more realistic result.
[14:38] But right now it's enough for me.
[14:40] And I just want to add some minor damage like this one.
[14:44] Okay.
[14:45] Let's add another one here.
[14:46] And that's fine.
[14:47] Okay.
[14:48] Now you can give more time to add the more realistic paint for this layer and achieve
[14:54] better result inside the damage effect.
[14:57] Okay.
[14:58] But right now we are done with the wood.
[15:00] That's great.
[15:01] As you can see, we have a great result.
[15:03] And we can go back here and add another fill layer.
[15:07] Just keep the roughness.
[15:08] I'm going to make it as a roughness variation.
[15:11] Okay.
[15:12] Let's add a black mask.
[15:13] Go here.
[15:14] Add fill and add something like finger print effect.
[15:18] And increase styling to something this way.
[15:20] And we can play the roughness value.
[15:22] Yes.
[15:23] Much better.
[15:24] We can play with the balance and trust or we can invert it.
[15:27] Okay.
[15:28] This one is much better.
[15:29] And that's it.
[15:30] We just create roughness variation and that's fine.
[15:32] Okay.
[15:33] Let's go for the steel.
[15:34] And for the steel, I'm going to use a default smart material that comes with the substance
[15:38] painter.
[15:39] And the name of the smart material is the silver armor.
[15:42] Okay.
[15:43] It's not good that we have this rungy wood surface with a clean steel or the silver surface.
[15:50] So I'm going to create a fill layer and I'm going to call it dirt and just the color,
[15:57] roughness and the metallic because the dirt is not a metal surface.
[16:01] So let's bring up the roughness value to something like 0.8 and change the color to
[16:07] something like this gray.
[16:09] And I'm going to add the black mask and the dirt generator is and we can control dirt
[16:14] level to achieve the result that we want.
[16:17] Okay.
[16:18] That's it.
[16:19] So we just create a material for this is to and that's it.
[16:23] And at the end, I hope you learned something new in this video.
[16:26] And if you liked this video, please hit the like button, share your mind and thoughts
[16:31] in the comment section.
[16:32] And if you want to access the project file of this tutorial, you can join to our Patreon
[16:37] channel and the link of that is in the description.
[16:41] So just read the description, every detail that you need is over there and be safe, be
[16:46] creative.
[16:47] Bye.



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
