---
title: How to Texture NavyCap In Substance Painter in English
source: YouTube
url: https://www.youtube.com/watch?v=dGmVGU7aHb4
author: 3DRedBox
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/how-to-texture-navycap-in-substance-painter-in-english/
frame_count: 0
frame_status: pending-selection
---

# How to Texture NavyCap In Substance Painter in English

**Source:** [YouTube](https://www.youtube.com/watch?v=dGmVGU7aHb4)
**Author:** 3DRedBox
**Duration:** 24m35s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py how-to-texture-navycap-in-substance-painter-in-english <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


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
