---
title: Texturing a Black Suit in Substance Painter
source: YouTube
url: https://www.youtube.com/watch?v=X24_IYUXOzU
author: 3DRedBox
ingested: 2026-08-12
app: "Substance 3D Painter"
version: "not stated on screen; narrator explicitly says the UV-set-to-UV-set fill projection source used to fix stripe-direction mismatch is 'a new feature for the Substance Painter in a 10th version' — places this at 10.0.0+ (2024-05-16, per version-tracker.md); UI (Export dialog, Texture Set list, no Skew/OpenPBR) is consistent with the pre-12.1 era"
tags: [layers, fill-layer, paint-layer, masks, smart-material, generator, curvature, anchor-point, blend-mode, baking, mesh-maps, ambient-occlusion, udim, texture-set, uv, pbr, metal-rough, basecolor, roughness, metallic, height, normal-map, alpha, procedural, export, export-preset, channel-packing, game-engine, unreal-export, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/texturing-a-black-suit-in-substance-painter/
frame_count: 9
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Texturing a Black Suit in Substance Painter

**Source:** [YouTube](https://www.youtube.com/watch?v=X24_IYUXOzU)
**Author:** 3DRedBox
**Duration:** 25m14s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hey everyone, welcome to another tutorial from our YouTube channel, Tier 3 Red Bugs, I'm
[0:14] Mehdi and today we are going to talk about how to texture this suite inside the Painter
[0:18] and render it inside the Marmoset Toolbag 5.
[0:21] So, beat me, but before that, let me introduce you the brand new course that we release for
[0:26] Substance Painter from Zero to Hero.
[0:29] Learning Substance Painter is easier than ever.
[0:32] Hey all Substance lovers, texturing seekers and awesome future artists, welcome to ultimate
[0:38] course for learning Substance Painter from Zero to Hero.
[0:48] Ready to learn how to texture with different projects?
[0:51] Substance Master really is a brand new course for those who want to learn to texture with
[0:57] Substance Painter.
[0:58] In this course, we cover from preparing the model to rendering different projects, different
[1:04] challenges.
[1:05] If you want to level up your skill in texturing, come and check the Substance Master Ultimate
[1:09] course for learning Substance Painter.
[1:12] Okay, welcome back and we can start the process.
[1:15] So first of all, we need to load the model inside the Painter and for this specific model,
[1:20] we are going to use UV Tide workflow because we need to have high quality texture at the
[1:26] end and we don't want to lose any detail on the material.
[1:29] Okay, so let's press OK.
[1:31] And as you can see, we have the model inside the Painter and as UV, we have these three
[1:37] UV Tide for the suite and this one is for the accessory like button and the button holes.
[1:43] Okay, so that's it and we can continue our work.
[1:46] First of all, we need to go to the baking menu and bake all the mesh maps for this model.
[1:51] So I'm going to turn on Bent Normal, change the output size to 4K and change anti-aliasing
[1:56] to 64X and just press on the bake select the texture and wait for the end result and after
[2:02] that we can continue our processing in the texturing base.
[2:05] Okay, now for the first step, I'm going to create the layers for the suite itself.
[2:10] So we are going to use a premade material from Substance Community Asset.
[2:14] So it's free, you can use it.
[2:16] I'm going to put the link in the description so you can download it and use it in your
[2:20] project.
[2:21] So it's so easy, you need to just download the file, click and drag, import it to your
[2:26] layers and yeah, you have that.
[2:28] Okay, and let's bring down the scale.
[2:31] Maybe six is good.
[2:33] Yeah, perfect.
[2:34] And we have a good base for the fabric and we can go into the pattern and change the
[2:40] type of the pattern that we have.
[2:41] For example, we can have the checkerboard or we can have the wave or mesh type.
[2:46] Okay, I prefer to use the wave and let's increase the size of the document so we can see what's
[2:52] happening on the texture much better and let's increase the tiling to three or maybe we can
[2:58] go for the four.
[2:59] Yeah, it's okay.
[3:00] Yeah, and I'm going to decrease this promissor, maybe lines intensity so avoid any kind of
[3:06] lines effect on the material.
[3:08] Yeah, like this.
[3:09] And I'm going to increase tiling for the line.
[3:12] So yeah, it's so much better.
[3:14] Okay, let's pick the color of the top in a dark gray and for the bottom we can go darker.
[3:20] Yeah, something like this.
[3:21] The black suite is so awesome.
[3:23] Okay, so let's decrease the wrapping lines effect and we can go to the parameter itself
[3:28] and change the luminance variation.
[3:31] So if you bring up this option, this is the result that you are going to get but I'm going
[3:35] to decrease it.
[3:36] Yeah, it's so much better in this way.
[3:38] Okay, that's great.
[3:40] Before doing anything else, let's go to the texture set setting and add the inclusion
[3:44] channel because we need that here.
[3:46] Okay, and it's time to create the lines on the fabric.
[3:50] So I'm going to create fill layer.
[3:52] Let's call it lines pattern and I just need to have the color roughness and the metallic.
[3:57] I choose the metallic channel because I want to have some metallic line on the suite.
[4:03] So let's bring up the metallic value to something like 0.8 and the roughness value is good for
[4:09] me and maybe a little darker gray would be better.
[4:13] That's great.
[4:14] So we can go here, add the black mask and add the fill and in this field, I'm going to
[4:19] load a strip.
[4:20] That's great.
[4:21] Okay, let's change the tiling to something like 5 and let's go back to the pattern.
[4:26] I'm going to increase the strip to 12.
[4:29] Yeah, and let's bring down the width size.
[4:32] So we have the small line.
[4:34] That's great like this.
[4:35] And for the shift, let's bring it to 0.
[4:38] Okay, so we have a problem here and the problem is mismatching in the direction or the texture.
[4:44] But how we can solve this?
[4:45] The old method is to mask the area and create a duplicate layer and just rotate it.
[4:50] But the new workflow is using the UV set.
[4:54] So I'm going to choose the UV set and change the source to UV set 1 and as you can see,
[4:59] the direction is right.
[5:01] So let's change the rotation to 90 and it's fixed.
[5:04] That's a new feature for the Substance Painter in a 10th version and it's awesome.
[5:09] But how we can set the UV set for our model?
[5:12] Let's do that.
[5:13] Okay, right now I'm going to use Sirius Max for doing this stuff, but you can do it with
[5:17] any other software like Blender or Maya.
[5:21] So basically you just need to create a guidance, another UV set for Substance Painter to set
[5:27] the direction of the texture or the projection of the texture.
[5:30] Okay.
[5:31] So first let's select the model.
[5:33] Okay, give the unwrap UVW map modifier to that and we have the UV layout for the model,
[5:39] but the direction is not right.
[5:40] Okay, so let's bring this UV layout to the next channel.
[5:44] Okay, so I'm going to use the move.
[5:47] So we are in a second channel and we have the same UV layout that we had inside the
[5:53] first channel.
[5:54] Okay, and in this channel, we are going to change the direction of the UV island according
[5:59] that we need and we want.
[6:01] So let's select all these layers of the UV.
[6:04] Okay, that's great.
[6:06] And I'm going to just choose the rotate 90 degree.
[6:10] That's great.
[6:11] Or we can do it in a way like this.
[6:13] Okay, that's great.
[6:14] So there is no need to packing again, rearrange the UV island, just change the rotation in
[6:21] the way that you want.
[6:23] That's it.
[6:24] And we just need to convert it to editable poly.
[6:26] So your model is going to have two separate channel.
[6:30] The first one is the main UV channel that you are going to create your texture based
[6:34] on that.
[6:35] And the second one is a guidance for your texture projection inside the painter.
[6:40] And you just need to reimport this model to the painter and that's it.
[6:44] So we find a way to solve this kind of problem.
[6:47] I mean the direction mismatching problem very easy and very fast with the new feature inside
[6:52] the substance painter, which is very powerful and you can implement that technique into
[6:57] your texturing process and solve various problems.
[7:00] Okay, but right now we create the line, we create the base of the fabric and we need
[7:05] to create a folder for them.
[7:07] Okay, so let's call it sweet base, put that into the folder, create a mask, add a paint
[7:12] and just select the area that I want.
[7:15] Okay, that's great.
[7:16] We create a mask for our first folder, but I'm going to add another paint here to the
[7:21] line pattern, change the blending mode to subtract and choose some area here like these
[7:26] parts to create some variation for our sweet material.
[7:30] Okay, so basically we create the base and I'm going to add some color variation.
[7:35] So let's add the first layer, the color variation number one.
[7:39] I'm going to pick the color, just the color and put it on white value, change the blending
[7:44] mode to soft light and add a black mask at the generator, go here and choose a 2D linear.
[7:50] Okay, that's great.
[7:52] So let's play with the balance and we can change the color to the black.
[7:56] I think it's much better.
[7:58] So let's invert it.
[7:59] Yeah, I think it's so much better.
[8:01] That's great and can play with the balance again, change the opacity of the layer and
[8:06] yeah, that's great.
[8:07] So let's create another color variation.
[8:10] So let's add a mask, add a field and let's load something for, I think for number one
[8:15] is good.
[8:16] Let's bring up the tiling number.
[8:19] Okay, play with the controls, play with the balance.
[8:21] That's great.
[8:22] So let's add filter blur.
[8:24] Okay, that's great.
[8:26] I'm going to add another field, load a grunge.
[8:29] Okay, bring down the balance, change the blending mode to subtract.
[8:32] Yeah, and let's add another filter here and let's load the histogram scan.
[8:37] So let's go to the mask.
[8:38] So I think it's good to have some white spot on the surface, but we need to bring down
[8:43] the scale, the balance, play with the blur intensity and we can control it with the position
[8:49] in the histogram scan.
[8:50] Okay, so let's bring something.
[8:51] Okay, that's great.
[8:52] So let's go back to the layer.
[8:54] I just need to keep the color in height, just a small amount of height and maybe white value.
[8:59] And we are going to tweeze opacity that it's great.
[9:03] Okay, and I think that's enough.
[9:04] We can add another free layer.
[9:06] Let's call it curvature.
[9:07] Okay, just pick the color.
[9:09] Let's go to the white value, change the blending mode to something like soft light.
[9:13] Yeah, and let's go to the black mask and the generator and load the curvature.
[9:18] Okay, so basically it's going to add more value on the edges and the top surface.
[9:24] Okay, and we can decrease the opacity, but as you can see, we have a great touch on the
[9:30] wrinkles, for example.
[9:31] That's great.
[9:32] You can go here, play with the global blur or value.
[9:36] So we can decrease the opacity again.
[9:38] I think, yeah, this would be great for this model.
[9:40] That's fine.
[9:41] So we create the first folder for the suite and it's a base and we need to move on to
[9:46] the tie and other piece of the suite.
[9:49] Okay, let's focus on the tie.
[9:51] And for the tie, I'm going to create a folder.
[9:53] Let's tie.
[9:54] Let's add a color like orange to that.
[9:57] Let's add a black mask, choose the area for the tie.
[10:00] Okay, that's great.
[10:01] So we just create a mask for the tie and let's go here and create a feed layer.
[10:06] I'm going to call it the base and we just need to have the color, high roughness and
[10:10] metallic.
[10:11] Okay, so let's pick the red color for that, but not kind of this red.
[10:17] Maybe this one is much better.
[10:18] Okay, I'm going to bring up the roughness to something like 0.6.
[10:23] Okay, that's great.
[10:24] And I'm going to add a field layer.
[10:26] Let's call it street pattern and just add a black mask and add a field and load a strip
[10:32] texture here.
[10:33] Okay, first let's choose the tiling number to 10 and let's go back to the pattern.
[10:39] Okay, bring down the sheet to maybe this one.
[10:42] I want to have this direction.
[10:44] So let's change the rotation to 90.
[10:46] Okay, and bring up the sheet and yeah, I think 10 is good or maybe 9.
[10:50] I'm going with the 8.
[10:52] 8 is much better and let's bring down the weed to something else.
[10:55] Okay, that's great.
[10:57] Let's duplicate the street pattern, divide the tiling to 2 and put the 5 here.
[11:03] Change the blending mode to linear dodge.
[11:05] Okay, that's great and come back again, play with the weed and create this kind of pattern.
[11:10] You can add different pattern in here.
[11:13] Let me search about fabric.
[11:15] For example, you can choose this kind of pattern for the tides.
[11:18] Okay, you can download any kind of pattern from the internet, import it here and use
[11:22] it.
[11:23] But in a year, I prefer to use strip lines.
[11:25] Okay, so let's add another field like blur and put the value like 0.11.
[11:30] Okay, that's fine.
[11:32] And I'm going to add an anchor point in here because I want to create different fabric
[11:37] pattern for this area and the red one.
[11:39] Okay, so let's create another field layer.
[11:42] I'm going to call it the nanoparture and let's add a black mask, add a field, load the strip
[11:47] pattern anchor point that we create and just add a level and invert it.
[11:52] Okay, that's fine.
[11:54] So I'm going to use the material mode in the layer and load the cotton jersey.
[11:59] Hey, that's great.
[12:00] Let's bring up the tiling to the 5.
[12:02] We don't want to have the color roughness metallic A or anything else.
[12:06] We just need to keep the height in here.
[12:09] Let's go to the technical parameter and bring down the height range to some, yeah, 0.05
[12:14] is good.
[12:15] And we just need to come back to the strip pattern layer, change the blending mode to
[12:19] soft light, go back here, the white value, pure light, and we can control it with the
[12:24] opacity.
[12:25] Okay, that's great.
[12:26] We can keep it like this.
[12:28] It's a solid one.
[12:29] That's great.
[12:30] Let's just keep the color and the height and roughness and we can play with the roughness.
[12:34] Let's bring up the height.
[12:36] Yeah, I think it's much better.
[12:38] It's better to keep it like this.
[12:40] Okay.
[12:41] And for the color, we can create another fill layer, make color variation number one and
[12:45] same, we can use this method here too, but we need to adjust 3D linear mask like this
[12:52] or maybe we can choose the inward one.
[12:54] Yeah, so much better.
[12:56] And for the color variation number two, we can add another black mask go here and just
[13:01] search about the fabric and choose the clothes fold large so we can increase the tiling.
[13:06] Yeah, and I'm going to create the pure white, change the blending mode to soft light and
[13:11] play that slide.
[13:12] Okay, so we just add some variation on that.
[13:15] That's fine.
[13:16] So we are done with the tie.
[13:17] That's enough for that.
[13:18] And let's focus on the dress shirt that we have in here.
[13:22] Okay, so let's just create another folder and name it dress shirt.
[13:26] Okay, that's great.
[13:27] Let's add a pack mask and choose the area that we want.
[13:30] Okay, for the dress shirt, let's create a fill layer and I'm going to call base in the material
[13:35] mode.
[13:36] Let's load the denim.
[13:37] Okay, that's great.
[13:38] I'm going to bring up tiling to something like five or six.
[13:42] Yeah, it's good.
[13:43] And let's peak white value.
[13:45] Okay, this is a dark gray or maybe we can bring double detail and keep white.
[13:49] Okay, that's great.
[13:51] I'm going to the technical perimeter bring down the high range.
[13:55] That's great.
[13:56] And let's bring up the tiling to 12.
[13:58] Okay, that's fine.
[13:59] And I'm going to add the over pattern layer.
[14:02] Okay, let's add the black mask.
[14:03] Okay, and add a fill layer.
[14:05] Just search about the fabric.
[14:07] And in here, I'm going to use the fabric, the normal theme.
[14:10] Okay, let's bring up tiling to something to any.
[14:13] That's great.
[14:14] And let's use the UV set, UV set number one to create the correct direction for our texture.
[14:20] Okay, and I'm going to change the blending mode for all channel to the normal.
[14:24] So just right click on the blending mode and use apply to all channels option.
[14:29] That's great.
[14:30] Okay, let's go back to the mask and we can increase tile four.
[14:33] And yeah, much better.
[14:34] And we can play with the number.
[14:36] Okay, like this, play with the band, achieve the result that we want.
[14:40] Okay, I think it's good and it's enough for the white dress shirt that we have.
[14:45] Let's go back to the layer, keep the color, high roughness and the normal.
[14:49] Okay, let's peak a little whiter value and we can add little depth to the pattern that
[14:55] we have here like this.
[14:57] And for the roughness, maybe it's much better to have something like mid-range the roughness
[15:02] value.
[15:03] That's great.
[15:04] Let's check other channel.
[15:05] This is the base color.
[15:06] This is the roughness.
[15:07] Yeah, it's so much better.
[15:08] And this is the normal plus high plus mesh.
[15:11] And yeah, perfect, perfect.
[15:12] Okay, that's great.
[15:13] But it's not the overall pattern that we want to have.
[15:16] We want to have different pattern on this part.
[15:19] So let's create folder and call it the base.
[15:22] Put these two in here and the black mask and choose the area that we want.
[15:27] And let's create another folder.
[15:28] I'm going to name it second layer, add the black mask, go to the mask and choose this
[15:33] layer.
[15:34] Okay, it's super easy to fill this second layer because we want to have this base again
[15:38] inside the second layer.
[15:40] Okay, like this.
[15:41] But the color, it's totally different.
[15:43] I'm going to pick the color from the tie.
[15:45] Okay, and just make it a little darker or maybe we can go for the brighter color.
[15:50] Yeah, I think that's good.
[15:52] And I'm going to create another fill layer and call it color variation number one or
[15:56] we can call it fabric pattern.
[15:58] It's much better to understand what we are going to have in this layer.
[16:02] So we just need to keep the color, the height and the roughness and the metallic.
[16:06] Okay, I'm going to add a little metallic value to that, a little roughness.
[16:11] We need to change it to more rougher surface.
[16:13] Okay, maybe a little height value like this amount.
[16:17] And for the color, let's pick the dark value and we are going to change the blending mode
[16:22] of all channels to the normal.
[16:24] Okay, like this.
[16:25] And let's add the black mask, add the fill, search about the fabric.
[16:29] And I'm going to choose this one.
[16:30] Fabric star block and bring up tiling to 10.
[16:34] Yeah, and we can increase tiling here to four.
[16:38] Okay, let's play with the roughness.
[16:40] That's fine.
[16:40] Okay, yeah, I think it's good.
[16:42] Let's go back in here and maybe we can go for the minor negative value like this one.
[16:47] And yeah, I think it's good.
[16:48] It's good and enough.
[16:50] And we can create again the color variation in here.
[16:54] Okay, same structure.
[16:55] And yeah, I think you can control balance.
[16:58] Okay, maybe change the black color to white.
[17:01] It's a good option.
[17:02] And I'm going to bring it up and put it on top of the fabric pattern because we want
[17:06] to have this effect on the fabric pattern too.
[17:08] And let's decrease the opacity.
[17:10] That yeah, I think it's good.
[17:12] That's great.
[17:13] And this is for the second layer.
[17:15] Okay, we are done and we can go for the accessory and create the material for the accessory.
[17:20] And after that, we are going to export everything from painter to the marmoset and create a lighting.
[17:24] But before doing that, okay, let's add this area to the dress shirt folder.
[17:30] Go back in the second layer and I will have inside this.
[17:34] Okay, that's great.
[17:35] And let's start the accessory material and finish up this project.
[17:39] Okay, let's go for the accessory part and for the accessory, I'm going to create the mask.
[17:44] So basically, we just need to go to the UV layout and just select this part because we
[17:49] just put together all the UV island related to the accessory in this UV top.
[17:54] Okay, so the mask is already in.
[17:56] We are going to use that.
[17:57] And for the first part, I'm going to use the plastic small material comes from the substance
[18:02] prankter itself, plastic soft dirty.
[18:05] Okay, I think that's good.
[18:06] And we just need to change some minor setting like the roughness value.
[18:10] Yeah, like this, because we want to have some shiny surfaces for the bottom.
[18:15] Okay, and let's add the color variation.
[18:18] Number one, let's pick the white value, change the blending to soft light, add a black mask
[18:23] and choose the field.
[18:25] And in here, let's load the ground, something like grunge map for okay, that's great.
[18:30] And I'm going to balance.
[18:32] Let's add a filter like Blair.
[18:34] Okay, so we have a great result in here.
[18:38] Maybe we can increase the blur intensity.
[18:39] Yeah, that's fine.
[18:41] And that's enough for the bottom itself.
[18:43] And I'm going to add another material for these parts.
[18:47] Okay.
[18:48] Add a field layer.
[18:49] I'm going to call it night look and in the material mode, let's search about the night
[18:53] one itself.
[18:54] Yeah, we have it.
[18:55] Okay, that's great.
[18:56] Let's go to the parameter and make it white and the dark gray.
[19:00] Yeah, it's better to have it in this way.
[19:02] You can play with the roughness value or play with the fabric variation.
[19:06] Okay, let's add a black mask, add a paint and choose these areas.
[19:10] Hey, the mask is ready.
[19:11] And as you can see, we have this, maybe we can add more.
[19:15] Yeah, maybe this felt better.
[19:17] That's great.
[19:18] And I think we are done inside the pot before exporting.
[19:21] We need to add final touch on the third case.
[19:24] So let's read this paint layer to the effect, the blending mode to pass through and apply
[19:28] to all channels.
[19:29] And we'll add a filter like the sharpness.
[19:32] Okay, so we have the sharpen and the one is too long.
[19:36] So I suggest to you to pick a value between the zero and two and zero point eight.
[19:42] Okay, so in here, I choose zero point two.
[19:45] Okay, that's fine.
[19:46] Let's filter and going to call that the contrast and bring up the contrast, the color.
[19:52] We just need to have this on the color.
[19:53] So be sure to turn off all channel except the color.
[19:57] So this is the difference.
[19:58] And at the end, let's add a and a filter like high to no.
[20:02] Okay, and I'm going to turn off the use word unit.
[20:05] So we have intensity.
[20:07] And for this project, I think two is enough.
[20:09] Okay, maybe I can go with that.
[20:12] And for the AO, we can decrease the radius.
[20:14] That's great.
[20:16] Right now we are going to export the texture from substance painter.
[20:19] Okay, with the Unreal Engine for template, let's put the file type to base on output
[20:24] and just for the size, pick the four K.
[20:26] Okay, I'm going to export it, import everything inside the Marmoset, create a lighting system
[20:31] and render it and the finish.
[20:32] Okay, right now we are in the Marmoset tool bag and we just need to import our model
[20:37] with the simple drag and drop and choose the material and change the UV in the texture
[20:43] to you, because we use the UV tile workflow inside the painter or in the other words,
[20:49] you deems.
[20:50] So we just need to change this setting.
[20:52] And right now we can import the texture with a single drag and drop.
[20:56] And as you can see, it's low, the UDMS.
[20:58] So it's super simple.
[21:00] And yeah, okay, so let's change the channel for the roughness to the G copy this texture,
[21:05] paste it here, change the channel to the B.
[21:08] And for the occlusion, we have this paste texture and the red or the R is fine for the
[21:13] occlusion.
[21:14] Okay, so the material is good, but we need to flip why for the normal.
[21:18] As you can see, we have this, okay, we can select the model, turn off the callback faces.
[21:23] That's great.
[21:24] So I'm going to create a camera, change the focal length to something like 75.
[21:28] Okay, that's great.
[21:30] And let's go back to the render and just change the output size to 2000, 2500.
[21:36] Okay, that's great.
[21:37] Go back to the camera, choose the save frame option.
[21:40] So we have this.
[21:41] And right now we can change the render engine type in here.
[21:45] So we change the raster mode to the ray tracing.
[21:48] Great.
[21:49] And now it's time to create the lighting setup.
[21:51] So I'm going to select the sky, change the backdrop to the color, pick the dark gray
[21:56] like this.
[21:57] Okay, and in the library, let's go to the interior and choose the train station.
[22:02] Okay, put it on 10.
[22:04] That's great.
[22:05] It's time to add the additional lights.
[22:07] So first of all, I'm going to add a light, change the type to the directional.
[22:12] And in the position, let's make zero for the rotation, make zero for the position two.
[22:18] Okay, just select the light, turn off the sky and change the light shape to the rectangle.
[22:24] Put it on the maximum value that we have here, change the brightness to something like seven.
[22:29] Okay, and just bring the light to the back.
[22:33] So this is the backlight that we have.
[22:35] Okay, for the color, let's pick the white.
[22:37] And I'm going to duplicate this one and just rotate it in the X axis to create the top
[22:43] light.
[22:44] But we need to control the shape like this.
[22:47] And even we can change it to the spot.
[22:49] Okay, so we can bring it up, the brightness, increase the spot angle.
[22:54] Yeah, and we have this kind of top highlight effect.
[22:57] That's great.
[22:58] So we need to create the field light and the key light.
[23:01] So let's duplicate this directional light.
[23:04] I'm going to name it the key light.
[23:06] Okay, let's turn off all the lights, change the shape to the sphere, bring up the diameter
[23:11] and let's rotate it.
[23:13] Okay, so this is our key light.
[23:15] This is our backlight.
[23:16] Okay, and this is our top thick light and we can decrease the brightness or that.
[23:21] Yeah, maybe this one is good.
[23:22] And let's rename it to top light and for that back, okay, so we have this arrangement and
[23:28] let's duplicate the key light and rename it to the field light.
[23:32] That's great.
[23:33] And just rotate it and I think this side is good, but we need to decrease the brightness
[23:38] to some this.
[23:39] Okay, and yeah, we have the studio lighting that we want.
[23:42] It's great.
[23:43] Let's go back to the camera, go to the tune mapping.
[23:45] We can change the tune mapping to the Aces, but it's going to create our image more darker.
[23:50] Okay, so we can keep the tune mapping with the new method that Marmoset gives us in the
[23:55] fives version and just play with the clarity, a little contrast, play with highlight, control
[24:00] it and play with the mid tone and shadow.
[24:02] Go back to the sky, bring down the color in here.
[24:06] Go back to the camera, go back to the post effect, increase the sharpen in the render.
[24:10] Yeah, I think it's good.
[24:11] Maybe we need to increase highlight a little and we can increase the exposure to, yeah,
[24:16] I think it's much better.
[24:17] Okay, we can have the bloom.
[24:19] We need to increase the size and we have we need it.
[24:21] And that's it.
[24:22] We have a beautiful shot inside the Marmoset.
[24:24] We can duplicate the camera, change the camera and set your location and the frame for the
[24:29] camera like this.
[24:30] Okay, and we can go to the focus, turn on the depth of field, choose a location and you
[24:36] create this beautiful shot.
[24:38] Okay, and that's it.
[24:39] So I hope you learned something new in this tutorial.
[24:42] If it's all, please hit the like button, share this video with your friend and put your
[24:47] mind in the comment section.
[24:48] You can contact us with the email or you can visit our store in the artstation, in the
[24:53] website and we recently opened a Patreon channel that you can visit over there.
[24:59] We are going to create more content for the Patreons over there and you can have exclusive
[25:04] benefits like one on one session, feedback in on your personal project and so on.
[25:09] So don't forget to do all these actions.
[25:12] Be happy, be safe, be creative and bye.



---

## Captured Frames

- [1:34] tutorials/frames/texturing-a-black-suit-in-substance-painter/frame_000.jpg
- [1:51] tutorials/frames/texturing-a-black-suit-in-substance-painter/frame_001.jpg
- [4:44] tutorials/frames/texturing-a-black-suit-in-substance-painter/frame_002.jpg
- [5:04] tutorials/frames/texturing-a-black-suit-in-substance-painter/frame_003.jpg
- [9:18] tutorials/frames/texturing-a-black-suit-in-substance-painter/frame_004.jpg
- [11:34] tutorials/frames/texturing-a-black-suit-in-substance-painter/frame_005.jpg
- [17:44] tutorials/frames/texturing-a-black-suit-in-substance-painter/frame_006.jpg
- [20:19] tutorials/frames/texturing-a-black-suit-in-substance-painter/frame_007.jpg
- [22:02] tutorials/frames/texturing-a-black-suit-in-substance-painter/frame_008.jpg

---

## Structured Notes

### Core Technique
UDIM/UV-Tile garment texturing of a full suit (jacket, tie, dress shirt/vest, plastic/metal accessories) built from layered smart materials and fill layers, using Painter's UV-set-to-UV-set projection source to fix pattern-direction mismatches across UV islands, then exported and lit/rendered in Marmoset Toolbag 5.

### Summary
A full pipeline video: load a 3-UV-Tile suit model, bake mesh maps (with Bent Normal), build the jacket's pinstripe fabric from a free Substance Community smart material plus a hand-built metallic "Lines Pattern" stripe layer, solve a fabric-direction mismatch between UV islands with a secondary guide UV channel authored in 3ds Max and Painter's UV-set-projection source, layer in curvature- and generator-driven color variation, then repeat a similar base+pattern+variation recipe for the tie (with an anchor-point-driven secondary weave layer), the dress shirt/vest (nested Base/Second Layer folders sharing one mask), and the accessories (buttons, selected via Polygon Fill on a UV island, built from the `Plastic Soft Dirty` smart material). Finishes with a Pass-Through "final touch" paint layer stacking Sharpen/Contrast/AO filters, exports an Unreal-style PBR Metallic-Roughness template at high resolution, then imports into Marmoset Toolbag 5 for UDIM-aware channel-packed material setup, a 3-point light rig plus HDRI backdrop, and final composited hero renders.

### Key Steps
1. **Import the model using a UV-Tile (UDIM) workflow** — 3 UV tiles confirmed in the Texture Set list: one for the suit body, one for the tie/shirt, one for accessories (buttons/buttonholes) — chosen specifically to preserve high texture detail rather than a single shared UV set.
2. **Bake mesh maps** with `Bent Normal` enabled, output size set to 4K, anti-aliasing set to 64x, then `Bake selected textures`.
3. **Build the jacket base from a free Substance Community smart material**: drag-and-drop import, scale to 6, switch the material's built-in pattern type to `Wave` (vs. Checkerboard/Mesh options), raise pattern tiling to ~4, lower "lines intensity" to avoid a visible line artifact, raise line tiling, pick a dark grey top / darker bottom color split, and tune the `Luminance Variation` parameter down from its default (too strong) value.
4. **Add an extra channel via Texture Set Settings** before proceeding (transcript: "add the inclusion channel") — done specifically to support a channel the stripe/metallic work below needs; exact channel name uncertain from audio alone.
5. **Build a dedicated `Lines Pattern` fill layer** for the pinstripes: enable only Color/Roughness/Metallic, push Metallic to ~0.8 (metallic thread look), tune roughness, pick a darker grey; add a black mask + Fill with a `Strip` pattern alpha, tiling ~5, Strip count 12, reduced width, Shift 0.
6. **Fix stripe-direction mismatch across UV islands with the UV-set projection source** (called out explicitly as new in Painter 10.x): in the Fill layer's `Projection` settings, set `Source` to `UV set 1` (a second, guide-only UV channel) instead of the default UV set, then set `Rotation` to 90 — corrects the pinstripe direction without re-masking or duplicating layers, which the narrator calls out as replacing the older workaround (mask + duplicate + manually rotate).
7. **Author the guide UV set in the DCC app (demoed in 3ds Max, works the same in Blender/Maya):** apply `Unwrap UVW`, copy the existing UV layout into a second UV channel, select the same island selection, rotate it 90° in that second channel only (no repacking needed since it's a projection guide, not a real UV layout), convert to Editable Poly, re-export/re-import into Painter.
8. **Organize and finish the jacket base**: group Suit base + Lines Pattern into a `Suit Base` folder with a black mask (paint-selected area); add a second paint mask on the Lines Pattern layer set to `Subtract` blend to hand-remove the stripe in selected regions for variation.
9. **Layer procedural color variation on top**: a `Color Variation #1` fill (white value, `Soft Light` blend, black mask + `2D Linear` generator, then invert + balance tuning); a second color-variation fill using a numbered alpha + increased tiling + `Blur` filter + a `Grunge` fill (`Subtract` blend) + `Histogram Scan` filter to place small white surface spots, feeding a small amount into Color+Height.
10. **Add a `Curvature` fill layer**: white value, `Soft Light` blend, black mask + `Curvature` generator — pushes extra value onto edges and the top/highest surfaces (visibly picks out jacket wrinkles), opacity brought down after.
11. **Build the tie in its own folder**: base fill (Color/Height/Roughness/Metallic only) in a red picked specifically for contrast, roughness ~0.6; `Stripe Pattern` fill using a `Strip` alpha (tiling 10, Rotation 90, then tuned to ~8), duplicated with tiling halved (~5) and blended `Linear Dodge` for a denser secondary stripe pass, plus a `Blur` filter at 0.11.
12. **Drive a second weave layer off an Anchor Point**: place an Anchor Point on the Stripe Pattern layer, then build a new fill (`Nano Texture`) whose black mask references that anchor point via a `Levels` filter (inverted) — loads the `Cotton Jersey` material in Material mode, height-only (Color/Roughness/Metallic/Normal unchecked), tiling 5, `Height Range` reduced to ~0.05, then blended `Soft Light` back onto the Stripe Pattern layer for woven-fabric depth.
13. **Build the dress shirt/vest in nested folders**: a `Base` fill using the `Denim` material (tiling ~5-6, white/dark-grey split, Height Range reduced, tiling raised to ~12) plus a `Fabric` (normal) pattern fill projected through `UV set 1` (same guide-UV trick as Step 6) with its blend mode set to `Normal` for all channels via right-click → `Apply to all channels`; group Base + pattern into a `Base` folder with a paint mask, then a `Second Layer` folder reusing that same mask (copy-mask reference) but recoloring (color picked from the tie) and adding its own `Fabric Pattern` fill (`Fabric Star Block` alpha, tiling 10/4, small Metallic + Roughness + Height) plus a repeated Color Variation pass moved above the Fabric Pattern layer.
14. **Build the accessory (buttons/buttonholes) material** on its own UV tile: switch to `Polygon Fill` mode and click the relevant UV island directly in the 3D/UV view to generate the mask (no manual painting needed since the island is already isolated on its own tile); apply the built-in `Plastic Soft Dirty` smart material as the base, raise roughness contrast for shine; add a grunge-driven Color Variation fill (`Soft Light` blend, black mask + Fill + `Blur` filter).
15. **Add a top-of-stack "final touch" `Paint Layer`** set to `Pass Through` blend, applied to all channels, holding three filters: `Sharpen` (recommended range 0–0.8, used ~0.2), a `Contrast` filter isolated to the Color channel only (all other channels disabled), and an AO-style filter with `Use World Unit` off, Intensity ~2, reduced radius.
16. **Export** via the Export Textures dialog using an Unreal-Engine-oriented `PBR Metallic Roughness`-style output template, PNG file type, output size set to 4K (dialog defaults shown mid-setup before the resolution/preset were finalized).
17. **Marmoset Toolbag 5 finishing pass**: drag-and-drop import the mesh, switch the UV mode to UDIMs to match Painter's UV-Tile export, wire the channel-packed texture manually (paste-and-recopy the same texture into Roughness=G, Metallic=B, AO=R channel slots), flip the Normal map's Y/green channel, disable backface culling; set up a 75mm-focal-length camera, switch the render engine from Raster to Ray Tracing; build lighting from an HDRI backdrop (`Interior` library → `Train Station`) plus a custom 3-point rig — a rectangular `Back light` (directional, brightness ~7), a `Top light` (duplicated + rotated, shape switched Rectangle→Spot with widened spot angle), a spherical `Key light`, and a `Fill light` (duplicated key, lower brightness); tune tonemapping (Marmoset 5's newer non-ACES tonemap method, since plain ACES over-darkened the result), post effects (clarity, contrast, highlights, exposure, bloom, sharpen); duplicate the camera per hero shot and enable Depth of Field for final composed stills.

### Layers / Tools / Settings
- **Smart materials used:** free Substance-Community fabric smart material (jacket base, Wave pattern mode), `Plastic Soft Dirty` (accessories base)
- **Materials loaded in Material mode:** `Cotton Jersey` (tie's anchor-point-driven weave layer, height only), `Denim` (dress-shirt base pattern)
- **Alphas/patterns used:** `Strip` (jacket pinstripes, tie stripes), `Fabric Star Block` (second-layer vest pattern), unnamed numbered fabric alpha + `Grunge` (color-variation breakup), `Fabric normal theme` alpha (dress-shirt weave normal)
- **Generators used:** `2D Linear` (color variation mask), `Curvature` (edge/highlight value pass)
- **Filters used:** `Blur`, `Histogram Scan`, `Levels` (on the anchor-point-referencing mask, inverted), `Sharpen` (~0.2), `Contrast` (Color-channel isolated), an AO/HBAO-style filter (World Unit off, Intensity ~2)
- **Blend modes used:** `Soft Light` (color variation, curvature, weave-over-stripe), `Subtract` (stripe removal paint, grunge breakup), `Linear Dodge` (secondary tie stripe density), `Normal` applied to all channels (dress-shirt pattern normal), `Pass Through` (final-touch composite paint layer)
- **Projection/UV technique:** Fill layer `Projection` set to `UV set to UV set projection`, `Source: UV set 1` — a second, projection-guide-only UV channel authored in the DCC app specifically to control pattern rotation per-island without remasking; called out as a Painter 10.x feature
- **Anchor Point usage:** one anchor point placed on the tie's Stripe Pattern layer, referenced (inverted, via a Levels filter) by a separate Cotton Jersey weave-detail layer's mask
- **Texture Set Settings:** an extra channel added before stripe work began (audio: "inclusion channel", exact name uncertain)
- **Baking settings:** `Bent Normal` mesh map enabled, 4K output, 64x anti-aliasing
- **Export:** `Export Textures` dialog, Unreal-oriented PBR Metallic-Roughness template, PNG, 4K
- **External render app:** Marmoset Toolbag 5 — UDIM-mode texture import, manual channel-packing (R=AO/G=Roughness/B=Metallic into one packed map), Normal-Y flip, backface culling off, Ray Tracing render engine, HDRI Interior/Train-Station backdrop, 3-point custom light rig (Back/Top/Key/Fill), non-ACES Marmoset-5 tonemap, Depth of Field

### Difficulty
Intermediate to Advanced — the layer-building recipe itself (fill layers, generators, grunge breakup) is approachable, but the UV-set-to-UV-set projection trick requires understanding a second guide UV channel authored in an external DCC app, and the pipeline spans three applications (DCC for UVs, Painter for texturing, Marmoset for lighting/render/channel-packing).

### App & Version
Substance 3D Painter — version not stated on screen. The narrator explicitly frames the UV-set-to-UV-set fill projection source (used to fix the stripe direction mismatch, Key Step 6) as "a new feature for the Substance Painter in a 10th version," which places this tutorial at Painter 10.0.0 or later (2024-05-16 per `references/version-tracker.md`). No OpenPBR shader or Skew baking UI (both 12.1.0+) is visible, consistent with a pre-12.1 version. Render/finishing pass uses Marmoset Toolbag 5 (external, not a Painter version signal).

### Tags
layers, fill-layer, paint-layer, masks, smart-material, generator, curvature, anchor-point, blend-mode, baking, mesh-maps, ambient-occlusion, udim, texture-set, uv, pbr, metal-rough, basecolor, roughness, metallic, height, normal-map, alpha, procedural, export, export-preset, channel-packing, game-engine, unreal-export, intermediate

---

## Related Tutorials
- [How to texture a realistic slipper model](how-to-texture-a-realistic-slipper-model.md) — same creator (3DRedBox); shares the same overall production recipe (DCC-side mesh prep, 4K/64x-AA baking, layered smart-material-plus-hand-built-fill-layer construction) and both videos independently date to the same pre-11.0.0 tool-naming era.
- More 3DRedBox tutorials (wooden stool, lace shorts, poison bottles, UDIM workflow deep-dive, shawl, tactical boots, UV-set/stencil video, NavyCap) will be cross-linked here as they are ingested — see `tutorials/INDEX.md` for the current full list.
