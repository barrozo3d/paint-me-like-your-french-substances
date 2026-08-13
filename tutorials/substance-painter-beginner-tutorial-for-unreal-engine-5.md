---
title: Substance Painter Beginner Tutorial for Unreal Engine 5
source: YouTube
url: https://www.youtube.com/watch?v=dXDWFPHkeZM
author: Unreal Sensei
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/substance-painter-beginner-tutorial-for-unreal-engine-5/
frame_count: 0
frame_status: pending-selection
---

# Substance Painter Beginner Tutorial for Unreal Engine 5

**Source:** [YouTube](https://www.youtube.com/watch?v=dXDWFPHkeZM)
**Author:** Unreal Sensei
**Duration:** 175m21s | 25 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py substance-painter-beginner-tutorial-for-unreal-engine-5 <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hello everyone, if you want to learn how to make materials and textures in Substance Painter and Unreal Engine 5, then this video is made for you. In this tutorial, you will go from knowing nothing about Substance Painter to creating this asset you see right now.
[0:15] All the textures were created from scratch in Substance Painter and brought into Unreal Engine 5. In case you don't know, Substance Painter is the most popular program for creating textures and materials for 3D. It is used everywhere.
[0:27] If you have ever played a video game in the past couple of years, odds are the majority of assets were textured using Substance Painter. It is industry standard. And Painter is the main way we create textures for Unreal Engine 5. Both some real objects were made with this program. In this tutorial, you will learn how to import 3D models and navigate inside of Painter, how to use the layer system and masking, create generators to speed up our workflow, paint custom detail and textures, bring materials and textures from Substance Painter into the game.
[0:57] And then you will learn how to import 3D models and textures from Substance Painter into Unreal Engine 5, create materials and edit textures in Engine, how to automatically create textures with smart materials, and finally how to paint high textures for use with Unreal's Nanite Displacement.
[1:10] Included in the description is a free master material made specifically for use with the Substance Textures you create. It has all the features you need, including Nanite Displacements.
[1:21] So we can create 3D height detail inside of Painter and breed it into Unreal, unlocking new creative possibilities.
[1:28] You will finish this video with a practical set of skills that can be applied to creating any material you can think of in UE5.
[1:35] Recently Epic Games launched Fab, which is their brand new marketplace for all 3D assets.
[1:40] To promote the marketplace, if you buy something for $25 or more, you get 6 month access to Substance Painter and Substance Modeler for free.
[1:50] Substance Modeler is a new program made by the same team behind Painter. It lets you create and sculpt objects without polygons, making it a lot easier to create 3D models than other programs.
[2:01] This video is sponsored by Epic Games and Adobe. Without them, these programs wouldn't exist. So let's jump into Substance Painter and start creating materials.


### Creating a Project [2:11]
**Transcript (timestamped):**
[2:12] To begin, this is what you will see when you open up Substance Painter for the first time. You can download it through Adobe Creative Cloud or through Steam if you got it there.
[2:21] Now to create a new project and start painting, you want to come up to File and in the drop down select New. This will bring up the New Project Settings.
[2:30] And the first thing it will ask for is the 3D model we want to paint. So go ahead and press the Select button and then navigate to the location of the 3D model.
[2:40] You can download this 3D model and all the assets I use in this video for free in the description of this video below.
[2:47] Included are two objects we are going to paint and an Unreal Engine project that has the Substance Massive Material we will cover when we get to the Unreal portion of this tutorial.
[2:57] Now to begin to cover the basics of Substance Painter, I want to paint the Meat Matte object.
[3:04] To select that, now we can select the resolution of the textures we will be painting on.
[3:10] So I'm going to select 4096, but you could select 1K textures. Substance Painter is unique in that it is non-destructive.
[3:18] You can start painting on a 1K texture and then later on upgrade all the textures to 4K without any issue. It keeps all the data.
[3:27] So it is up to you what resolution you want to pick.
[3:29] Now these two settings are very important if you plan on using them in Unreal. For the normal map format, make sure you select DirectX and then for Compute Tangent Space per Fragment, make sure this is turned on.
[3:42] You need these two settings for Unreal projects. Those are the only settings we need. So with that, we'll click on OK to create our first project.
[3:52] Now we can see the 3D model we have opened up on the left and then on the right is a 2D view of our model's UVs.
[3:59] As a reminder of the different parts that make up a 3D object, we have the Static Mesh, which is the 3D shape of the model, but a mesh is just a geometry.
[4:09] It doesn't have any material data, which is why we add a material onto it that defines how the mesh is rendered.
[4:15] Generally a material is made up of textures, and there are four main ones we use constantly. The most important one is the color texture, which defines what colors the object should be.
[4:26] A roughness texture, which is how rough or shiny the material is. A metallic texture, which defines what parts of the object are metallic and what are not.
[4:36] And a normal map, which artificially adds fake shadows to give the appearance that the object has more detail than it actually does.
[4:43] Together with these four textures, you can represent the majority of materials, from rocks to traffic cones. This is called physically based rendering or PBR for short.
[4:53] The entire purpose of Substance Painter and what you will learn in this tutorial is how to create those textures using this program.
[5:01] As a brief explanation for what we are seeing on screen right now, on the right we have a UV map.
[5:07] In order to put textures onto a 3D object, that model needs a UV map, which is just a 2D representation of the 3D object.
[5:15] Each of these sections of the UV map represent a different location on the model.
[5:20] Without UV maps, 3D programs wouldn't know how to use these textures.
[5:24] For our purposes, and for the majority of the time we are using Substance Painter, I just want to edit and view my model in the 3D viewport, not having this entire space taken up by the UVs.
[5:35] So instead, what I will do is up here, we'll select this button next to the pause icon and in the dropdown select 3D only.
[5:43] That's how I'm only focusing on this model.
[5:46] Now, the most important part of any 3D program is how we can navigate in the viewports to do so you want to hold down the Alt key.


### Navigation and UI [5:51]
**Transcript (timestamped):**
[5:54] And with that key held down, hold down the left mouse button to pan.
[5:58] So this will allow us to pan around the object.
[6:01] And then still with the Alt button held down, if we press the middle mouse button, so hold down on the middle mouse button, which is the scroll wheel, we can pan.
[6:10] So that is Alt, left mouse button to rotate and Alt, middle button to pan.
[6:16] Holding down Alt, I can press the right mouse button to zoom in and to zoom out.
[6:22] Alternatively, you can also use the scroll wheel up and scroll wheel down to zoom in and out.
[6:27] So whenever I'm navigating inside a painter, you want to hold down the Alt key.
[6:31] And let's say if I'm really far away, I have no idea where I am.
[6:36] Uh oh, where's my model? Press F to focus back to it.
[6:40] Before we jump into creating material, let's cover the user interface and what all these panels do.
[6:45] And if you ever used an Adobe program in the past, you're probably already familiar with some of these panels.
[6:51] So on the far left over here, we have our tool selections.
[6:54] So this will help us when we're painting, we can select a tool.
[6:57] We will cover what a lot of these tools do in due time.
[7:01] And then up here is the toolbar.
[7:04] So the toolbar will change depending on what tool we have selected.
[7:08] So by default, we have the paintbrush tool, which as you can guess, will just allow us to paint.
[7:14] So we will cover the paint tool in depth in just a moment.
[7:18] And to the right of that, we have the asset browser.
[7:22] So this is the content browser for Substance Painter.
[7:26] And it comes with a bunch of useful assets like materials, paint brushes, textures,
[7:32] and a bunch of other things that we will also use when painting our objects.
[7:37] Also up here, I can switch over to the Substance 3D Assets,
[7:41] which is a bunch of extra materials created by Adobe that we can download.
[7:46] So this gives us even more options for our texturing.
[7:50] Now, all the way over here, we have the texture set list at the top.
[7:54] This is where we will have multiple materials in case our object has different materials.
[8:00] This will be covered when we paint the next mesh after this one.
[8:03] And then below that is the Famous Layers tab, which we will use in just a moment.
[8:09] But this contains all the layers, all the data that makes up the material we are creating.
[8:14] So this is where we're going to be spending the majority of our time in here,
[8:19] manipulating the layers to get what we want.
[8:22] And with all these windows, we can make them bigger by hovering over in between them
[8:28] and then adjusting them like this.
[8:31] Also to the right of layers, we have texture set settings.
[8:34] This is where we adjust settings for the material up here.
[8:38] We will come to these settings when they are needed.
[8:42] And then below layers, we have the properties window,
[8:45] which is where we can change and edit the properties of a selected layer.
[8:50] So for example, if we have a fill layer, now the properties window changed
[8:54] to show the settings of that layer.
[8:56] Or when I select the original layer, then it changes to the paint settings.
[9:01] So what I'll do is select a layer and delete it because we will cover that.
[9:06] I just want to show how important the properties window is.
[9:09] We'll be making a lot of changes here for our layers.
[9:12] And then at the far right is a bunch of docked windows.
[9:16] So these windows currently aren't being shown.
[9:18] But if we select them, then we can see what is inside of those windows.
[9:22] So here are the display settings for my viewports, which we will cover next.
[9:26] And below that is also the shader settings.
[9:29] When there is a property we need to change, I'll make sure to note it
[9:32] when I'm coming over here and selecting it.
[9:35] Now the user interface is also very customizable.
[9:38] I can hold my mouse button over any of these interfaces to undock them.
[9:43] And then still with my left mouse button held down, I can move this window
[9:47] between other ones, for example, over here, or I could dock this at the bottom like that.
[9:53] So sometimes when you are watching other substance painter tutorials,
[9:56] you'll see that the asset browser is down here.
[9:58] Also, if I ever exit out of a window, for example, the substance 3D assets.
[10:03] Now we'll see that a new window is docked over here, which is the window that we exited out of.
[10:09] If I ever want to get back this window into my viewports, then hold down the left mouse button
[10:14] and just drag it out as a docked one and bring it back right there.
[10:19] Now let's say I exit out and I mess up my user interface to the point of no return.
[10:25] I have no idea how you could get back the original user interface.
[10:29] Then all you have to do is come up to window and select reset UI to get back the original user interface.
[10:37] Now I just want the 3D viewports because now I'm going to cover the controls we have over this window
[10:43] because obviously this is the most important one because this is where we are viewing our object.
[10:48] So all the way over here, we can select this little icon that looks like a screen and these are the display settings.
[10:56] Now let me go ahead and I'll make this a little bit bigger and increase the environment opacity.
[11:02] And we can see that we have an environment that is illuminating our object.
[11:08] I can also go down to environment blur and bring it all the way down to zero.
[11:14] That's what we can actually see what this environment is.
[11:17] So this is the default environment.
[11:19] And if I ever want to, let's say, rotate an environment, I can hold down shift
[11:24] and then hold down the right mouse button holding down shift.
[11:28] And the right mouse button will allow me to rotate the environment, which is very important to see my model at different lighting angles.
[11:36] Now, if I want to change the background that we have, well, what I can do is come back to viewports and under environment map by default is set to panorama.
[11:45] Substance painter comes with a bunch of other environment textures.
[11:48] So we can see what it looks like in a little cave.
[11:51] Now our model has a bit of a greenish tint coming from the texture or see what it looks like in a studio lighting situation.
[11:59] But what I tend to do is to just keep it at the default of panorama.
[12:03] So I will type panorama to get that back and select it and bring down the environment opacity all the way to zero.
[12:11] Another thing you might see me do is go to environment exposure and bring this up.
[12:16] This will just control the brightness of my viewport.
[12:20] It's not actually controlling the colors of my textures.
[12:23] So I'll keep that as default value of zero for now.
[12:26] And if you don't like the flat look of my model, we have the ability to enable shadows.
[12:32] So by selecting shadows, we now have a closer representation of what it will look like in engine.
[12:38] Although I do think that this is way too strong by default.
[12:42] It is pitch black.
[12:43] So by bringing down the shadow opacity to something super small, we can just get a little bit of depth.
[12:48] Just get a little bit of a shadow going on, which can help out.
[12:52] Also, if you set it to intensive, then the shadows will have really good quality.
[12:57] For now, I will leave this off, but I might turn the back on in the future.
[13:01] Those are the important settings for the viewport.
[13:04] You also notice that with a lot of these panels, we have extra buttons up here.
[13:08] If you see a window with these buttons, these are just shortcuts to allow us to quickly jump to a different category of settings.
[13:15] Because obviously there could be a lot of settings.
[13:18] So if you want to quickly see the camera settings, I can click on this and then it'll just move down to those settings.
[13:24] So we will see these in a lot of the user interfaces.
[13:27] I'll press X to close that window.
[13:30] And here is one of my favorites shortcuts.
[13:33] And that is if I press tab, it will temporarily hide everything.
[13:38] So it will dock all my windows to the side right here.
[13:41] I still have access to my windows if I select them like this, but I'm just able to focus specifically on the model,
[13:50] which is really good if you want to zone in and really focus on a model without the clutter of the UI.
[13:56] I'll press tab again to bring back my windows.
[13:59] Now, before we make any changes, of course, we need to save our project.
[14:03] Because if we get out of this program, then we lose all our progress.
[14:07] So to save is as you can guess is with control and s.
[14:11] Now you can navigate to where you want to save this file on your computer.
[14:14] In my case, I'll save it to a folder called substance painter project on my desktop.
[14:18] And I'll call this first project and then click on save.
[14:23] So now whenever I save, it'll be saved to that project.
[14:26] And if I exit out of substance painter to open up that project, I can just double click on the painter file.
[14:34] Now that we know how to navigate within substance painter, let's create our first material.


### First Material with Fill Layers [14:37]
**Transcript (timestamped):**
[14:39] Throughout this tutorial, we are going to texture two objects.
[14:42] The first object is this little character called meat math.
[14:45] This is a simple 3d model and will be used as an introduction to the core features of painter.
[14:50] Most of painters features will be demonstrated on this guy.
[14:53] And then later in this tutorial, we will move on to a much more advanced object by texturing this science fiction crate asset to demonstrate some painters more advanced features.
[15:02] Both of these materials will be imported into unreal back in substance.
[15:06] In order to create materials, we have to use the layer system.
[15:10] This is why I like to say the substance painter is basically Photoshop, but in 3d.
[15:16] We have a layer system that is very similar to Photoshop and other programs.
[15:20] So if you've ever used those programs, you probably are pretty familiar with how it works.
[15:25] And don't worry if you don't know what this is, we are going to cover it in depth.
[15:29] So by default, we have a paint layer.
[15:32] We will cover this in the future.
[15:34] But for now, I will delete this and create the simplest layer possible in substance painter.
[15:39] And that is a fill layer up here by clicking on the paint bucket.
[15:43] So clicking on this will create a fill layer.
[15:47] And by selecting it, we can now edit its properties down here below the layers.
[15:53] So scrolling all the way down here until we get to materials, we can see that we can edit the
[15:58] different properties or channels of this material.
[16:02] So we could change the base color right here by selecting it and I can change it around.
[16:08] So let's go a red color or go down into the roughness setting.
[16:13] And I can make this really rough by dragging this all the way up to one or bring it down to zero to make this really shiny.
[16:21] So this is the core of substance painter and PBR materials in general.
[16:26] And that is in order to create materials.
[16:28] All we are doing is editing the base color metallic and the roughness.
[16:33] So for example, if I want a gold material, then within the base color, let's change this to something a little bit like dark orange right there.
[16:43] And then for metallic bring this all the way up to one.
[16:47] And now we have a gold material or if I want this to be iron, I can come here and then make this to be a little bit more shiny.
[16:55] Make this to be a little bit off gray like that.
[16:59] And it still play with the roughness.
[17:01] That's how it's not completely shiny.
[17:04] This is the essential to physically base rendering.
[17:07] We have a base color where we can choose the color and then we have a value from zero, which means no metallic to one, which is 100% metallic and a roughness value that is zero.
[17:19] So there is no roughness and then one where we don't get any reflections.
[17:25] These are the same values that you see in unreal material system blenders materials and most three programs up here under material.
[17:36] We can choose what channels this fill layer is using.
[17:39] So if I only want to edit, let's say the base color, then what I'll do is just uncheck metal rough normal height.
[17:47] And now this fill layer will only change the base color.
[17:51] So for this layer, I do want to edit the metal and the roughness and let's make a painted plastic look.
[17:59] So for metal, I'll bring this down to zero for no metallic and roughness bring this down so that it's a little bit shiny.
[18:06] For the color, I want to use a bright orange.
[18:09] So let's move this up and play with a hue on this bar.
[18:13] I think this is a good color for now.
[18:15] We could always go back in and change it.


### Textures [18:18]
**Transcript (timestamped):**
[18:18] Obviously, this material does not look realistic because it is uniform.
[18:23] There are no changes to its color and there are no changes to its roughness.
[18:27] Normally, you would expect imperfections on a material because nothing is perfect except in computer graphics.
[18:34] So that's the goal is to make it not perfect.
[18:37] So the easiest way to do that right now is to break up its roughness.
[18:41] That's how some areas in the mesh are shiny and other areas are not.
[18:46] And we can drive this roughness value with a texture.
[18:50] So over here within assets, I can select the texture icon and I would get access to a bunch of different textures.
[18:57] You can pick any black and white texture, but specifically I'm going to use the texture that's called grunge rough dirty right here.
[19:05] Because each pixel within this texture represents a value from zero to one.
[19:11] So we will use this texture to now drive it.
[19:14] Hold down the left mouse button.
[19:16] I can go ahead and drag this onto my roughness channel and let go like that.
[19:21] So now if I move the light around using the shift and right mouse button,
[19:25] we can see that we're getting different reflections on the model and already it looks a lot better.
[19:32] An alternative to adding a texture is let's first get rid of it by pressing X and then select roughness right there.
[19:39] Then type in what I want, which is grunge rough dirty and select that.
[19:44] Now the benefit of this texture is that it is procedural.
[19:48] What that means is that we can edit the look of this texture through some of its properties that we can change right here.
[19:54] So under the roughness texture, there is balance.
[19:57] I can bring this down to bring back more shininess or bring it up like this.
[20:02] I can also play with a contrast to change how that grunge exactly looks, which is pretty cool.
[20:09] Now one thing to note when it comes to reflections is that if we want higher quality reflections,
[20:15] that more represent the rendering engines that we are going to use this material inside of that you could come up here to the shader settings,
[20:22] which is this ball icon and under specular quality bring it up to something like high.
[20:27] We will just get better, more accurate reflections that way.
[20:31] And if I want to know exactly how my roughness channel is changing, then up here in the dropdown,
[20:37] I can just look at my roughness by going down here under signal channel and selecting roughness.
[20:43] Here is what our texture currently looks like.
[20:46] So where this model is black are the shiny areas and then the white areas are the non shiny areas.
[20:53] If I change it down here, so bring down the contrast.
[20:57] And if I play with the balance right here, you can see it updating in real time so we know exactly what is happening.
[21:04] And if I ever want to see the entire material again, come up here and select material or I can press the M key as a shortcut.
[21:13] M stands for material.
[21:16] Before we continue, let's briefly go over texture projection and to do so just as a demonstration.
[21:22] So we won't use this for the final material.
[21:24] I'm going to scroll all the way up here under the texture category and grab the texture that's called camo woodland.
[21:30] So I'll go ahead and drag this on top of base color and let go.
[21:34] Now it is this texture that is driving the color of this fill layer, not just a single uniform color.
[21:40] So this texture is pretty cool because I get to edit the color of all the spots right here.
[21:46] But the main reason why we're using this is to showcase how for all these textures, if I scroll up in the fill layer at the very top right here,
[21:54] we have the projection settings for this texture.
[21:57] So I can increase the tiling right here to make it tile a lot more.
[22:02] And now you'll start to see this texture repeating.
[22:07] And by default, the textures are added to the object using the objects UVs.
[22:12] And to see the UV map, we can come back up here to this button and select 3D and 2D.
[22:19] So it is just projecting this image using the UVs that this model came with.
[22:24] And let's go to tiling and I'll bring this back to one and UVs are good.
[22:30] But oftentimes we can have some issues and a better see this.
[22:33] I'll go ahead and go back to 3D only.
[22:36] And that is on the back.
[22:38] The UV seams are very noticeable.
[22:41] We can see that there's just a cut right there at the back of the object.
[22:45] And then at the bottom here, this can be hard to see because of the lighting.
[22:50] So I'll go to material and select base color.
[22:53] Also increase the tiling.
[22:55] There's a UV seam at the bottom here.
[22:58] So generally what I like to do for the majority of my textures is to not project them using the UVs,
[23:04] but instead use triplanar.
[23:07] So by selecting that, now those UV seams are completely eliminated.
[23:12] So I'll press M to go back into material mode and press controls the a bunch because that was just a demonstration to get back my original material.
[23:22] Now scrolling down here, I'm able to edit this texture by using the UVs.
[23:27] So as we shown beforehand, if we look at the roughness at the back of my mesh, there is a very noticeable steam.
[23:36] So what I'll do to fix this is switch that to triplanar, which is exactly what I want.
[23:42] And by playing with the tiling right here, we can get more detail out of this texture.
[23:48] So in the material, the changes between the roughness are much smaller now, compared to when they were at one.
[23:56] But in my case, I do like how it looks at one.
[23:58] So I'll leave it there.
[23:59] But just know that that is an option.
[24:01] So you will see me often throughout the tutorial, select a fill layer and then change the projection for its textures to triplanar to hide the UV seams.
[24:12] So now we will cover the most fundamental aspect of painter, and that is combining multiple layers with mass.
[24:20] So to do that, let's create a brand new layer coming up here and selecting the fill icon again.
[24:26] What I want it to be is a light blue color, press on the color to bring up the color picker.
[24:31] And let's go ahead and change it to bluish.
[24:35] I like this one and exit out.
[24:37] And one thing you will notice that with the fill layer by default, is that it overridden and replace all the layers below it.
[24:45] We can better see this by temporarily hiding this layer.
[24:48] To hide layers, just click on the I button on the layer.
[24:51] You can see that the roughness and the color are being replaced.
[24:55] And in my case, I do want this to replace the color, but I don't want it to replace the roughness.
[25:00] I want the roughness of my bottom layer to be carried over.
[25:04] So to do this with a fill layer, I'll just go ahead and unselect roughness.
[25:09] This layer is completely ignoring roughness.
[25:12] It is taking the same values that it had from the bottom.
[25:16] I'll also uncheck metal, normal and heights, since this is only going to change the base color.
[25:22] Now if I change the metallic or roughness in the bottom layer, it will carry over to the top layer.
[25:28] So here I'm increasing metallic or changing the roughness.


### Mask [25:33]
**Transcript (timestamped):**
[25:33] But I still want the original color.
[25:36] I don't want this blue layer to be on top of the entire mesh.
[25:40] I only want the character's arms to be blue.
[25:43] So to tell substance painter where I want this layer to be on the mesh, we use masks and masks operate the same way they do in Photoshop or any other program.
[25:53] So to add a massive layer, make sure it's selected.
[25:56] And then up here, select the mask icon and in the dropdown select black mask.
[26:01] Now that blue layer has disappeared.
[26:03] But if I start painting on this mask, make sure the mask is selected and that we are using the paint tool and painting like this.
[26:11] We can see that that layer is slowly starting to be revealed again.
[26:15] And to see exactly what is happening, we can look at the mask by holding down alt and clicking on a mask.
[26:22] So holding down alt and clicking will reveal that a mask is just essentially a black and white texture.
[26:29] So where there is white is where the layer will be revealed and where there is black is where the layer won't be.
[26:35] So if I just paint like that and then to get out of mask view,
[26:40] I could come up here and select material or just like with a shortcut, I could click on the M key.
[26:46] Throughout this tutorial, you will see me hold down alt and click on the mask a bunch to see exactly where the layers are being added.
[26:54] And with the brush, I could come all the way down here.
[26:58] So make sure you scroll down under grayscale and bring it down to zero.
[27:03] So by painting black, we are now taking away from the mask.
[27:07] The brush tool is pretty important in substance painter.
[27:10] As we can see, we have a bunch of different options.
[27:13] So this tool will be covered in depth in another section of this tutorial.
[27:17] For now, I want to show exactly what the polygon fill tool does right here.
[27:22] Right now I'm in the brush tool and I want to add to the mask just the arms of my object, nothing else.
[27:28] So what I could do is come in here and with white selected to start painting my mask.
[27:35] But this is a very long and tedious process, or I can use the mesh's geometry to change the mask.
[27:42] I want to start with a clean mask.
[27:44] So I need to clear it by right clicking on the mask and selecting clear mask.
[27:49] Now I'll go ahead and select the polygon tool right here.
[27:52] And by default, either this triangle or this polygon is selected.
[27:57] What this allows us to do with a value of one, if I zoom in to any of these policies,
[28:03] I can start selecting them like this.
[28:06] And we are just filling in those exact polygons by holding down alt and selecting the mask.
[28:12] We can see exactly what is happening.
[28:15] It's just adding whites to that location according to the policies.
[28:18] Or I can bring this all the way down to zero and then start subtracting away from a mask like this.
[28:26] Now I don't want to select each polygon individually.
[28:29] That would obviously take a while.
[28:31] So what I will do is press on the mesh fill select icon, which is the 3d box.
[28:37] And what this will allow me to do with a value of one is select entire sections of the objects that are not connected to each other.
[28:44] For example, this arm is not connected to the body or the head.
[28:48] So if I select it, now this entire arm will be white, or I could just select the ground or the head to fill them in.
[28:56] I'll press Ctrl and Z to undo those.
[29:00] And let's go ahead and select the other arm.
[29:04] So pressing the M key going back to material mode, we can now see that this is exactly what I want.
[29:10] My second layer using the mask is only affecting the arm section.
[29:15] Of course, if you do not want to see the polygons on the mesh, then you can select anything else other than the mask.
[29:21] So I'll go ahead and select that layer to get back my original view.
[29:25] If you ever want to disable your mask temporarily for some reason, then hover your mouse over the mask, hold down Shift and click on it.
[29:33] This will give us an X icon, which will disable the mask.
[29:37] If I want to re-enable it again, then Shift click on top of it to get rid of the X icon.
[29:42] Now let's add in a third layer.
[29:44] But before I do that, as we can see, my layer names are just fill layer one and fill layer two.
[29:49] To organize my project a bit, I can double click on the name to rename it.
[29:54] Let's call this layer paint one and double click right here to call this one paint two.
[30:00] Now this third layer will be a layer of dirt on top of everything.
[30:05] So I'll come up to the add fill button, select that, and this will be my dirt.
[30:11] I don't need the normal and I don't need the height.
[30:14] But what I do want is the color, metal and roughness because dirt is not metallic.
[30:19] So I want to make sure that this is zero and it's going to override any metallic values that we have.
[30:24] We don't have any metallic values, but just in case if we do add them in the future, it's good to set this dirt layer metallic to zero.
[30:31] And then for the roughness, bring this up.
[30:33] That's how it's super rough.
[30:34] Dirt obviously isn't shiny.
[30:36] And then base color.
[30:38] Let's just make this a really dark brownish color.
[30:41] Like right here.


### Effects [30:42]
**Transcript (timestamped):**
[30:43] Okay, great.
[30:45] Now we will add in a black mask by selecting the mask icon, selecting black or a shortcut is to just right click on the layer and then select add black mask right there.
[30:57] Now, instead of manually painting where the dirt is on the mesh, let's drive this mask with a texture.
[31:04] So something we can do to mask is add in effects.
[31:08] So you can think of effects as basically layers within layers.
[31:12] So making sure this black mask is selected.
[31:15] If I select the wand icon, now I could come down here and then add in a fill.
[31:20] So by doing that, we can see that this mask has a fill layer right there.
[31:25] And in order to see this, just in case if you're unable to select an effect, make sure the mask is selected.
[31:31] So now I can select that and to better see what is happening, hold down alt and click on the mask.
[31:38] So with the fill layer and the properties, I'm able to decrease it to zero or increase it to one.
[31:44] But we want this to be driven by texture.
[31:47] So I could grab a texture from here and drag it into the properties or click this.
[31:53] And now let's go ahead and let's find dirt for and I want to select this texture right there.
[32:01] So go ahead and select it.
[32:03] And now we will see that this mask is created through this texture.
[32:07] Going into the full material view, we can see a layer of dirt on top of everything.
[32:13] And already this is starting to look a little bit more realistic.
[32:16] Now, I think this is too much dirt.
[32:18] So with it selected, I can bring down the balance to get rid of the dirt or I could change its opacity.
[32:27] So let me go all click again by coming here to this drop down of 100.
[32:33] I can bring this down so we can see we're transitioning from zero.
[32:37] And then this is the opacity of that layer.
[32:39] So something like 40, I think will look good.
[32:43] Okay, so just a very subtle change of just a little bit of dirt on top of everything.
[32:48] And is important to say that order does matter for these layers.
[32:52] If the dirt was, let's say below, holding down the left mouse button and dragging below paint to there is no dirt on the arms,
[33:01] which is why we want it to be the first layer.
[33:04] So it's on top of everything.
[33:05] And let's make it clear that this layer is dirt by double clicking on the name and typing in dirt to see what we have created.
[33:13] So far, we can go through all of my channels.
[33:16] For example, I can look at the base color or see the roughness and how the dirt is now affecting the roughness.
[33:22] Or what I can do to see all my different channels is the shortcut C key.
[33:27] So C will allow me to cycle through our channels and just pressing M will bring it back.
[33:34] So that's a shortcut to very quickly see the roughness or color channel.


### Bake Mesh Maps [33:38]
**Transcript (timestamped):**
[33:39] It is time to cover one of substance painters main features and that is baking mesh maps.
[33:44] Mesh maps are textures that are specific to the 3d model, which store information about how the model is formed,
[33:50] which can help us in the texturing process.
[33:53] Now, I know that was a lot of words. So it's best to show with an example.
[33:57] So hopping back into painter to bake mesh maps, you want to come up here to the top right hand corner and select this croissant icon to bring up baking.
[34:07] Now there are a bunch of settings and it can be intimidating for the most parts.
[34:12] Unless I'm doing something very specific, we can leave everything at its default.
[34:16] So if you do make a change, you can just click on restore defaults to bring it back.
[34:21] Now I'm going to come down here and select bake selected textures.
[34:25] And we can see in real time those textures being created.
[34:29] Now that we are finished baking to return to the main mode, which is called painting mode.
[34:33] I can select this button right here or select the paintbrush icon in the top right now to see the new maps that were created in the texture set settings.
[34:43] I can scroll down and here are all the new maps and to visualize it on my mesh.
[34:51] Instead of viewing our materials channels scrolling more down, we have mesh maps that we can look at.
[34:57] So the most important map that was just created is the ambient occlusion map.
[35:02] Here you can see exactly what it is.
[35:04] It is a texture that is adding black to the crevices or corners of our mesh.
[35:11] So we can see that right here where the arm is in between the body, it is darker or where the foot is on top of the base here.
[35:21] There's like almost like a little bit of a shadow.
[35:24] And the next most important map that was created is the curvature map that I can select there, which shows us where the edges of the mesh are.
[35:33] So where the mesh becomes really sharp and its corners.
[35:36] And you can see that when we're transitioning in sharp areas, it gets a little bit wider to quickly see all the mesh maps because mesh maps are pretty important.
[35:46] There is the B key to cycle in between them.
[35:49] So pressing B, I can see everything that was created and M to go back to my material mode.
[35:55] One thing you might have noticed after creating the mesh maps is that the ambient occlusion is automatically applied to our mesh to show what I mean in the layers.
[36:04] Let me go ahead and let's hide everything.
[36:07] And our texture set settings, we can see the ambient occlusion map that was just baked.
[36:12] If I click on the X icon to get rid of it, then you'll immediately see that the crevices aren't as dark.
[36:18] This is what we were working with before we added the ambient occlusion map.
[36:22] So I'll press control and Z because I do want that on the smash.
[36:26] If you don't like seeing the ambient occlusion map, maybe you think it's too strong.
[36:30] Then in the shader settings, we have AO intensity.
[36:34] So right now by default, it's set to 0.75.
[36:37] If I bring it down to zero, we're able to turn off or bring up to one to really exaggerate what it looks.
[36:43] So I'm just going to leave this towards this default of 0.75.
[36:47] Just because in our viewport, we can see the ambient occlusion doesn't mean that it's applied to our base color.
[36:54] And let me go back to layers and bring all my layers back.
[36:57] So the ambient occlusion isn't baked into our base color yet.
[37:00] Having the ambient occlusion in the viewport is just a visual change for us.
[37:04] It will not be in the exported textures.
[37:07] Unless we specify that in Unreal, which I will cover when we get to the Unreal Engine section.
[37:12] Okay, now let's cover how we can use these texture maps in our material creation process.
[37:18] And we can do that with generators, which are essentially advanced mass that we can add to our layer mass.
[37:26] These generators will only work if we did bake out these texture maps because they use them as inputs.
[37:33] Now one texture map.
[37:34] And again, we're going to go ahead and show the ambient occlusion map because this is the most important one.
[37:39] This is a really nice texture map since ambient occlusion is showing us the crevices of this mesh.
[37:46] That means we can probably use it to help better refine our dirt mass because dirt generally won't be everywhere in a mesh.
[37:54] You can expect dirt to build up in the crevices.
[37:58] So there'll be more dirt right here or dirt below the feet.
[38:02] So let's change our dirt mask to use the ambient occlusion map.
[38:07] What I will do is let's erase the fill effect.
[38:11] So click X and then come up to the add effect button and in the dropdown select add generator with the mass selected.
[38:21] Go ahead and select that.
[38:23] And now in the generators, I will type in dirt right there.
[38:27] So there is a built in dirt generator selecting that and we'll immediately see that it is using the ambient occlusion map to create a layer mass for dirt.
[38:37] Pull it down alts and clicking on the mask.
[38:39] We can better see exactly what the generator is creating.
[38:43] Now within the properties of this generator scrolling down, we can see that it is using the ambient occlusion map.
[38:49] We just baked.
[38:50] So this is absolutely amazing.
[38:53] We'll be using generators a bunch because they are so powerful and could help take our material to the next level.
[38:59] So obviously we can control its properties right here and you want to make sure you have the generator selected.
[39:07] So let's go back into the material mode and start refining the look of it.
[39:13] So a green down the dirt level to something a little bit less.
[39:16] Also, I'll bring down the dirt contrast because right now I think it's too contrasty and increase the grunge.
[39:22] So grunge is just the overall dirt level.
[39:25] That's how the dirt isn't just in the crevices.
[39:28] It's also elsewhere on the mesh and to control the opacity of the mask just like with the fill effect.
[39:34] We could come over here and instead of a passive 100 let's bring this down to something like 85.
[39:41] Now there is dirt where you would expect there to be dirt.
[39:44] So looking down here with the feet.
[39:47] Notice how the dirt is accumulating below the feet and within the crevices right here and between the body and the arm, which is pretty amazing and a lot more realistic than just placing a texture uniformly over everything.


### Premade Materials [40:02]
**Transcript (timestamped):**
[40:02] Now let's make use of another generator.
[40:04] But instead of it being used for dirt, it will be used for metal.
[40:08] So it will give you the appearance that in the past this object was originally metal.
[40:13] And then it was painted over with a glossy paint color.
[40:17] But over time and this model has probably been outside for a while.
[40:21] Slowly the paint has been shipped away and we're showing the base, which is metal.
[40:27] To do that we need a new layer for the metal.
[40:30] So I could come up to fill layers, create a new one and then down here bring down the roughness and then bring up the metallic to create a metal.
[40:42] And while this does work an easier way and a more customizable way is that I could just delete this and use one of the pre made materials that are included within substance within the asset browser.
[40:55] I want to select the category at the far left right here, which is the materials and then in search I'll type in metal and then let's use metal galvanize.
[41:05] So I could just drag this on my mesh or drag it into the layer stack.
[41:10] So this will add a really cool metal material that is already created for us.
[41:16] And just like with the textures and substance, I'm able to edit a lot of these materials properties already.
[41:22] So I can change the color and it changed how much variation there is the roughness and a bunch of other unique patterns to go ahead and play with a lot of these materials and see what's possible in substance.
[41:37] Now in my case, I'm just going to use the default parameters because I think they look good and we won't really see that much of the metal to begin with.
[41:44] Now I will right click and add in a black mask.
[41:47] And just like with a dirt, let us add a generator instead of coming up here and clicking on the add effect button generator.
[41:55] I can right click on this and then add a generator to the right click.
[42:00] So I'll select here and in generators instead of dirt type metal and select metal edge.
[42:09] So right off the bat, we can see that is giving us a really nice effect where only the edges or the sharp areas of my mesh have the metal exposed.
[42:20] So this looks really cool.
[42:22] And as you can guess, this will be using the curvature map.
[42:26] So going down here, the mesh maps here is the curvature map.
[42:30] And within the inputs for this generator, it is using curvature down there.
[42:36] So to better see my mask, hold on Alt and click on my mask to look at it.
[42:41] And I can play with these values until I get something that I like.
[42:46] By default, there is a little bit of grunge.
[42:49] The grunge is the equivalent of adding in a texture uniformly.
[42:53] It is not using the curvature.
[42:55] And maybe we want to get rid of that a little bit because I don't really want my metal to be shown everywhere on the mesh, like how it is right now.
[43:06] So going into the grunge amounts, I'll go ahead and decrease that to something like 0.2.
[43:12] This is what happens when I go all the way up and see how the metal is now everywhere.
[43:17] This is too much.
[43:18] We don't want that.
[43:19] So bring that down to 0.2.
[43:22] There is a big issue right now.
[43:24] And that is the metal should not be on top of the dirt.
[43:27] Dirt should be on top of everything just because this part of the mesh is metal doesn't mean dirt won't stick to it.
[43:33] So I'll go ahead and drag my dirt layer up here and let go.
[43:38] So now the dirt is on top of it for a more realistic blend.
[43:43] And just with four different layers, I'm able to create something really realistic like this.
[43:49] And that is incredible.
[43:51] Now, what if I want to make some adjustments to my metal mask that are not currently possible with a generator?
[43:57] For example, I want to add some scratches and have a lot of control over what those scratches look like.
[44:03] Right now, this mask is just using one effect, which is the generator.
[44:07] Now we will cover something that is absolutely incredible and will unlock a ton of new possibilities within Substance Painter.
[44:14] And that is layering effects.
[44:16] So we are not just limited to one effect.
[44:19] We can have multiple effects layered on top of each other to create a single mask.
[44:24] And to show what I mean, let's say I want to add a scratch mask now.
[44:29] What I can do is with the mask selected, come to add effect and then add a fill or just right click and add fill right there.
[44:37] So now we get another effect that is on top of the metal edge where and of course, I don't want a single color.
[44:45] Instead, I want the texture of scratch and use grunge scratches rough texture right here.
[44:52] Select this and alternative and faster way to add to this texture as an effect is to click on the X buttons.
[44:58] So let me just get rid of that temporarily.
[45:00] And over here, let's go to the texture category and find the same scratches.
[45:07] So right here grunge scratch rough.
[45:09] Just go ahead and drag it until you are hovering over the mask and let go.
[45:15] Now, obviously we have one big issue and that is my fill effect is now overriding the generator.
[45:21] I don't get the nice curvature mask that we just created to add effects on top of each other without one overriding.
[45:27] The next one, I can change the blend modes.
[45:31] Let's make this bigger and to see what blend mode is currently being used.
[45:35] It is to the left of the opacity.
[45:37] So right now it is set to normal and they want to add on top of a mask, then come down here and select linear dodge.
[45:45] So selecting that will blend the two together.
[45:47] So this is being added on top of that without replacing anything.
[45:51] This is before and this is after.
[45:55] So we're just adding a little bit of scratches and the benefit of separating them out into two different effects is that we have a lot more control.
[46:03] So I can make edits to the fill without affecting the metal edgeware.
[46:08] So I think I have way too many scratches.
[46:11] So I want to get rid of some of that by decreasing scratch quantity.
[46:16] So that's how we're just getting a few.
[46:18] And also I think the length is too much.
[46:21] These scratches should be just smaller.
[46:24] Which I can do by playing with the width and the length and also coming up here to tiling.
[46:31] And let's have this tile just a little bit more like right here.
[46:35] This is a very subtle effect, but it is adding a bit more character.
[46:41] Almost like this object has been thrown around and thrashed a bunch.
[46:45] Now that you know we can stack effects.
[46:47] A very common workflow in Substance Painter is to do a lot of the work creating masks by layering effects.
[46:55] Oftentimes you will see masks with four more layers.
[46:58] So let's do the same thing for the dirt because right now if I look at the dirt and actually let me increase this opacity to 100 so we can better see it.
[47:08] This is way too uniform.
[47:10] There is just a bunch of dirt in the crevices and there is no breakup.
[47:14] This isn't what you would expect.
[47:16] You would expect there to be at least just a little bit of breakup where there isn't areas with so much dirt in the crevices.
[47:22] So to get around that, let's use another texture specifically spots and it is black and white spots one.
[47:31] So I will drag this on the dirt layer and let go.
[47:35] This fill layer is overriding the dirt layer.
[47:38] We don't want that to happen.
[47:39] Instead, I want the black and white spots to subtract from the dirt layer.
[47:43] So where we get darker locations on this material, I want to take that away from the dirt.
[47:51] So that's how we don't get, you know, these pure white areas like we do in this location.
[47:56] Instead of using a normal blend mode, I will set this to multiply and these blend modes operates exactly the same as they do in Photoshop and other programs.
[48:06] If you do have a workflow that you like to use creating masks or textures and those programs,
[48:12] you can bring them over into substance painter.
[48:15] So by using multiply, you can immediately see that effect.
[48:20] So these pure white areas here is before and here's after it's just getting chopped up a little bit, which is exactly what I'm going for.
[48:30] Now, I think these spots are way too big.
[48:33] So under tiling, let's increase this.
[48:36] And also so we don't get those nasty seams.
[48:40] I'm seeing one right here changes to try planner projection.
[48:44] Okay, just like that.
[48:47] Now this dirt is looking a lot more realistic.
[48:51] Instead of being uniform, it's being chopped up a little.
[48:54] And I think it might be too strong.
[48:57] So what I'll do and actually, yeah, that is probably a little bit too strong is the opacity of this mask.
[49:03] Just bring it down to control it.
[49:06] So that's how we still get dirt in that area.
[49:09] But it's being subtracted from like right there.
[49:13] Okay, nice.
[49:15] You may have noticed that whenever we are using try planner projection, we get this little gizmo right here.
[49:21] This gizmo allows us to move around the projection of the texture in case we don't like the position of the texture for some reason when using try planner projection.
[49:31] So you can move this and you can see just a little bit of those changes and maybe find something you like.
[49:37] For the most part, especially when using natural textures, I find it's not very necessary to change the projection, unless you really want that control.
[49:46] So this is what our layer stack looks like right now.
[49:50] And once we start getting to really complicated materials, showing all these mask effects can take up a lot of space.
[49:57] So if you ever want to hide them, then you can come up here and just select the icon for the layer.
[50:02] So if you want to hide these select them.
[50:04] And then if I want to get back those effects, then click on the mask on the subject of blood modes.


### Blend Modes [50:09]
**Transcript (timestamped):**
[50:11] All of our layers have their own blood modes and opacity.
[50:14] So if I want to lower the dirt opacity as a whole, I can come over here and lower it like this to control exactly how much.
[50:23] Or maybe for example, I only want the arms to be half blue for some reason, then I can lower its intensity to 60, which is 60% its full opacity.
[50:34] And we have a blood modes, the exact same that we have for the effects.
[50:38] So instead of blending with a normal, I can come down here and select something like soft light, which is a difference from the normal blend mode.
[50:47] Because the math of how the colors are mixing are now completely different.
[50:51] But I'll just leave this at normal.
[50:53] It is also very important to point out that each of these different channels right here have their own blend mode.
[51:00] And we can see what those blend modes are within the dropdown.
[51:04] So by default, we are looking at the base color blend modes.
[51:08] If we come down to roughness, we can see the roughness blend modes.
[51:11] For example, if I only want to lower the roughness of the dirt for some reason and not have it affect any of the other channels.
[51:20] What I would do is come over to this dropdown and select roughness.
[51:25] Now for the dirt layer, I can come over here and just lower that opacity.
[51:31] And you can see exactly what it is doing at zero.
[51:34] It's the equivalent of essentially turning off the rough channel for the entire layer.
[51:39] And obviously that doesn't make sense because now the dirt is pretty shiny.
[51:45] But this is good information because it gives us a lot more control over my layers.
[51:50] So by increasing this, we can see the roughness start to come back.
[51:54] This opacity amount for roughness is completely separate from the other channels,
[51:59] so that is how we can get precise control over our channels.
[52:04] So I'll just go ahead come up here and leave it at base color, which is its defaults.
[52:10] If you are ever adjusting a layer and for some reason your properties aren't really working,
[52:15] then you might want to come over and then check out what the blend modes are for the different channels.
[52:21] Maybe there was a change there.
[52:23] Now it is time to cover another amazing feature of Substance Painter and that is how to organize layers into groups


### Smart Materials [52:24]
**Transcript (timestamped):**
[52:30] and how to create smart materials.
[52:32] So so far, we essentially just have one material that is made up of four different layers.
[52:39] Now if I want to organize this material, what I can do is come up to this folder icon to create a group
[52:45] and then holding down control, select multiple layers and drag them into this folder like that.
[52:53] So now we have one folder that contains all of our layers or if I press control and Z,
[52:59] a shortcut to doing that is to hold down control and select all the layers and press control and G
[53:06] to create a new folder from the selected layers.
[53:09] So what I will do is rename this to coated metal.
[53:13] Now we can think of the combination of all these different layers to be one single material because that is how Substance Painter works.
[53:22] We combine multiple layers with mass to texture our object exactly what we want.
[53:27] So since the textures of my object are just made up of different layers,
[53:31] that means we can save these layers and bring them between different Substance Painter projects to reuse all the work we already did.
[53:39] Because if we want a similar look to another mesh, why would we recreate the layers when we could just copy and paste them into a new project?
[53:46] And that is essentially what smart materials are.
[53:49] And we can see the smart materials that Substance Painter comes with by selecting this material icon.
[53:54] So smart materials are literally just folders of layers just like what we have with the coated metal.
[54:00] So for example, we have this machinery smart material.
[54:03] What I will do is drag it on my object or drag it into my layer stack and let go.
[54:09] Instead of this being a single layer, this smart material is a group of layers.
[54:14] So if I hide all the top layers, we can see the base is just a simple yellow fill layer.
[54:21] And then the dirt is another layer that is using a mask of the ambient occlusion.
[54:26] Holding down Alt, we can see exactly what this mask is.
[54:30] And Substance Painter is smart enough to already automatically input the mesh maps that we created for this model.
[54:37] So it's not using the original mesh maps for whatever project.
[54:41] It is using the mesh maps of this project.
[54:43] And then above that, we have dust, which is a also very subtle effect.
[54:49] We can see what mask it is creating.
[54:51] And this is a positional mask.
[54:53] We can select the mask builder to see exactly what they're using to get this feature.
[54:58] It is masking in the parts of the mesh that are facing up in the Z direction because dust will congregate at the top of the mesh and not on the sides.
[55:08] And finally, they added a rust layer.
[55:12] Maybe I don't like this machinery group.
[55:14] Let me scroll.
[55:15] Let me scroll.
[55:16] And I can also check out this wooden hole smart material by dragging it onto my mesh and let it go.
[55:22] So now this is an entirely different group of unique layers.
[55:27] And as we can see, this layer group is a lot more complicated than the one we created and the machinery layer group.
[55:34] So this is the power of smart materials.
[55:37] We can just drag them onto our model.
[55:39] And then already it will use the baked mesh maps.
[55:42] So you need to make sure you bake the mesh maps before using smart materials to start assigning different layers.
[55:48] So already we are pretty much 70% of the way there and it makes a workflow for using substance painter a lot easier, especially if we have certain materials.
[55:57] We're going to be using over and over again.
[55:59] The way we can use this right now is let's say and let me delete the new smart material and the machinery one just so that I have the wooden ship material.
[56:09] For example, if I just want the body here to be wood and the rest of the mesh, my original material, then I can add a mask to the group.
[56:18] So instead of masking out an individual layer, I can mask the entire group.
[56:22] So let me add a black mask to this.
[56:25] And just like beforehand, I will use the polygon fill tool and just masses in with a white color.
[56:33] With this mass for the material group as a whole, I'm able to just place the wood on the body and not the rest of my material.
[56:42] This is the main workflow I use for substance painter.
[56:44] As soon as I get a new object, I bake the mesh maps and then I go through my smart materials and see which ones I want to use.
[56:51] After dragging them out to my object, I can always go into the layers and edit any properties I want to use.
[56:57] Not to mention smart materials are an amazing learning resource.
[57:01] If you want to know how to create realistic materials and substance painter, then you could just go through these layer groups and see how they were created.
[57:08] In addition to the smart materials that ship with substance painter, we also have a bunch of smart materials created by the community.
[57:15] If we go to Adobe Substance 3d Community Assets and scroll down here to smart materials, here are a bunch more materials we can play with and add to substance painter.
[57:25] And all these are free because they're created by the substance community.
[57:29] Now to create my own smart material so I can reuse the material we've made throughout this tutorial in another project on another object.
[57:37] Then what I will do is let's go ahead and close this.
[57:40] So it's on my way and right click on any layer group down here, select create smart material.
[57:47] Now a new smart material will pop up in my smart material category and that is our material and whatever name we call the folder.
[57:56] Now in any new project, I could just go to my smart materials and grab the material we created and drag it on a new object and boom.
[58:05] Instantly all the work we did in that project can be carried over onto an entirely different mesh, which is absolutely incredible.
[58:12] You just want to make sure that you bake your mesh maps before using this smart material.
[58:17] You will notice that the entire toad is blue.
[58:20] That's because the only part of this layer stack that was specific to the original mesh where we painted according to the meshes geometry and the UVs was the blue layer right there.
[58:30] So substance painter doesn't know what to do.
[58:32] So it just assigned white to this entire mask.
[58:35] If I want to get rid of this, I can always delete the layer or hide it.
[58:39] Or what I can do is let's go ahead and remove the mask and then add back a mask but make it black.
[58:47] So using the paintbrush or the polygon fill tool, I can add the blue accent color to different parts of this frog.
[58:56] Hopping back into my original project because that was just a demonstration.
[59:00] What I will do is let's delete the wood chip hole.
[59:04] So we're working with what we originally had.
[59:06] Now throughout this tutorial, we have not done any painting so far with the brush tool, which is surprising given the name of the program is substance painter.


### Paint Tool [59:07]
**Transcript (timestamped):**
[59:15] It goes to show that the majority of our work will be editing the layers and textures in order to get fine control over our materials.
[59:23] We need to use the brush tool, which unlocks a whole new level of creativity.
[59:28] So let's cover that right now.
[59:30] Currently, I cannot paint anything because we don't have a paint layer or paint effect selected.
[59:36] So to create a paint layer, I can come up here to the paintbrush icon and select it.
[59:41] This will create a new layer.
[59:43] What I want to do is make sure that this is at the top of my layer stack.
[59:46] So when I paint, it is on top of all my materials.
[59:50] This is also the default layer you will get when you create a new substance painter project.
[59:55] So now let's cover what the controls are for the brush.
[59:59] And in case your brush looks different, you could select the default brush that we have by clicking on the brush icon in categories and selecting basic soft.
[60:10] This is the main brush, which we will automatically get at first.
[60:14] And you can see in the middle here, we have a little preview icon.
[60:18] If you don't see the preview icon come up to here and select full preview cursor.
[60:23] I like seeing this because it shows exactly what we are going to be painting.
[60:27] There are three different places where we can change the brushes parameters up here on the toolbar.
[60:32] I can change its size, the opacity and the flow, which we will cover in just a moment.
[60:37] Or down here with the paint layer selected, I could change the properties also within this window.
[60:43] And here's a really cool shortcut to quickly get this exact same window when painting.
[60:48] And that is right clicking.
[60:50] So right clicking will also bring up the properties paint window.
[60:54] So I can quickly access it because odds are you will be changing these parameters a lot.
[60:59] Or if I press tab to hide my user interface, now I can still get those properties by right clicking.
[61:06] So very cool. You might see me do that a bunch throughout this tutorial.
[61:10] Obviously, one of the fundamental controls for a paintbrush is the size.
[61:15] So if I want to lower the size, I could come up here to size and decrease it.
[61:19] So I get a much more fine brush or the shortcut is to use the bracket keys, same as Unreal.
[61:25] So right bracket key to increase it or left to decrease it.
[61:30] But oftentimes in Substance Painter, there is another shortcut to increase and decrease the size.
[61:34] And that is to hold down control and then hold down the right mouse button.
[61:38] So control and right mouse button held down at the same time.
[61:41] And then you want to move your mouse to the right to increase it or move your mouse to the left to decrease it.
[61:47] So that is control right mouse button, mouse, right or mouse left to increase and decrease the size.
[61:54] Another property you might want to control is the hardness of the brush.
[61:58] And I'll press control and Z a bunch to get rid of my strokes so we can better see my brush right now.
[62:03] And within the properties scrolling down under alpha, we have this hardness parameter.
[62:09] So if I increase this, we get a much sharper brush than before when it was really soft.
[62:16] The shortcut for hardness is control right mouse button again, but instead of moving it right or left,
[62:21] we're going to move it up or hard and down to make it softer.
[62:25] So that's up and down instead of right and left for size.
[62:29] And if you ever forget what a shortcut is, because substance painter does have a bunch of shortcuts built into it,
[62:35] then you can just hold down shift, control or alt.
[62:38] For example, let me hold down control and down here in the bottom left hand corner,
[62:42] we will see all the shortcuts associated with control.
[62:45] You can see that we have control right, which changes the tool size and the hardness,
[62:50] which is the shortcut we just covered.
[62:52] Also on the subject of alphas, alphas are the texture you are going to paint.
[62:56] So this is the default alpha that comes with a basic brush, which is just a soft circle with a fall off.
[63:02] If I go over to the alpha category, which is next to the brushes, then we get a bunch of other options to choose from.
[63:09] So instead of a circle, I can grab the arrow long and then drag it into the alpha and let go like that.
[63:15] So now I'll just be painting this and placing that down.
[63:19] So just a single click will add a single stroke or I can hold down my left mouse button and then paint with the arrows.
[63:25] I'll press control and Z because if I want to now rotate this, that's how my arrow isn't always pointing to the left of this object.
[63:32] Then down here under direction, I can move it.
[63:35] So that's how it's painted this way like that to the right.
[63:39] And the shortcut to rotate an alpha is control and instead of the right mouse button, hold down the left mouse button and move the mouse up and down.
[63:48] So control left mouse button up and down to change the rotations.
[63:53] And you might have noticed that whenever I'm making changes to my brush within my settings, those changes will also be shown right here within this window.
[64:01] And if you ever want to test out a brush without testing it out directly on the mesh, you can come here and then hold down left mouse button and you can paint directly in that window, which is super cool.
[64:11] Now I will cover flow and opacity.
[64:13] So I want my default brush back.
[64:16] I'll go ahead and double click basic brush to grab that and press control and Z for a blank canvas.
[64:22] Stroke opacity will control the strength of my brush, just like how we're able to control the opacity of the channels of my layer right here.
[64:30] So if I bring down a stroke capacity to 50%, now this is at 50% strength, we can still see the original color below this layer.
[64:39] But you will notice that if I hold down my left mouse button and create a single stroke and still with my left mouse button held down, move my mouse over the original stroke.
[64:50] That we're not increasing the opacity.
[64:52] The opacity is capped at 50%.
[64:55] I have to let go of my mouse and then create another stroke.
[64:58] And when I move over previous strokes, now we are increasing opacity.
[65:03] And while this can be good for certain situations, if we are painting a bunch, this can feel unnatural, which is why I'll press control and Z.
[65:12] Instead of using stroke capacity, we generally use flow, which is similar to opacity.
[65:17] Except now, if I have a single stroke, and the stroke goes up and down, and my brush overlaps with itself, it will increase the opacity.
[65:26] So with a flow super low, like 10.
[65:29] Now if we hold down left mouse button, I can paint.
[65:32] And then if I paint over, we'll see that opacity increasing.
[65:35] So this creates a much more natural looking paint and feeling.
[65:40] So if you are going to be paying a bunch, I recommend to use flow and not stroke capacity, which is why the shortcut is not stroke.
[65:46] So that's why the shortcut to decreasing the strength of my brush is for flow.
[65:51] So holding down control and the left mouse button, if I move my mouse horizontally to the left, we decrease flow, and then moving it horizontally to the right, we increase it.
[66:02] So that is control, left mouse button, mouse right to increase and decrease it with left.
[66:08] Some more important parameters for the brush is spacing.
[66:12] If I better see this, I will increase my hardness and increase spacing to something crazy like 150 in between when my brush is stamped will be longer.
[66:22] What I mean is that if I create a stroke, we can see that now the stamps are very noticeable of the alpha.
[66:28] And by decreasing this to a value of 20, this is what gives us that smooth looking feel to our brush.
[66:35] But it is still noticeable depending on the alpha.
[66:38] So if we use the arrow alpha again, select that with a spacing of 20, it is noticeable that this is an arrow.
[66:45] So decreasing it to something like four, we'll smooth that out a bunch.
[66:50] For some brushes, you want a low spacing and for other brushes, you want a high spacing, especially if you want to add in a bunch of randomness to your brush, which is what I'm about to do.
[67:00] So I will set this to 100 and you even see the spacing change in real time within my brush preview.
[67:07] So saying this to around 100 coming down to the jitter options, I'm able to change the look of the brush, for example, the size, increasing this to 100.
[67:18] Now each of my stamps will be a different size doing the flow will randomize its opacity.
[67:25] So some of the strokes are fairly noticeable while others are at 100.
[67:30] Of course, as you can guess, angle will give the alpha a random angle and position will really increase that randomness.
[67:39] So now my brush is all over the place.
[67:42] And by combining all these parameters, we could get some really unique looking brushes.
[67:48] And luckily for us, substance painter already comes with a bunch of brush presets we can already use.
[67:54] So learn press control and Z to go back.
[67:56] And one of my favorite brushes if I select this is the dirt, and it is dirt to so selecting this brush and we can see that's making heavy use of the size and angle jitter.
[68:07] Now I can very quickly paint some realistic looking dirt for an organic looking feel to our model.
[68:15] So go ahead and see what brush presets you like and what is possible.
[68:20] Now, that's the entire time we've been covering how the brush works, but the brush is just the first part of the paint layer.
[68:26] The second part if we scroll down is the material section.
[68:30] So we're not just painting in color right now, we're painting in an entire material.
[68:35] So we're painting the metal rough normal and height.
[68:38] If I come to metal and increase this to one, we can see the preview of the material that will be painted.
[68:44] Now I'm going to go back to basic soft.
[68:46] And now I am painting what looks to be iron or changing the color.
[68:51] I can make this let's go just a little bit of an orange, orangey yellow for gold.
[68:57] And now I am painting gold.
[69:00] If I just want to paint very specific channel, for example, if I just want to paint roughness, then I can disable all the other channels and just have roughness or the shortcut is holding down Alt and clicking on a channel to enable the
[69:06] channel and disable the rest.
[69:08] So Alt clicking on roughness will enable that.
[69:11] And then if I come down here with a really low roughness, I can start painting in a lot of shine that we can see at the right angle.
[69:16] Okay, so I'm almost like painting in what looks to be puddles or making the entire model wet by painting that in here.
[69:23] Now, what we're going to do is we're going to go ahead and do a little bit of a roughness.
[69:27] And then we're going to go ahead and do a little bit of a roughness.
[69:30] What looks to be puddles or making the entire model wet by painting that in here.
[69:35] Now, we are not just limited to painting in uniform colors and values.
[69:40] We can also paint in textures and entire materials.
[69:44] So if I go to the material section, I will choose this fabric linen or any of these and just simply drag it onto the material mode in my brush settings and let go.
[69:54] So now if I increase my brush size, as I start to paint, you'll see that I'm just going to go ahead and do a little bit of a roughness.
[69:59] So if I go ahead and start to paint, you'll see that I'm painting using the textures of the material, which is a pretty unique workflow.
[70:07] If I ever want to get back my original brush, then I could come over here and select the X icon to remove the material, go to brush, and then select my basic soft to get it back.
[70:19] Now, obviously, this model looks like a complete mess because of our paint layer and this layer was just for demonstration.
[70:26] So if I go to the elite key, I will create another paint layer again, because now that we know we could paint materials.
[70:33] This is why some of the brushes here are unique, like the autumn leaf brush, because we are not just painting a single color.
[70:40] Instead, we are alternating between a material.
[70:43] So at the bottom of this object, I can place this around with this.
[70:48] I'm painting a pile of leaves at the base here.
[70:51] Or there's another cool one, which is this Ivy branch brush that I can now start painting on Ivy's for the character.
[70:59] As you can see, the paint brush is really versatile and powerful.
[71:03] But the main way we use the paint brush is for painting mass.
[71:08] So let me X out of here and just temporarily I will add in, let's say this rock face material to the top of my layer stack and increase the tiling just a bit.
[71:19] So for example, maybe I want only rocks on the belly right here for some reason.
[71:24] Then we add in a black mask.
[71:27] And now with the paint tool, I'm able to paint in or manually edit the mask with a paintbrush like this.
[71:35] By selecting the mask with the paintbrush, I am now able to paint in that material holding down alt on the mask to see what is happening.
[71:45] And then to paint away the material, instead of painting white, we paint pure black.
[71:51] So I move this slider all the way down to the bottom to paint away.
[71:56] And that is a very common workflow in substance painter, having to switch in between zero and one when we're painting mass.
[72:02] So that's why we have this button right here to invert it from one to zero automatically, or I could press the X key to invert.
[72:10] So that's X when it's white, I'm able to paint it in and then press X again to now chop away at the mask.
[72:17] So this is how we paint mask in substance painter.
[72:20] But generally, I don't recommend painting directly on a mask.
[72:24] Instead, what I recommend you is to create a paint effect for the mask and then paint on that effect.
[72:30] The reason why is because this will be a lot more versatile and give us a lot more options down the line to make changes.
[72:36] So best to show what I mean with that example.
[72:39] First, I'm just going to clear this. So right click and then select clear mask.
[72:43] So I just get a black mask again.
[72:45] And now with white by pressing X to invert my brush, I will hold down control, right mouse button and really increase my brush to make this super hard.
[72:54] So I'll come in here and instead of directly painting on it, I'll come up here to the effects tab and then add a paint.
[73:02] So select that to add a paint effect.
[73:04] And it is within here.
[73:06] I'm now going to paint my changes on the belly like that so I can hide and unhide to see what this is doing.
[73:14] So we didn't paint directly on the mask.
[73:17] Instead, we painted on this layer right here.
[73:19] The reason why is now let's say in the future, I'm like, oh, this is way too sharp.
[73:24] I want to go into the mask and I'll make the fall off much more natural.
[73:29] Then I would have to come in here with a brush, make it really soft and then just try to paint all those changes.
[73:36] Or what I can do is leverage all the effects that we have in substance painter and apply those effects to the paint layer.
[73:44] So I'll come up here to the magic one icon again, add a filter and then we will just use the blur filter.
[73:51] So go ahead and select that.
[73:53] And how we can immediately see what is happening.
[73:55] I can increase the blur to soften my paint or decrease it.
[74:00] And this blur is right on top of my paint.
[74:03] So it's directly affecting what I do here.
[74:05] So let me hop into material mode and we can better see exactly those changes.
[74:11] So I can start to layer effects on top of my paint layer to supplement my painting because I have the blur with the paint selected.
[74:20] I can still go in here and paint a bunch and then it will automatically have that blur effect on top of everything.
[74:27] So this is a really powerful way to paint in mass and we can still leverage all of substances, nice procedural features.
[74:35] A practical example of using the paint effect that we can immediately start using is to gain extra control over the texture mass that I'm using specifically for the metal.
[74:46] So I'll go ahead and let's delete that layer and then go here to my metal.
[74:52] If you remember we are creating the metal mask through first adding in the mesh map curvature, adding the metal to the edges of my object.
[75:01] And then on top of that, I'm adding in some scratches.
[75:04] So this is without the scratches and then this is with.
[75:08] So the main way I use the paint tool is to help get fine control over my mass.
[75:14] So for example, let's say I don't really like this scratch right here and I want to get rid of it.
[75:19] Well now up here in the one icon I can select paint or right click on my mask and select paint to add in a new paint layer.
[75:28] So with this paint layer, I can go in with a black brush and then start to paint away exactly what I don't want from this mask.
[75:37] So I could go ahead and remove that entire scratch or increasing the harness and decreasing the size.
[75:44] I could start to paint in my own scratches.
[75:46] So pressing X to get white.
[75:48] Now I can paint across to get the exact look that I want.
[75:53] So when you are building out your mass in substance painter, just know that you aren't limited to your textures or procedural tools in substance painter.
[76:02] You could always go in with a paintbrush and make any manual adjustments you need.
[76:06] To fine tune your model and create exactly what you want.
[76:09] Substance painter is really customizable.
[76:12] You are not limited to any workflow.
[76:14] Now that we have the basics of painting down, let's do something practical with it for our model.
[76:20] And that is specifically to paint a little cartoony face on our character's head.
[76:24] So this will be really fun.
[76:26] And also if you are following along with this tutorial, this part will be pretty easy.
[76:31] So you can follow along and create your own little cartoony face.
[76:34] You don't have to follow along exactly with me for now because this is up to artistic interpretation.
[76:39] So to begin, I want to create a new layer specifically just to affect the color.
[76:44] So I'll go ahead and let's close my group, create a new fill layer and make sure this fill layer is outside of my group.
[76:51] And this will only have color selected.
[76:54] Hold down Alt and clicking on color.
[76:57] Now the rest of my channels will be left alone.
[77:00] I'm also going to come up here at a black mask.
[77:03] And like I said beforehand, just in case if I want more flexibility in the future, I'm going to do all my painting within a paint effect layer.
[77:12] And with my brush, I will make this hard like that.
[77:17] The reason why I'm setting up my layers like this and not just directly painting on another paint layer is that when I paint down a color like here, that color is there forever.
[77:27] It's going to be really hard to change it.
[77:29] Meanwhile, if I paint using a mask, so I'll come in here and paint my color like that.
[77:35] Now if I want to change my color, it's very simple.
[77:38] I just come into here, go to base color and now I can change it so I can still do a bunch of painting and make changes.
[77:45] And if I don't like the color, I can always go back here and change it.
[77:49] So for this color, I'm specifically going to do something like a dark black like that.
[77:55] And then I'm going to delete all that because that was just an example.
[78:00] And one thing we need to cover now because I want to paint the character's eyes is that if I make changes to this side of the mesh, I also want to carry over to the next side.
[78:09] So that is where cemetery comes in within the paint tool up here.
[78:13] I could click on the symmetries button and now we're going to get a red line going down my model.
[78:18] So this red line tells me that if I make any changes to the side, then that change will be shown on the left side.
[78:24] We also get a bunch of different options up here.
[78:26] If I click on the gear icon, I could change the direction of the cemetery or even the location of it by moving the gear.
[78:35] So I'll click on this button to reset it because I do want it at the zero location.
[78:40] This works fine.
[78:42] Now I want some really smooth strokes.
[78:45] Let me get rid of this and show you what I mean if I decrease my stroke size, make it super small.
[78:51] And now if I try to create a smooth line, we can see it is pretty jagged because I am limited to the ability of how smooth I can move my mouse around.
[79:01] So to get a smooth paint coming up here, I can select on this distance button.
[79:07] So now you see that there's a larger darker circle that is encompassing my circle.
[79:13] And this tells us how smooth this stroke will be.
[79:16] So now as I do a stroke, we can see that there is a very smooth line going with it.
[79:22] And then I can control how big that circle is up here.
[79:25] So decreasing this or increasing it.
[79:29] So with this, I can get some really unique patterns and I don't have to worry about how fidgety my hands are throughout this entire process.
[79:37] You might see me make a stroke and I don't like it.
[79:39] So I press control Z and I try again.
[79:41] That's just the artistic process.
[79:43] You can expect to do a hundred controls these a day.
[79:46] So with distance turned on and cemetery, I will first start with the eyebrows.
[79:54] And then add in some oval shaped eyes.
[79:57] Turning off distance.
[79:59] Go in here with a brush and fill it all in black.
[80:03] Now time for the mouth.
[80:04] I will disable cemetery turned back on distance.
[80:09] And he will be frowning.
[80:11] He's had a bad day.
[80:16] And now time for the pupils.
[80:18] What I'll do is let's call this layer black to duplicate a layer, press control and D at the same time.
[80:24] So that's control D to duplicate.
[80:27] I'll make this layer white.
[80:29] And since it is carrying over the mass from below it, I need to reset its paint layer.
[80:35] So go ahead and delete the paint effect and then add back a paint and let's call this layer white.
[80:43] Okay, with cemetery turned on and distance again, I'll come in here with the white brush.
[80:50] And draw another oval for its pupil.
[80:58] Now you may find that it's actually easier to draw in 2D view mode.
[81:02] Coming up to here, go to 3D and 2D.
[81:05] And now we can see that angry face in the top right hand corner.
[81:09] And let me go ahead and let's make this guy a little bit bigger.
[81:12] So we can see that the changes carry over in real time.
[81:15] So zooming in here, I can still make some changes.
[81:19] And then notice how in the 3D viewport we're able to see what it looks like.
[81:23] Also, you can set the view mode to face color.
[81:26] So we're just focusing on the color and we don't have to worry about the lighting getting in the way when we're painting.
[81:32] So that is another neat tip.
[81:34] Now you will notice that the UVs are kind of tilted in the wrong direction.
[81:38] That's okay.
[81:39] If I want to paint in the correct direction, then I can hold down Alt and the left mouse button to then rotate my UV map.
[81:47] So that's Alt left mouse button to rotate a UV map.
[81:51] And then I can zoom in here and try to get the angle correct.
[81:55] And then start painting in here.
[81:57] Now, in my case, I do enjoy painting in 3D.
[82:00] So I'll just go into the 3D only view mode.
[82:04] And finally, for the last color, press Ctrl D.
[82:08] Although you could add as many colors as you want.
[82:11] I'll call this red.
[82:12] And we will make this just a little bit of a reddish brown color.
[82:17] Get rid of the paint effect and then add in a new one.
[82:21] Still with cemetery turned on.
[82:23] Let's go in here and let's give him some cheeks.
[82:27] And I will want this to be below the eyes.
[82:30] So let's grab this layer, move it down.
[82:34] And also this is not red.
[82:36] So let's make this a little bit more pinkish, orangey.
[82:41] There we go like that.
[82:42] And then make sure to fill it in.
[82:48] Okay, there we go.
[82:49] So now we have a nice little face for our character.
[82:52] And honestly, it breathes so much more life into this model.
[82:56] I'll go ahead and turn off cemetery and to organize what we've done.
[83:01] Hold down Ctrl and grab all the layers.
[83:03] Press Ctrl G add them to a group.
[83:05] And I'll call this painted face.
[83:08] And just like that, we are done with this model,
[83:12] which helped us learn the very fundamentals of substance painter.
[83:16] So we started off by creating this material.
[83:19] And then we learned painting to go ahead and add in a little face.
[83:24] Now that we have a material, let's cover how we could bring it into unreal.


### Import Textures to Unreal [83:25]
**Transcript (timestamped):**
[83:28] And once it is inside of unreal, it could be used for anything,
[83:31] whether that be games or animations.
[83:34] Now this is not introduction to Unreal Engine 5.
[83:37] I do assume that you know the very basics of the engine.
[83:40] If you do not, then you're in luck because you can watch the UE5 beginner
[83:44] tutorial on this channel.
[83:46] There's a link to it in the description below.
[83:48] Before we can import our textures and create the material,
[83:51] let's first import the static mesh.
[83:54] So this object right here, because obviously these textures were created
[83:57] for this specific object.
[83:59] Getting out of here, I have a blank Unreal Engine project.
[84:03] I'm just using the basic level.
[84:06] And what I did was scale up the ground.
[84:08] That's how it's a lot bigger than Unreal's defaults.
[84:12] So with this blank project in the downloadable content,
[84:15] I will grab that same 3D object.
[84:18] So here are the downloaded content.
[84:21] It is called Meat Mat.
[84:23] So in the content drawer, I'll open this up and then go to a folder
[84:27] I made called Meshes and simply drag that in here like this.
[84:31] So now we have a bunch of options for importing.
[84:34] Generally, I keep everything at default, except if I scroll down.
[84:38] Under materials, we have this import materials.
[84:42] I like to turn that off and for textures.
[84:44] I like to turn off import textures.
[84:46] I find this Unreal will try to create its own material for us,
[84:50] but I already know what textures I'm going to use and what material I will use.
[84:54] I turn them off so we are just creating the static mesh and now select import.
[85:00] So here is our cool little character.
[85:03] I'm going to drag in here.
[85:05] There's our little guy.
[85:06] But of course, where are his textures?
[85:08] Where is the material?
[85:10] So now hopping back into Substance Painter,
[85:12] it is time for us to finally export them into Unreal and use it in a practical situation.
[85:18] Now, before I export for Unreal Engine, you want to come up to Edit, Project Configurations.
[85:24] And if you remember when we created this project, we turned on DirectX
[85:29] and turned on Compute Tangent Space per Fragment.
[85:32] So you want to make sure these two settings are selected before exporting
[85:36] because Unreal needs them on.
[85:38] Now to export a texture, come up to File.
[85:41] Come down here to Export Textures or the shortcut is Control, Shift and E
[85:46] to bring up the Export Texture window.
[85:49] These are the default export settings for Substance Painter.
[85:52] And we will be exporting the textures for one material
[85:55] because remember there's only one material on this object.
[85:59] And if we come up to the Texture Setlist, we'll see that that one material is called Material.
[86:04] So to see the textures being exported for it, I will select the name of the material
[86:09] and Substance Painter. They are called Texture Setlist.
[86:12] And here's a list of all the textures that will be exported by default.
[86:16] Now, I already know I'm not going to export any high texture.
[86:19] We will cover that later in this tutorial.
[86:22] Also, we will not export the mixed AO, which stands for Ambient Occlusion.
[86:26] I will cover Ambient Occlusion in just a bit, but that is an optional mask
[86:31] that isn't necessary for our materials.
[86:34] The core materials we always want is the color, metallic, roughness and normal.
[86:40] Now you also see that we have normal underscore direct X.
[86:43] This is the normal map we want.
[86:45] So I'll uncheck the default normal map.
[86:47] Another thing we can change is the size of the textures.
[86:50] Throughout this entire tutorial, I have been creating 4K textures.
[86:55] Now, if I want to increase the Texture Set, for example, if I want to export 8K textures,
[87:00] then I can select them right here.
[87:02] Honestly, 8K is probably overkill, so I'll leave them at 4K.
[87:06] Because Substance Painter is non-destructive, we could have been using 1K textures
[87:11] this entire time.
[87:12] And then finally, when we get to the export window, I can upscale that to 4K,
[87:17] and we won't lose any quality or data.
[87:20] Okay, to select where I want to export these textures,
[87:23] under Global Settings, we have Output Directory.
[87:26] I will click on this.
[87:27] And then navigate to a folder I created on my desktop called Exported Textures.
[87:32] So I'll select that.
[87:33] And now I'm ready to export.
[87:36] Opening up that folder, here are the textures that Substance Painter created.
[87:41] We have our base color, metallic, normal map, and the roughness.
[87:49] Now let's bring them into Unreal.
[87:51] So I'll go ahead and exit out of here.
[87:53] And then within the Textures folder, I'll go ahead and select all my textures
[87:58] and then drag them into the folder and let go.
[88:02] Okay, there we go.
[88:03] Don't forget to save everything with Ctrl Shift S.
[88:06] And now this is very important for all of my mass textures,
[88:09] specifically my roughness and metallic textures.
[88:13] We're going to go into them.
[88:15] So double click to see the properties.
[88:17] And you need to make sure sRGB is turned off.
[88:20] So for the metallic map, turn this off.
[88:23] And then for the roughness map, also turn this off.
[88:26] These are the only settings you need to change.
[88:28] Because Unreal was smart enough to know with a normal map to set this texture
[88:33] to the normal settings so we don't need to do anything here.
[88:36] You also notice that the normal map isn't really that detail.
[88:40] Only have normals where the metal is.
[88:42] That is okay because in the next project we are going to create,
[88:45] we're going to create a detailed normal map and height map and go over
[88:49] how to use them.
[88:50] So now that I have my textures, let's exit out and create a new material.
[88:55] So I'll go ahead and actually let me create a new folder, call this materials.
[89:01] And then right click, create material right here and call us M underscore meet Matt.
[89:07] Just like that and double click to open up to bring up my material view.
[89:12] If you are watching this in the future, the material editor might look a little bit different.
[89:17] This is because Unreal is transitioning to a new material editor for our purposes in this tutorial.
[89:23] Don't worry, all the inputs are exactly the same.
[89:27] So go ahead and hook them up like normal in this video.
[89:31] We can see that at the top we have our core channels for base color metallic roughness
[89:36] and then towards the bottom normal maps.
[89:39] So I'll now go ahead grab all my textures holding shifts and then selecting the last texture to grab all of them.
[89:46] And drag them in and let go.
[89:48] So my base color goes into base color, of course, as you can guess, and then my roughness here.
[89:55] And I could see that's called roughness.
[89:57] We'll go into roughness, normal into normal and finally metallic into metallic.
[90:04] Press apply.
[90:06] And now get this material and drag it onto my mesh.
[90:12] Let go and boom.
[90:14] Wow, all the work that we've done throughout this entire tutorial do create this cool material.
[90:22] And honestly, this material looks insanely good running in real time in Unreal Engine.
[90:27] So this is our little angry guy that we can now use in any of our environments.
[90:33] We can see what it looks like in different lighting setups by holding ctrl l to move the light in Unreal Engine zooming in onto my character.
[90:42] We can see all those fine little details that we got from the mass like the scratches, the edgeware and the dirt that's being built up in the crevices.
[90:54] Honestly, creating textures and assets for Unreal have never been easier than now.
[91:00] Now, exporting using the default substance painter settings are completely fine.
[91:05] There is nothing wrong with doing it this way.
[91:07] You will get great quality.
[91:09] But substance painter also comes with the ability to export textures specifically for Unreal.
[91:15] And we can see what that is by pressing ctrl shift and E to go to the export settings again.
[91:20] And then for the template, let's pick the Unreal template.
[91:24] So coming down here to Unreal Engine four, go ahead and select that probably in the future.
[91:30] They will rename this to Unreal Engine five, but four is good for now.
[91:35] And now in the materials, we'll see what is being outputted.
[91:39] We still have the color texture.
[91:41] We have a normal texture.
[91:43] But now we have this unique texture right here.
[91:46] We can't really see what it is.
[91:48] But if I hover over my mouse, you can see the name of it.
[91:51] And it is called occlusion roughness metallic.
[91:54] That is a really long name.
[91:56] It is a handful.
[91:57] But let's see what this gives us.
[91:59] And we have an emissive map and a missing map is necessary.
[92:03] If there are lights in my material, there are no lights.
[92:06] So I'll uncheck that because we don't need export it.
[92:09] So now let's export this.
[92:11] And we will see that we have three new textures right here that was exported using the Unreal template.
[92:17] So I'll go ahead and let me create a new folder called this Unreal templates.
[92:23] So we don't confuse the textures and outdrag all of this inside of here and let go instead of giving us a roughness or metallic mask.
[92:32] It gives us this really unique funky mass that if I double click on, we could see what it is.
[92:38] And since this is a mask, you want to make sure that sRGB is turned off.
[92:42] The only difference between exporting with the default settings and the Unreal settings is that it will pack the necessary mass into a single texture.
[92:51] So if I uncheck the red channel and the green channel, we'll see that this is our original roughness mask.
[92:58] Or if I uncheck green and check blue, this is our metallic mass.
[93:02] So all it is doing is just taking these two masks and combine them into a single texture for us, which can be easier to use when creating a material.
[93:12] And it just helps with memory when it comes to game streaming and optimization.
[93:17] We also have a red channel, which is the ambient occlusion I will cover in just a moment because the main channels are the roughness and the metallic.
[93:27] Now let's create a brand new material.
[93:30] Right click new material, call this M underscore new mats, double click to go inside of this.
[93:37] And the way we would use that is we will plug up the base color the same.
[93:43] The normals the same.
[93:45] So plug it up right here.
[93:48] And then drag out this big mask.
[93:52] Now if I want to grab any of the channels individually, I would drag from the RG and B.
[93:58] And according to the name of this hovering over, this is called occlusion roughness metallic.
[94:04] So that tells me that the first channel here is the ambient occlusion map.
[94:08] The second channel is the roughness mask.
[94:11] And the third one blue is metallic.
[94:14] So dragging from green will go into roughness and blue will go into metallic.
[94:20] I'll press apply.
[94:22] And now let's take that new material and drag it onto the meat mat on the far left.
[94:29] And when I place it here, we can see that there was no change.
[94:32] The only difference between these two materials is that one material is packing their mass into a single texture.
[94:39] Well, the other one has those textures separated.
[94:43] So it is up to you and the workflow you want to use, whether or not you want to pack everything into a single mask or have them be separate.
[94:51] Now this can be a tedious workflow, especially if we're creating hundreds of objects and substance painter.


### Master Material [94:52]
**Transcript (timestamped):**
[94:57] Every time we import the textures in, we then have to right click create a new material, import those textures, drag them in, and then connect all the nodes.
[95:07] And what if I want more control over this material because right now it looks good, but maybe in different circumstances, I want to change the contrast to hue or even decrease or increase the roughness values of my model.
[95:21] Then I would have to edit the materials with even more features.
[95:25] So luckily for you also included in the downloadable content is this master material I made to make the process of using substance payer materials a lot easier.
[95:35] So we will open up this project.
[95:38] The only thing this project contains is the master material.
[95:41] If I want to grab the master material and move it into my original project, right click, go to asset actions, select migrates, hit OK, and then navigate to the folder of the umbral project you are importing into and select its content folder.
[95:56] So I'll go ahead and select that it will copy over that material.
[96:01] I can close it.
[96:02] And now in my original project, we have the new folder with the master material and this master material is pretty simple.
[96:10] You can open it up and pick it apart to see exactly what changes I made.
[96:15] It is simple, but it's also super versatile.
[96:18] We can pretty much make 95% of the edits we would want to.
[96:22] So now to use this.
[96:24] All you have to do is right click, create a material instance and I'll call this M I for material instance underscore meet Matt.
[96:33] Now the workflow is to import textures from substance painter and within the master material and let me exit out of all that under textures.
[96:44] I can activate all them and then drag in those export textures like this.
[96:52] And drag the mask into the mask, a O roughness metallic.
[96:56] And I'll place this one on the far right, right there like this.
[97:01] This is exactly the same.
[97:03] We just didn't have to manually create the nodes and plug them up.
[97:06] The benefit of this is now if I undock my material instance, and let's make this bigger, we have all these adjustments I can make.
[97:16] So I want to go over each of these adjustments.
[97:19] These are pretty essential for most materials, especially if you want to make a change on the fly in engine.
[97:25] If you want to make a very small change, having to go into substance painter, make that change and re importing can be a huge hassle.
[97:32] You would rather just do that in engine.
[97:35] So obviously we have color tint.
[97:37] This will just allow us to make a slight color tint to give it a completely different feel.
[97:42] I can make it just a little bit greenish like that.
[97:45] Now it's yellow.
[97:46] And below that is the brightness.
[97:48] We can make the textures brighter or going below one darken the textures.
[97:53] And then I have contrast.
[97:55] I can make this really contrasty and also increasing the brightness to get a really interesting looking character compared to the original one.
[98:04] And color saturation will increase the saturation and also decreasing it below one will de saturate it.
[98:13] Zero will just completely remove those colors and make it black and white.
[98:18] So for roughness strength is just a slider.
[98:21] If I increase this, our character will be more rough and then decrease it.
[98:26] The character will be less rough.
[98:28] So we see those changes happening.
[98:30] Same thing with the roughness contrast increasing it will make the roughness pop a little bit more.
[98:37] And here's a tip just like how we can view channels and substance painter.
[98:41] We can also view channels in unreal to know exactly what we are editing.
[98:46] So I will undock this detailed panel to the side so I still have access to it.
[98:50] And up here under lit there is a buffer visualization.
[98:54] So if I just want to focus in on the roughness of my environment, then I select roughness right there.
[99:01] So here are the roughness maps we were working on in substance painter.
[99:05] And now I can see the edits I'm doing.
[99:08] So you can edit the roughness map like this.
[99:12] And also I have a min roughness and max roughness that you can optionally use.
[99:17] So maybe you don't like how rough some parts of the dirt are.
[99:21] You want to clamp that to a specific level.
[99:23] Then I could change this to 0.5.
[99:26] So now the entire model will never have a roughness value above 0.5.
[99:31] It is a lot shinier than the original texture and below that is a normal strength.
[99:37] So if explanatory this can increase the bump map of the material normals and height maps will be covered in the next section.
[99:46] Because built in to this material is a nanite displacement.
[99:50] If we activate the use height, but we did not export a height map with this material.
[99:55] So that is saved for the next section because I want to make this material as flexible as possible.
[100:00] If you don't like packing all your mass into one texture, we have this option to use mask.
[100:06] Uncheck it. And now you can still input the roughness and metallic maps separately.
[100:11] So I'll go ahead and turn that on and with use mass turned on since we already are exporting by default a ambient occlusion map.
[100:19] There is the option to activate the ambient occlusion to turn on ambient occlusion.
[100:26] Check this and click on the plus button.
[100:29] Now you might not have noticed a difference.
[100:31] But if we look at the shadows, this was before and this was after it is naturally darkening the crevices of my object just like how it was in the substance viewport.
[100:44] So this is before and actually let's go to lit and detail lighting to better see this.
[100:50] This is before and this is after this will only be noticeable in the shadow areas of the static mesh.
[100:58] So if I add in a cube and scale this up so my character is completely in shadow.
[101:08] Do better see the before and after especially noticeable in the bottom here.
[101:15] Do keep in mind that in order to see your ambient occlusion make changes in the project settings, you have to disable allow static lighting.
[101:22] Material ambient occlusion will not work if this is turned on.
[101:25] So go ahead and turn that off and then it will work.
[101:28] So that is optional.
[101:30] You don't need it for materials.
[101:31] In case you do want to use it, the option is there.
[101:34] And of course you can control the strength and the contrast down below so you can really exaggerate that ambient occlusion look.
[101:43] I'll go ahead and delete it because I no longer need the cube.
[101:48] We also have the option to change the specular.
[101:51] Now for this kind of material, I don't recommend changing the specular.
[101:55] This is also optional.
[101:56] You don't need to use this, but generally for natural assets like ground textures or rocks, you don't want to use unreal default specular value of 0.5.
[102:06] So for those kind of assets, if you enable specular right there, then this is before and this is after.
[102:16] This removes a lot of the reflective highlights we were getting on the mesh, especially from this angle before and after.
[102:23] Now in this case, I do want this turned off.
[102:26] But if you have a rock or maybe like a tree bark, then turn that on will make the material look a little bit better.
[102:32] And if you have an emissive map, we don't.
[102:34] But if you did paint lights into your material, then you could turn on the emissive right here and input the emissive texture.
[102:42] And finally, we're able to change the UV tiling with this one.
[102:46] Although for the most part, if you're exporting from substance painter, you don't need to use this since the textures were made for this specific UV map.
[102:54] As soon as we start changing the UV map, for example, like the scale, then everything breaks.
[103:00] So if you're exporting from substance painter, you don't have to use this.
[103:04] This is just an option in case you want to use this material for other things.
[103:08] So that is the basics of importing and how to use the substance master material.
[103:13] Now that we have created a simple material and painter and brought it into Unreal, let's create a brand new paint project to show how we could do that same process.


### Texture SciFi Crate [103:14]
**Transcript (timestamped):**
[103:22] But for a high quality asset made for games or animations, specifically this science fiction crate you see on screen.
[103:29] Now this model was originally created by Giovanni Nakpil over at Adobe.
[103:34] You can check out his art station to see some of his other work.
[103:37] It was made using substance modeler, which is created by the same people who made painter.
[103:42] Compared to other 3D programs, modeler is much more artist friendly.
[103:46] It feels more like sculpting a model out of clay than it does out of polygons.
[103:51] I recommend checking that program out if you're new to 3D modeling.
[103:54] The sci-fi crate model is just a little bit more complicated than the previous model, so we will induce a lot of new advanced features.
[104:02] Now let's jump into it.
[104:03] Let's start painting our sci-fi crate.
[104:05] And don't worry, this project will go by a lot faster than the previous one because we aren't explaining the basics.
[104:11] We're just going to go straight into it and start texturing using smart materials.
[104:16] So let's open up the sci-fi crate included in the downloadable content.
[104:20] I'll just go ahead and drag it into my project and let go.
[104:24] Now make sure the normal map is direct X and compute tangent space per fragment is turned on.
[104:30] Also, this is good to know, but if your model doesn't have a UV unwraps, then you can select the auto unwrap option.
[104:37] And Substance Painter will do its best to unwrap the model for you.
[104:41] In my case, my model does have UVs, so I'll leave that unchecked and click on OK.
[104:46] And here is our sci-fi crate.
[104:48] Now this crate is a lot more complicated than the previous model, mostly because if we go to the texture sets, we see we have a bunch of different texture sets.
[104:58] Compared to the last model with only one texture set, you can think of texture sets as being different materials on the same model.


### Texture Sets [105:02]
**Transcript (timestamped):**
[105:06] The main difference is that each of these texture sets will have their own unique layer stack.
[105:12] So when we export out this model, each texture set will have their own set of textures that will be exported independently of each other.
[105:20] Generally, texture sets are assigned in 3D modeling programs.
[105:24] I imported the original model from Substance Modeler into Blender.
[105:29] And within here, I assigned different materials.
[105:32] This is how we would create texture sets in Blender, and that is assigning different materials to different parts of the mesh.
[105:40] And then I exported this object into Substance Painter.
[105:44] You'll notice that all the materials and the names are the same as the texture sets in Painter.
[105:50] One benefit of using texture sets is now we can get a lot more detail throughout my model.
[105:56] If I want to view what texture sets are assigned to different parts of the model, then I can come up here and select the one icon.
[106:04] Now I can select all my texture sets and see where they are located.
[106:10] I can click on the one icon again to see everything.
[106:14] If I just want to hide and unhide a texture set, then come over to the texture set and click on the I icon to hide it and the I icon again to unhide it.
[106:24] The benefit of using texture sets right now is that this gives us a lot more data we can use.
[106:29] Since each of these texture sets will be exporting their own textures, that means for the front here, this area can have textures that are 4K.
[106:39] And then the body, which is right here, can have its own set of textures that are 4K.
[106:44] The top can have their own 4K textures and the rest of the texture sets.
[106:49] If this was just one material, then we are limited to it having one set of textures that are either 4K or 8K.
[106:56] This also gives us the flexibility and that is, let's say with this top device, you know, this is pretty small.
[107:04] It might not need 4K textures, so the rest of my mesh can be 4K.
[107:08] But if I select on the resolution, now I can lower this area of the mesh to 2K textures.
[107:15] So I can control the resolution for the different parts of the mesh.
[107:20] As an example, right now, I will just add in a fill layer for the body.
[107:24] That's how we can see it and make this a little bit red right now.
[107:30] Okay, so in order to see a texture sets layers, we have to have it selected.
[107:35] If I select the front metal, then we're seeing the layers of the front metal and we don't get that fill we just created.
[107:40] So I can select the texture set by clicking on it from the texture set list right here.
[107:45] Or I can hold down control and alt at the same time and then right click on an area of my model.
[107:51] If I want to select the device, then I'll right click it there and we can see that I have it selected to select the body, control, alt and right click.
[107:59] Do now select the body and get back my layers.
[108:02] That is a very important shortcut that I use all the time when my model has texture sets on the subject of resolution because there is so much data on this model.
[108:12] You might notice that the viewport starts to lag.
[108:14] If your viewport is lagging, then I recommend to come over to your texture sets and start lowering the resolution.
[108:21] Don't worry, you won't lose any data.
[108:23] When you go to export out your textures, you can always increase it without any loss of information.
[108:29] Now, whenever I'm just starting out in a new substance painter project, the first thing I do is go ahead and check my materials and see if there's any good materials here or smart materials I can use as a base to kickstart the texturing process.
[108:44] And I already know if I go here under my smart materials, scroll down.
[108:48] I want to use this steel painted stained smart material because I want to give this a military look.
[108:55] Almost like this could be an asset from Halo that the Marines use.
[108:59] So you could almost imagine that this crate is made out of steel and then it's painted a military green color.
[109:06] But of course, before we use any smart materials, we first have to bake our mesh maps.
[109:11] So come up here to the croissant and select that and leave everything at default.
[109:17] Now this might take a while to bake because instead of baking a set of mesh maps once, we have to bake the set of mesh maps for all the materials.
[109:25] All of my texture sets.
[109:26] So I'll just select bake, select the textures and we can watch it working in real time here.
[109:32] So I'll go ahead and speed up the video.
[109:37] OK, great.
[109:38] Now that it's done baking, return to painting mode.
[109:40] And now we can see all the mesh maps for my different texture sets by selecting a specific texture sets and in texture set settings, scroll down and here they are.
[109:50] So these are the maps for the body.
[109:52] I go to front metal and they'll have a different set of texture maps.
[109:56] Now let's assign our first smart material and specifically it is steel painted stained.
[110:01] So I'll drag this onto any of my texture sets.
[110:04] Specifically, we'll start with the body first and let go.
[110:07] Great.
[110:08] Now already this looks really cool.
[110:10] There's already a bunch of detail built into its layers.
[110:14] So to start, just real briefly to cover it.
[110:17] We have the base paint and then also a roughness map to simulate scratches and wear over time.
[110:23] Then there's a little bit of a dirt on top of that.
[110:26] Some more dirt that's using the ambient occlusion map.
[110:28] This one is very subtle.
[110:30] You can kind of notice it right here in this corner before and after and then more surface details specifically to edit the normal map and give it just a little bit of a bump and shadows.
[110:42] And finally, for the last layer, we have the edges, which is chipping away at the coated paint, revealing the steel base of the container.
[110:51] And while this does look good, it's not really using the curvature much.
[110:56] I want to increase the curvature look for this because while it is chipping away at the crates with these little flakes, we're not seeing any difference at the sharp edges or the corners of the base.
[111:10] So let's go ahead and edit this mask.
[111:13] I'll select the mask and it looks like we have a fill layer.
[111:16] Okay, that's not doing that much.
[111:18] But below that we have the metal edge wear generator.
[111:22] So maybe one of these settings will help us increase the curvature.
[111:26] And if I scroll all the way down, you see we do have a curvature option at the bottom.
[111:30] So it's at the zero point four.
[111:32] That is not that much.
[111:33] Instead, what I'll do is increase this to something like zero point nine two.
[111:39] Okay, so now this is looking a lot better.
[111:42] And in my opinion, just a lot more realistic.
[111:45] Because if I just view the mask now, notice how the steel is following the curvature of my geometry.
[111:52] But I do think that there's just a little bit too much grunge right now.
[111:56] So if I come up to grunge and grunge amount, maybe okay, I can lower this significantly.
[112:03] So maybe to zero point five.
[112:05] Again, none of these changes are final.
[112:08] I can always go back in and edit them.
[112:10] If I did it like a change, I did now time to change the color of this material.
[112:15] And we will do that with the very first layer base paint.
[112:18] Also, these layers that are below the group, I no longer need.
[112:22] So I'll go ahead and delete them.
[112:24] So going back to my face paints, select this.
[112:27] I don't want a blue.
[112:28] I want a military green.
[112:30] So we'll go down to the greenish range and try to select something.
[112:34] Okay, I think this looks good.
[112:36] So I will exit out of it.
[112:38] Now my material is starting to look like something the military would produce.
[112:42] And don't forget to save your project.
[112:44] That's how we don't lose anything.
[112:46] So I'll go ahead and save this in my substance painter project folder.
[112:49] Call this one sci fi crates.
[112:52] One thing I'd like to do is increase the brightness of my viewport because I noticed by default substance painter is just a little bit too dark.
[113:00] So this is optional, but I think it gives a better representation of what the color will look like in Unreal Engine with a high exposure.
[113:08] And that is to come over to the viewport settings up here.
[113:11] And for environment exposure, I'll increase this to one.
[113:16] Now, as you can see that the rest of this mesh, and that's because by default it is using really white values.
[113:23] And you would expect them to be pretty much blown out, unless they're in shadow.
[113:28] So temporarily what I'll do is go to one of the other texture sets, a temporary fill layer with a base color that is somewhere in the grayish area and also increases roughness.
[113:44] Now I will control see this and paste it in the rest of my texture sets.
[113:49] That's how when I'm working, at least for now on the body, the rest of my mesh isn't so blown out.
[113:56] Okay, so there we go. I think I'm getting a better view of what my model will look in engine.
[114:02] Now something else I want to do is blend this smart material with another smart material, which is this material compared to the original one has a lot more bumps and is a little bit dirtier.
[114:13] This will help give more of an agent effect to my sci fi crates.
[114:17] So I hold down the mouse button and drag it onto my crate like that.
[114:21] Now obviously this is the wrong color. So before I even mask it out, I'm going to come into here, grab the base paint, and I will copy its hue value right there.
[114:32] So go ahead and control C. And then going into my still painted worn, you'll see that there is a folder within the folder called paint.
[114:43] And it is right here, shiny paint. I'll select that and then paste in the original green value I found.
[114:51] I only want to place this according to my ambient occlusion. So I think I'll use a dirt generator, scroll up to the very first folder and selecting this, we will add in a black mask and then a generator for dirt like that right there.
[115:09] I like the effect that this is giving, especially in areas with a lot of high detail like over here, I do want this to be pretty subtle.
[115:17] So I could chip away from the dirt within the generator right here.
[115:21] Or what I can do is select the folder as a whole and just lower the folders opacity.
[115:27] So I'll come over here to normal and decrease it to something like 20.
[115:33] And you will notice that even if I do have an opacity that is super low, we still get a lot of the height data that is coming from this folder.
[115:41] Because as you remember, height opacity and blend mode is controlled separately in a different channel, specifically, of course, the height channel.
[115:50] So going to the height channel will allow me to, let's say, decrease this.
[115:55] So with height, I still want a bunch of the bump that we're getting from the still painted worn.
[115:59] So I'll leave that at around 43.
[116:02] And then for the base color, I'll leave this at like 25.
[116:07] Okay, so now this is giving a really cool effect, especially if I get the angle right with the lights.
[116:13] This is before and this is after.
[116:17] So it is giving a much more worn out realistic look to the entire crates.
[116:22] Now let's take this same material and apply to the top.
[116:25] So to do that, I will close all my folders, select both of my smart materials, press control and see, and then hold down control and alt, right click on the top to select the texture set, or I could have selected it from the window and press control and V to paste that in.
[116:42] Now I will select these two layers and delete them.
[116:46] Okay, so this is already looking really good right off the bat.
[116:50] But I do think I want to increase the curvature right here to make it more apparent.
[116:55] So within the still painted stains under edges, let's go to the mask, metal edgeware and increase curvature weights all the way up to one.
[117:06] And also for the contrast, maybe if I okay if I breathe this down, we're getting back a lot more steel and also playing with the levels here too.
[117:17] Okay, there we go. I think I like those values.
[117:20] Now let's work on the metal.
[117:22] I want to use this smart material.
[117:24] So steel gun painted as a base and just drag it on and let go.
[117:30] Okay, and it will automatically select my front metal texture set for me.
[117:34] So I can start editing it and it's already looks great, but it is just a little bit too dark.
[117:40] So I will lighten it up.
[117:42] And actually, let me go ahead and select these two layers.
[117:44] We don't need them in the folder.
[117:46] Select the base metal.
[117:48] It is mostly the first layer that controls color and right here.
[117:52] Okay, this is pretty dark.
[117:53] I will increase their color just to make them a little bit brighter.
[117:57] And also there's a second color here that is blending between the two.
[118:01] So for this one also increase it to make it bright like right there, just like what we did with the base where we blend it between two smart materials.
[118:09] I will do the same for the metal to add a lot more variation because right now this is looking pretty stagnant.
[118:15] Scrolling up specifically, I found iron forge old to be really good.
[118:20] So I'll drag it onto my steel let go and it's giving a really cool look to it.
[118:26] Now, of course, we need to blend it.
[118:28] So I'll add in a black mask and a generator.
[118:32] This one will be our curvature.
[118:34] So metal edge where and this iron forge old.
[118:38] Is only showing up on the sides now.
[118:40] I do want it to be more apparent that there is a lighter metal on the edges with metal edge where increase the levels or actually also increase the contrast.
[118:52] I think this looks good.
[118:53] And also in the past, I found that mixing the metal edge where with the dirt generator can create a really detailed look.
[119:01] So that's what I will do right now.
[119:03] I will use two generators, one primarily using the curvature and one primarily using the ambient occlusion.
[119:09] So going to the wand add generator will use the favorite one and that is dirt.
[119:15] So selecting dirt, I will blend the two by changing its blend mode to linear dodge add.
[119:23] Okay, cool.
[119:24] So this is what I'm getting.
[119:26] And I think I want to increase the contrast also for dirt.
[119:31] So increase it there like this.
[119:35] And also the levels.
[119:37] Okay, so we're getting a very contrasty look.
[119:40] This is what it looks like right now before and after.
[119:46] I think it added a lot of necessary detail for the metal.
[119:51] So slowly over time, our crate is starting to come together.
[119:55] Now I want this same exact metal.
[119:58] These two layers on my side and on my top, select both of them, control C, control Alt, right click, and I'll paste them into here.
[120:09] Select those layers, delete them, right click, and I'll paste them into here too.
[120:15] Okay, nice.
[120:17] Honestly, this has gone by very quickly, but we already have a near ready asset by just using the resources that substance painter comes with.
[120:26] We can create really realistic textures right off the bat.
[120:31] I think maybe for the metal on the side, the curvature is a bit too strong.
[120:36] So I'll select it, see what it is.
[120:39] And okay, this mask is taking up the majority of the space.
[120:42] So we probably want to decrease that.
[120:45] So we still get some of the original material.
[120:48] And finally, the last part we need to paint is of course the device up here.
[120:52] You can imagine that someone needs to input a password into this device in order to open up the crates.
[120:58] So the device will be pretty simple.
[121:00] What I'll do is hold down control and alt and then right click to go into the body texture sets.
[121:06] And I'll just copy the steel painted stain control right click on the device to go into that and paste that in.
[121:13] I don't need these two layers.
[121:15] I'll delete them.
[121:16] And now I do think the curvature is a little bit too strong.
[121:19] It is overwhelming, especially since this device has a lot of sharp angles compared to the rest of the mesh.
[121:25] So we will lower the curvature here by going into there and decreasing it.
[121:31] Okay, that looks better.
[121:33] I want a bunch of different colors on this device.
[121:36] So for the outer color, I'll select this and bring this up so I can better see it.
[121:41] I will desatrade and also lighten it up to somewhere like right there.
[121:48] And now I will duplicate this control and D and give it a different color for the steel inside of the device.
[121:56] This one will be a lot less green like right here and add a black mask.
[122:03] Now I could add in a paint effect and the paint there.
[122:07] But in my case, I know that I'm just masking out the geometry.
[122:10] I'm not going to add any fancy generators or effects.
[122:13] So in my case, I'll just paint directly on the mask.
[122:16] So go into polygon fill mode and select the inside to add in that color.
[122:23] Okay, that looks better.
[122:25] And I will add in an even lighter color or lighter gray to the middle part here.
[122:30] So press control and D. Let's edit this color, make it lighter.
[122:35] And I don't want the same mask as below because it is replacing the bottom layer.
[122:40] So right click on the mask and then we will clear it and go back into the polygon fill tool.
[122:45] And select the middle.
[122:47] I want to paint the hinges right here blue.
[122:50] So duplicate this.
[122:53] Make this a bluish color.
[122:55] And once again, clear the mask and use the fill tool to select the hinges.
[123:01] Now for a second material for my device, I want a plastic smart material.
[123:07] So I'm going to find materials and type in plastic.
[123:11] Let's use this one, plastic glossy stain.
[123:14] Just drag it and let go now at the top of my layer stack.
[123:18] I have my new smart material will add in a black mask.
[123:23] And I just want the triggers and this cylinder to be plastic.
[123:28] So I'll select them like this, of course, with a polygon fill tool,
[123:32] because all these meshes are separate from each other.
[123:35] It makes painting a lot easier in substance painter.
[123:38] And let's add one more additional color to this plastic.
[123:42] So duplicate the base, make this red.
[123:45] And then I will add in a mask.
[123:47] But instead of adding a black mask, I'll just add in a white mask because I want the majority of this material right now to be red.
[123:55] So I can leave all the triggers the same.
[123:57] I just want to mask out this red layer from the cylinder.
[124:01] So we get back our original orange layer.
[124:04] So I need to make sure my color is zero to mask it out and select it right there like this.
[124:10] Here is what we have for my device and it looks pretty good.
[124:14] One last thing I want to do is because this is a screen, this should be pretty glossy.
[124:19] It is not glossy right now.
[124:21] It's hard to tell that this is a screen that would display some information.
[124:25] So I'll just add it real quickly in a fill layer for the base color.
[124:29] Make this pretty dark because the darker the color is, then the more reflection we will get in engine roughness.
[124:37] Bring this all the way down so it is not rough.
[124:40] It is pretty shiny black mask and select the middle.
[124:45] Now you will see that the bump map below this layer is being carried over.
[124:51] So it makes the screen really bumpy.
[124:53] That's not how screens should look.
[124:55] So in order to change this and get rid of that bump, I need to go into the high channel and remember that all my channels have their own blend modes and opacity.
[125:05] By default, the layers in the high channel will be set to linear dodge.
[125:08] That means all of these layers, if we look right here, are being added on top of each other contributing to the final look.
[125:15] Instead of using the linear dodge, I will change this to normal.
[125:19] We'll show them just replace the height and we don't get any of that bump.
[125:23] Now in just a moment, we will cover height and normal maps in depth and how to get displacement and unreal.
[125:30] But I do want just a little bit of bump here.
[125:32] So what I'll do with the opacity in the high channel is just lower it a little bit so we can see we're getting that back.
[125:39] So maybe lower it to something like 80.
[125:41] Okay, that looks good.
[125:43] And now finally one last change before we see what our mesh looks like an engine and that is to add in a red highlight on my key.
[125:51] That kind of matches the red highlight on the device.
[125:54] So over here, I'll hold down control and alt right click it to go to the top metal texture sets.
[125:59] And let's go back to base color for my channel view, add in a fill layer.
[126:05] I will move this outside of my smart material.
[126:09] And then base color.
[126:10] Let's make this a reddish like right there.
[126:15] Add in a black mask and select the middle.
[126:19] Okay, that looks good.
[126:21] I think I will increase the metallic to make this a metal like color.
[126:28] And also decrease the red because that is pretty strong.
[126:32] Now we are ready to export this and bring it into unreal.
[126:37] We are back in the unreal project with the angry orange people.


### Import SciFi Crate [126:38]
**Transcript (timestamped):**
[126:41] So we will import the same sci fi crate mesh that we've been painting on.
[126:45] I'll do that within the meshes folder and drag that in.
[126:50] It will use the same settings that we set up before.
[126:53] All we did was that we turned off importing materials and importing textures because we will create those from scratch select imports.
[127:01] And here is our sci fi crate.
[127:04] And it is ready for us to start importing the textures.
[127:09] Now back in substance painter press control shift and E to bring up the export settings.
[127:14] And this will look different from the previous mesh we exported because instead of one texture set we have several texture sets.
[127:20] So each of these texture sets will export their own group of textures.
[127:25] So that means in unreal each of these will represent their own unreal material.
[127:30] Now I could export these textures as is using the default settings or what I'll do is go to global settings and then just use the preset of real life before that it comes with.
[127:40] So scrolling down here let's go to Unreal 4 packed and select that now selecting any of my texture sets.
[127:46] We will see the color and normal and also that mass material that contains the metallic roughness and ambient occlusion.
[127:53] Now I do not need to export and amiss of texture.
[127:56] So I'll go ahead and uncheck the last texture for all my texture sets.
[128:02] Another thing to keep in mind is that this asset will be very expensive in unreal because we have six different sets of 4k maps.
[128:11] That is a lot.
[128:12] So if you're going to use this in a game that you might want to considering lowering exporting 4096 not because unreal can't handle resolutions out of this size.
[128:22] But because if you are going to distribute your game that is going to be a lot of data that the player has to download and store.
[128:29] Normally for game assets we would just use one set of texture sets.
[128:33] Unless this is a hero asset where the camera will be up close to it for some reason kind of like a weapon or armor on the main character.
[128:41] In my case I want to show off the best quality possible.
[128:44] So I'll leave all the texture sets at 4k one last thing.
[128:48] Let me export to a folder on my desktop right here and let's export a case for some reason you don't know where your textures were exported.
[128:58] You could always come up here to the open output directory to see the exported textures back in unreal.
[129:04] Let's import our textures.
[129:05] So I'll go to textures and just create a new folder.
[129:09] Call this one create textures and within here I'll go ahead and select all of them and drag it in a let go.
[129:18] Okay great.
[129:19] Don't forget to control S and save all them.
[129:22] We will already see that unreal was smart enough to give all the normal textures normal map settings.
[129:27] But if we open up any of the mass then we will see that sRGB is not turned off.
[129:33] So I have to go through all of these masks and turn off their sRGB one by one which can be a hassle especially if we're importing a lot of textures or a shortcut is a hold down control and to select all my mass that I want to turn off sRGB in and then right click on them come up to asset actions and down here select edit selection in property matrix.
[129:56] So this will bring up all of its properties.
[129:59] And now what I can do is in the search type in sRGB and uncheck it right there.
[130:07] Now that will uncheck sRGB for the rest of my textures and we can even see it that it was unchecked for us that way.
[130:15] That is a neat little shortcut that will save a lot of time.
[130:18] So we do not have to open up and edit each mass texture individually.
[130:22] Now time to create materials and add those textures to it.
[130:25] And instead of creating the material from scratch what I'll do is leverage that master material in the downloads.
[130:32] So I'll right click create a material instance called this MI underscore creates underscore body open this up and then drag those textures that correspond to the body material.
[130:46] So here normal and roughness like that.
[130:51] And then I'm able to go back and drag it on like this.
[130:56] So I'll do that same process for the rest of the texture sets.
[131:00] I've gone ahead and created all the texture set materials from the master material.
[131:04] Now I can start applying these materials to the mesh.
[131:07] So our front metal goes into the front like that.
[131:10] The side metal right there top at the top the device and the last metal.
[131:18] So here is our high quality sci fi asset that is ready to go inside of unreal.
[131:24] And this is absolutely incredible how amazing these textures are.
[131:28] And it didn't even take us that long to create something realistic like this.
[131:32] That is the power of the workflow with substance painter and unreal.
[131:35] They go perfectly together.
[131:37] And because we created these materials with a master material that means I can make any adjustments on that material.
[131:43] So go ahead and open up the base material and then to better see it.
[131:48] I will just undock the details panel of this material instance and move it off to the side.
[131:54] So if I want to play with the saturation maybe bring it down.
[131:57] I think it's too green and I could do that right there or play with the tent and any of these other settings.
[132:04] So it is very customizable.
[132:07] Also you will notice that now if I do drag out my crate from the content browser.
[132:12] For example right here and drag it out then the materials aren't placed on it.
[132:17] I need to add these materials in the static mesh editor.
[132:20] So to do that just double click on the static mesh and then assign the same materials to it.
[132:30] Now if I drag out the mesh we can see that it already has those materials ready to go.
[132:36] But nothing is perfect.
[132:37] The creative process is very iterative after exporting and importing your textures.
[132:42] You might realize that you made a mistake or you want to change something after seeing what your model looks like in Unreal.
[132:48] And that is OK.
[132:49] Now I will show how we can make an edit in substance painter and then move that edit over to Unreal.
[132:54] Let's add a little bit more character to my crate specifically.


### Decals [132:55]
**Transcript (timestamped):**
[132:58] Let's add some text to the front right here and we will do so with decals.
[133:03] So decals operate very similar to how they do in Unreal.
[133:07] You could basically just think of it as one little stamp you can place on your mesh and it can be helpful to use decals instead of painting because we get a lot more precision.
[133:16] Best to show what I mean with that example.
[133:18] So let's first create a fill layer and this will be the text layer.
[133:22] I only want to affect the color.
[133:24] So hold down alt.
[133:25] I'll select color right there and then add in a black mask and a fill layer.
[133:31] So go to effects at fill and the texture we will use for this layers mask will be under here.
[133:39] Type in aerial bold so we can generate textures through fonts and by selecting aerial bold.
[133:46] I can now and OK.
[133:48] You can see that currently the projection looks pretty crazy.
[133:51] If I increase the tiling we can better see what it is because it is just right now using the UVs of my mesh for the texture projection.
[134:00] Now previously we've been using triplanar projection but to get even more control instead of triplanar projection which adds it to my entire mesh.
[134:09] We will change this to planar projection and now I will decrease the tiling because that was just an example to something large like this.
[134:19] Notice how this texture is repeating.
[134:21] I do not want this.
[134:22] I just want one texture in the properties for UV wrap instead of repeat select none.
[134:28] So now there will only be one image of this texture.
[134:32] It will not be repeating when using planar projection and with our texture selected we're able to edit where the texture is using this gizmo right here.
[134:42] So right now we are in translation mode.
[134:44] That is pretty self explanatory.
[134:47] It's just like how it is in unreal.
[134:49] I can move this around or I can go into rotation mode or even scale mode right here.
[134:56] And the shortcuts for this are w to move e to rotate and r to scale.
[135:04] This should be very familiar with you.
[135:06] If you use unreal these are the same exact shortcuts.
[135:09] I only want this texture here at the front when using planar projection.
[135:13] Oftentimes you might see an issue where it is projecting onto the back as well as the front which in my case does not make sense.
[135:21] So in order to get rid of the back projection in back face calling turn this on which will remove it.
[135:28] If you still see it there you might want to play with the angle and the hardness.
[135:32] Okay so now we can go to the front and I can try to position this where I want it to be another alternative to move this around which can be easier is to use the surface tool which will give me this little box.
[135:44] And if I hold down on this then it will snap according to the surface of the mesh which can also make decal placing easier.
[135:51] So I'll put my text right here.
[135:53] Of course we don't want it to say lorem ipsum.
[135:56] I can change the text to anything so feel free to type anything you want.
[136:00] In my case I'll type something on theme top secrets and call this great zero zero one dash three one two one or just any random numbers.
[136:10] Okay great.
[136:11] So now I can place that here and rotate it scale down a little bit.
[136:19] Okay I like where it is but this is way too bright.
[136:23] We need to blend the text in just a little bit more with the layers of pasty I will bring this down to something like 43 and I can even go in with a brush effect to go to effects at paint.
[136:38] Then we will go to our paintbrush select dirt to and chop away the text with a black brush to really help fade this in with the rest of the mesh and decrease that intensity.
[136:51] Okay that looks good.
[136:53] One last change this is way too stretched so I'll just squish it in the x axis to bring the changes into unreal I have to re export them out so control shift e to bring back the export settings.


### Reimport Textures [137:00]
**Transcript (timestamped):**
[137:06] I can't because I only made a change to the body.
[137:09] I don't have to export out the rest of the texture sets.
[137:12] I will disable them.
[137:13] So we're only exporting the body and I want to make sure that I do export them in the same location as my original textures.
[137:20] So these new textures will override the old ones and then press export.
[137:26] Now seeing where those textures are stored in the base color.
[137:30] I can see that we have the new texture because down here is our text.
[137:35] So in unreal let's go to where those textures are in my folder.
[137:38] So textures create texture and it is these three textures which I'm replacing.
[137:43] So what I'll do is go ahead and select these three drag them in and let go.
[137:49] So now those textures will be overridden and they still keep the same settings that we changed beforehand.
[137:55] And now my crate is using the updated textures.
[137:58] Another thing I could do instead of manually dragging back in the textures because I export them out in the same location as the original textures.
[138:07] I could have selected these textures right clicked on them and then select re import.
[138:13] That would be another way to update the textures in this section.


### Height Maps [138:17]
**Transcript (timestamped):**
[138:17] We will cover how to use substance painter to create Nanite displacement.
[138:21] This allows us to control the actual geometry of our mesh through its materials and textures.
[138:27] This allows whole new creative possibilities with substance painter and unreal.
[138:32] So far throughout this tutorial all the materials we created automatically have normal maps.
[138:37] These textures allow us to show depth by adding shadows directly to the material.
[138:41] But these shadows are fake and are not actually changing the geometry of my objects.
[138:46] Substance painter also has the ability to create height maps.
[138:50] Which unlike normal maps will physically deform my geometry with the white values representing higher geometry and black values being lower.
[138:58] We will go over both maps in just a bit.
[139:01] Before we move on I also want to mention a very common workflow you will see in substance painter and that is baking normal maps from high poly meshes to low poly meshes.
[139:12] Now depending on the way an object is created it can have hundreds of thousands of polygons.
[139:17] This many polygons is mostly unnecessary.
[139:20] And while Unreal Engine 5 is able to handle this many polygons because of Nanite,
[139:25] high poly meshes are still harder to manage and take up a lot of memory.
[139:30] What 3D artists do is that they decrease the amount of polys through a process called retopology or through automatic reduction algorithms.
[139:38] This makes an easier mesh for us to handle but by lowering the polygons we erase a lot of the geometric detail we may want.
[139:46] This is where high poly mesh baking comes in handy.
[139:49] When we go to bake we have this option to add a high poly mesh.
[139:52] Here we can add the original high poly object.
[139:55] Now when we go to bake substance painter will create a normal map from the high poly mesh with all the high detail baked into it.
[140:04] This normal map will automatically be applied to the mesh and be a part of the normal map when we export.
[140:10] So we get all the details of the high poly mesh without actually being a high polygon object.
[140:16] The details are being faked by the normal map.
[140:19] This is a very common workflow that you will see on a lot of 3D assets for games.
[140:24] Now in our case we don't have to bake from a high poly mesh since the 3D objects we have used already have enough detail
[140:32] and we are adding in normal map variation directly in painter.
[140:36] Now that we covered normal map baking let's go over how we can paint in high detail in substance painter.
[140:42] I am back in our original project.
[140:44] The reason why is because it will be easier to show how substance painter handles displacement with a simple mesh.
[140:50] We will return to the sci-fi crate in just a bit.
[140:53] So something that can confuse new users to substance painter is that there are two channels that control depth.
[141:01] That is the normal map and the height map.
[141:05] So if I select the height right now we don't have any height so it's just a pure black texture.
[141:09] If we had any white spots then that would mean we will edit the high channel in just a bit and then the normal map.
[141:17] If you are using any of the materials or assets that have normals built into them you would see them here.
[141:23] Right now there isn't that much normal detail on my character because the only material that has normals is steel.
[141:30] So if I go back to my coated metal scroll down here and we have galvanized steel that is being masked out.
[141:36] If I hold down shift to disable the mask and click on this we can see the normals of my galvanized steel.
[141:43] Because this is what my character looks like right now without masking out it.
[141:47] And if I move my light around that the lighting and shadow is changing on my character because of the normals that are on it.
[141:55] So I'll go ahead and hold down shift and click on my mask again to mask out the steel so it's not everywhere.
[142:02] When we go to export our textures pressing ctrl E you'll notice that under materials you will see that with the Unreal Engine templates that we're not exporting any height texture.
[142:13] We're only exporting a normal map and this normal map is the combination of the heights and the normals.
[142:20] So if we look at the channels below normal and height we have normal plus height plus mesh channel.
[142:27] This will be the exported normals so it will combine the height channel with the normal channel to create a new normal map that would be exported.
[142:35] And I know that was a handful of words.
[142:38] It is best to show what I mean with an example.
[142:40] So we will create two layers one layer is going to edit the height and the other layer is going to edit the normal map.
[142:46] So to begin let's create a new fill layer which will just change the height.
[142:51] So I'll come up here to fill and hold down alt and select the height channel.
[142:56] So we're only changing the height.
[142:58] If I change the values right now we're not noticing any difference and that's because the height is uniformly changing.
[143:05] We need to add a mask to this layer.
[143:07] So I'll go ahead and add in a black mask and then a fill layer or a texture.
[143:12] Let's go into the Alphas and see if I have any nice shapes and I like this heart.
[143:17] So I'll go ahead and drag it and use this as my mask.
[143:20] Now it is way too big.
[143:22] So up here I will increase tiling and I only want one heart not a bunch of different hearts and I want it in the location of his chest.
[143:30] So we will turn this into a decal by selecting planar projection and way too many hearts.
[143:37] So for UV wrap change this to none.
[143:40] Now I can move my heart around and let's place it right here.
[143:45] Also increase the size just a bit like that.
[143:49] When I move my light around we can see that the hearts shadows are changing.
[143:54] Zooming in right now I could change the depth of this heart by selecting the layer again and playing with the height value.
[144:02] So right now the heart is digging into the model and then if we go into the positive range the heart will be popping out of the model.
[144:09] We can visually see this change by selecting the height channel.
[144:13] So if I move this up into the positive value we can see the heart popping out of my character.
[144:18] Now if I do go into the negative range we don't see it right now but it is there.
[144:22] We just can't see it because this is now a negative value cutting into the character.
[144:26] If we zoom into this heart you'll notice that it isn't changing the geometry of my model.
[144:32] There is no displacement just yet.
[144:34] I will show how we can visualize displacement in substance painter.
[144:38] But for now the reason why we can see it is because the height data is being added to the normal map.
[144:43] If we look at our normal map channel it is not there but looking at the normal plus height channel there is our heart which will be exported.
[144:53] Now let's create a layer that will only affect the normal channel.
[144:56] So I'll go ahead and create another fill layer and with this layer I will just select the normal channel holding down alt and selecting that to unselect everything else.
[145:06] Now this is asking for a normal map unlike with height textures which are a lot more simpler because they're just black and white.
[145:13] I don't recommend manually changing the normal map color here instead you have to use normal map textures.
[145:19] And substance painter already ships with a bunch of normal textures by selecting the texture category.
[145:24] So I'm going to scroll down and just find one I like for example this texture right here and drag it into normals and let go.
[145:32] Now again this is way too big so we will increase the tiling and also change this to planar projection make it so that it is not repeating.
[145:42] And now I will move this around and we'll move it.
[145:46] That's how it's next to the heart and also scale down just a little bit.
[145:53] OK just like that.
[145:55] Now we can see this change reflected in the normal channel by selecting normal and going to the normal plus height channel.
[146:03] You'll see that this information from the normal map is carrying over and so is the high channel.
[146:09] So both of these two channels are being combined right here which is what we see in the viewport.
[146:14] If you want to control the strength of your normal then go ahead and select that layer and in the normal dropdown select this.
[146:22] Now we can control its opacity here.
[146:25] I'll just leave it at 100 and go back to base color.
[146:29] Now you might be wondering to yourself OK so what's even the point of separating out these two channels.
[146:34] Well the reason why they did it is that's how everything that is in the height channel can be geometrically displaced.
[146:40] So if we make a change to the height channel then the actual geometry of the model will change.
[146:47] And all the detail that we add to the normal channel like all our normal maps will not change the geometry.
[146:53] So if you want to edit the geometry do it on the height channel.
[146:56] If you don't then do it on the normal channel.
[146:59] Right now the viewport isn't showing us any displacement.
[147:02] If we want to see the displacement that the height channel creates then come up here to the shader settings which is the ball icon.
[147:09] And all the way down here at the very bottom we have displacement and tessellation.
[147:13] Make sure it is enabled and now we can increase the scale to see it.
[147:17] And we can already see it's making some changes but this is really messed up.
[147:21] That's because we need to add in extra geometry for this height displacement to work.
[147:26] And to add in that geometry we just increase the subdivision count to something pretty high.
[147:32] Now we can see that the scale is too much so I'll just decrease it to something like right here.
[147:38] So now if I zoom in on my heart we see that it is literally cutting into my geometry.
[147:43] This isn't being faked by the normal map the geometry is actually changing.
[147:48] And going into the height layer I can now edit it right here with a negative value is cutting into the mesh.
[147:55] And then with a positive value is going outside of the mesh.
[147:59] Right now this height value is way too strong going into the height channel.
[148:04] We'll see that there is no natural fall off.
[148:06] It just goes from black immediately to white normally high textures you will see a transition from black to white.
[148:12] So there'll be some gray area in there.
[148:15] So something that is a very common workflow when working with height mask is to go into your mask and then add an effect filter above your main mask.
[148:26] That will just blur everything so type it blur select that and there we go.
[148:31] So now we're getting a much more natural transition from the black to the white and I can control its intensity right here.
[148:39] So this is creating a really funky looking effect.
[148:42] So just something just a little bit of a bevel on my heart and now control the height.
[148:49] Now let's export this high texture and do keep in mind that the viewport setting scale for displacement.


### Nanite Displacement [148:50]
**Transcript (timestamped):**
[148:55] This is purely visual for my viewport.
[148:58] If I change this this will not change the exported textures.
[149:01] There is a similar parameter in Unreal which we will cover.
[149:05] Also I don't need a normal map so I'll go ahead and hide that.
[149:08] That was just an example and to make it more apparent where the heart is on my character.
[149:13] I will enable color and then for this color let's make this reddish or pinkish and under base color the channels.
[149:22] I'll decrease the opacity.
[149:24] There we go.
[149:25] So there's just a little bit of color right there.
[149:28] Now I'll press control shift and E to bring up the export window and using the default template under material we can see that height is already being exported out.
[149:38] But if we are exporting using the Unreal Engine for template if we want to pack all our masks together.
[149:45] So let's select Unreal Engine for go back to material.
[149:48] There is no high texture being exported.
[149:51] So we need to add that to my Unreal Engine for templates and we can do that within the output templates.
[149:57] So down here if I select Unreal Engine for I can edit this and what I will do is select this button up here to duplicate it so I don't accidentally make a mistake.
[150:06] I will double click on this new template and I'll call this Unreal Engine five to keep up to date and add and height like that.
[150:16] So now with this template selected we are editing.
[150:18] I'm going to come up here and we will export an additional grayscale texture by clicking grayscale and to add in the height channel come over here to input maps height and simply drag it on top of it and let go.
[150:31] I will select great channel and now I want a similar naming convention to the rest of my textures because right now this export texture will just be called grayscale.
[150:40] So what I'll do is copy the name from any of them pasted here and just replace the word.
[150:47] In my case it is a missive with height so we know what it is now going into my settings in global settings instead of Unreal Engine four we'll use our own custom template on religion five and height and that's how we're able to get back the height map right here.
[151:03] So I will uncheck emissive because I don't need that and select export.
[151:08] Now we get the height texture we can see right here it is completely gray except the heart that's popping out of the character back in Unreal.
[151:17] Let's import them and don't forget for your mask to turn off sRGB and in addition to turn it off for the mask you also need to turn it off for the height texture.
[151:29] So make sure it's off there.
[151:32] Now I will use the same master material we've been using create a material instance.
[151:37] I'll call this M I underscore meet math height and plug up those textures.
[151:47] Before we add in the height texture.
[151:49] Let's first add this to my mesh so we can see exactly what's happening in the world.
[151:54] I'll go ahead and exit out of those textures.
[151:56] We don't need them.
[151:57] And then I will undock it and place this material instance here.
[152:02] I will also add that new material.
[152:05] So let's go here and add the height to this guy at the front and we can already see that we have a heart here and it looks like the heart already has death to it.
[152:16] If I move my light around the shadow on the heart is changing and that's not because of the actual geometry displacing as we can see it is completely flat.
[152:26] That is because of the normal map because remember height is added to the exported normal.
[152:32] And to be honest this already looks really good.
[152:35] It goes to show that we can get a lot of detail out of just using normal maps.
[152:39] We don't always have to necessarily displace the actual geometry of our meshes to give death to them.
[152:46] But in case you do want to add displacement.
[152:49] This is how you would do it.
[152:50] First off we need to check on the use height option right there.
[152:54] And this will give us a brand new texture that we're going to place our high texture on.
[153:00] Drag the high texture and let go.
[153:02] Now right off the bat you won't notice any changes.
[153:06] That's because we need to do two things.
[153:08] Number one this mesh needs to be nanite by default now in Unreal Engine when we import meshes they will automatically be nanite.
[153:16] But we could double check that it is nanite by double clicking on my mesh to open up the static mesh editor.
[153:22] And over here we can see enable nanite support is turned on.
[153:26] So this is nanite and then within the details panel of my material instance scrolling down we will see that we have material property overrides in this dropdown.
[153:37] Make sure enable tessellation is turned on.
[153:40] Now if I zoom in here we can see that our heart is sticking out of the mesh.
[153:46] This is really cool.
[153:48] We're able to sculpt or create detail within substance painter and bring that into Unreal as actual geometry now using high textures.
[153:56] The major benefit of enabling tessellation is that we have real geometry.
[154:01] So this will cast correct shadows.
[154:04] If I rotate my character like this.
[154:07] Notice how the heart is giving off a shadow.
[154:10] If I turn off tessellation right there then the only shadow is from the normal map is not casting across the character.
[154:18] Now we do have the correct shadows.
[154:21] Do keep in mind that there is a little bit of a hit to performance overhead because going to lit down to nanite visualization and triangles.
[154:31] These are now the triangles we are getting on our mesh with displacements.
[154:35] So unreal is automatically adding the necessary tessellation to make this high texture look good.
[154:42] If we compare it with the amount of polys on the original model there is a lot less.
[154:47] Now nanite is dark magic.
[154:49] Unreal is able to handle this amount of polygons really well.
[154:53] But do keep in mind that if you have a lot of meshes with displacements over time it will add up and hurt your performance.
[155:00] Let's cover the most important settings and that is under displacement scaling.
[155:05] So this is where we're able to change the strength of the height map and this is where I recommend you change it.
[155:10] Right now it is set to four.
[155:12] I could increase this to 10 and now you see it's sticking out a lot more from the character's body.
[155:17] Or if I want to bring it down then instead of four we can make it to so it's just a very subtle change.
[155:24] Now generally I do like to leave it at four.
[155:26] I think that is a good value but it's up to you how large and effect the height map displacement should have.
[155:31] This is the equivalent of scaling in the viewport for substance painter.
[155:35] And we also have this center.
[155:37] This is the offset.
[155:38] If I set this to one then we can see that we just moved everything into itself or sent it to zero.
[155:44] And then now the entire object is scaled out.
[155:48] So now he's just a little bit chubbier.
[155:50] Using the center feature is helpful if we have displacement on a flat mesh like the ground here.
[155:55] Now in my case I wanted to keep the original geometry so we leave that at 0.5.
[156:01] Now just because we have displacement this does not replace the normal map.
[156:05] The normal map is still necessary even with displacement.
[156:09] To show what I mean let me scroll up here and we have normal strength.
[156:13] I will turn off the normal map by bringing this down to zero and immediately it's almost like this heart disappeared.
[156:20] If I angle this that's how it's not giving out a shadow.
[156:23] You can't even tell that the heart is supposed to be popping out of the character.
[156:26] And when I bring back my normals to one then that looks a lot more realistic.
[156:31] So do keep in mind you still need normal maps with your height maps to show off the other controls we have in unreal.
[156:38] I very quickly created a variant of this guy where instead of him being a stained metal he is made out of wood.
[156:45] So this was made super quickly in substance painter just using some of the default materials to briefly recap how this character was created.
[156:52] I added in the wood ship hole smart material on top of the entire body.
[156:58] And then in the material section I chose the bark material down here and just dragged it on and mass it out.
[157:05] So it was on the character's body and this material along with a lot of the assets that come in substance painter already has built in height information for displacements.
[157:16] I then added in the face that we created beforehand and a paint layer for the bolts.
[157:22] There is a really cool brush called screw bolt that allows me to automatically paint in bolts with high detail built in now by default.
[157:31] If we go into the high channel you'll see that with opacity of 100 this was way too strong it was sticking out too much.
[157:40] So I lower this to around 50 to bring it down to something more natural which you would expect both to look like.
[157:47] And then on top of everything I use the metal rust material as dirt and then mass it out with the dirt generator.
[157:54] I brought that information for its base color down to 50% also.
[157:59] So very quickly which is a few layers I was able to create a variant of the object back in unreal when you turn on high displacement you'll get some extra settings down here.
[158:09] So let me turn this on and cover them.
[158:12] So the first one is displace amount when I bring this down we remove displacement until at zero we're using the original geometry.
[158:20] And you notice that whenever I am making changes to my height through these parameters the shadows don't update in order to update those shadows you could just wiggle your mesh and the shadows will be fixed.
[158:32] This is just a work with displacement.
[158:34] If you don't want that to happen in the details panel of your static mesh type in shadows and then under shadow cache and validation behavior set this from auto to always.
[158:45] Now if we make any changes to the displacement the shadows will automatically change.
[158:49] Now do keep in mind that this will hurt performance.
[158:52] So you want to set it back to auto when you're done with it.
[158:55] Now I can show off these parameters without worrying about it.
[158:58] So this is just a good way to very quickly decrease the amount of displacement or see what your mesh look like before displacement.
[159:05] And then we have strength as you can guess with strength by increasing this we will get more displacement.
[159:10] Now do pay attention that with all of these settings if you do increase it to a large amount then you'll see that there is a limit to how much displacement can be changed.
[159:20] So now we have hit that limit.
[159:22] So our character is flat again by increasing it.
[159:26] If you do want to get more displacement that is where the magnitude down here is necessary.
[159:31] So by increasing this and then going back to its value we get a much higher range.
[159:39] I'll go ahead and switch this back to five and then with contrast you can play with the strength and the contrast to get an even sharper displacement.
[159:50] So now this height is a lot more exaggerated and he is super super spiky and the dents are more noticeable.
[159:59] And finally we have displacement offset which will move uniformly the high texture up and down for a little bit more control with all those parameters.
[160:10] You have all the necessary settings to handle displacement in unreal.
[160:15] Now that we know how displacement works in substance painter and unreal let's use it in a practical example specifically going back to our high quality sci-fi crate assets.


### Paint Hard Surface Details [160:16]
**Transcript (timestamped):**
[160:25] And for the most part when it comes to assets like this displacement isn't really necessary.
[160:30] This is a hard surface model.
[160:32] You will find the best use of displacement with natural organic assets like trees would and rocks but it can still be helpful in situations like this.
[160:41] Specifically we will be able to paint and add hard surface detail directly in substance painter.
[160:47] So instead of modeling this in something like blender or substance modeler we will paint it in substance painter and a good area to showcase this on this object is to the right here because this area is lacking a little bit of detail.
[161:02] So let's add in a new fill layer for height.
[161:05] This will only affect the height.
[161:07] So hold out Alt and select height right there.
[161:10] I specifically want to take away from the model.
[161:13] So for the height value I'll bring it down to something in the negative range.
[161:17] Now with that in a black mask and a paint effect.
[161:21] Now with the brush tool selected I will go into my alphas and substance painter comes with a bunch of hard surface alphas we can use automatically.
[161:30] Specifically I will select this one.
[161:32] Now I'm using this as my brush and we can even see the icon here as a reminder if you do not see the icon on your brush.
[161:39] Come up here and select full preview cursor with a grayscale value of one.
[161:44] I can start digging into my mesh and by default we do not have this placement enabled.
[161:49] So come up to the shader settings and increase that scale and obviously we want to increase the subdivision count to.
[161:57] Okay that's starting to look good and I can start digging into my mesh.
[162:02] So I'll just stamp this down like this and then rotate my brush and start to paint in those hard surface details.
[162:12] Now do keep in mind that this will not be perfect.
[162:15] I am going pretty quickly because this is just for demonstration.
[162:19] If this wasn't actual assets I would definitely take my time when creating such large details.
[162:25] I will swap out my alpha.
[162:28] I like this one.
[162:39] Of course this is way too harsh of an angle so we will blur this by going to filters and selecting blur.
[162:50] And let's go ahead and let's decrease it to give it a bit of a bevel.
[162:55] Okay this looks really good.
[162:57] Maybe the height is a little bit too strong right now so I will decrease this by increasing it so it is closer to zero.
[163:04] While this is deforming the geometry of my mesh it isn't changing my materials and it kind of looks out of place right now.


### Anchor Points [163:05]
**Transcript (timestamped):**
[163:12] The reason why is because remember we're using a curvature mask to add in some edge wear.
[163:18] And you would expect there to be a curvature mask also on the hard surface detail we just painted.
[163:23] But because this isn't the actual geometry if we go into the curvature mask there is nothing there for the edge wear generator.
[163:31] But that is okay because we can use anchor points to manually add in our changes to the edge wear generator.
[163:40] You can basically think of anchor points as a way to dynamically copy a specific mask.
[163:45] In our case we are going to copy this mask and then use the copied mask somewhere else in my layered stack.
[163:51] Specifically for this model's layers we will use this mask within the edge wear generator to add it to this mask.
[164:00] Since I know I need this mask or this layer generator I have to move this mask that's how it's before the generator.
[164:08] And right now this mask is above the generator which is what we don't want.
[164:12] So what I will do is rename this to heights and I will make this the very first layer in my layer stack.
[164:20] By grabbing it and moving it down here.
[164:22] That's how we can use this layer within all the layers above it.
[164:26] And immediately this will remove it.
[164:28] And that's because if I go into my height channel these folders are set to normal when they should be set to linear dodge.
[164:36] Because a linear dodge will allow us to add height detail on top of each other.
[164:41] These folders are right now replacing the height detail.
[164:44] So in the dropdown instead of normal select linear dodge and also right here select linear dodge.
[164:51] And now we get back to heights.
[164:53] Now to copy this mask elsewhere into my layers all I have to do is select the mask come up to effects and then add in an anchor points.
[165:01] So we can name this anything I'll call this hard surface.
[165:05] And now going back into my steel generator right here and let's view this so we can see what is happening.
[165:13] I will make the property windows bigger and we will see this option called micro details in this dropdown.
[165:20] We have micro height.
[165:22] You want to make sure you turn this on and then this will give me a new input down here called micro height.
[165:29] So go ahead and select this and then go to anchor points.
[165:33] Now we will select the copied mask which we named hard surface and boom instantly this will work.
[165:40] And now we are using the hard surface for my generator.
[165:44] Let's go ahead and view what this looks like.
[165:46] And this does kind of look wrong because instead of it going on the outer surface.
[165:52] It is being added to the inner surface which is what I don't want.
[165:56] So what I can do is change this down here under levels for my micro heights and just click on the invert button.
[166:04] And now it is chipping away at the correct location.
[166:09] I do think that this is a little bit too strong especially compared to the rest of the mesh.
[166:14] So up here under micro details curvature intensity we can bring this down and also play with all these values.
[166:23] Do something like right here.
[166:25] Also remember that we are using another generator to add in the steel painted worn in the ambient occlusion areas.
[166:32] So let's also add my anchor point to this generator.
[166:36] So go ahead select dirt micro details.
[166:39] I'll turn this on for heights and micro heights select that same anchor points.
[166:45] Okay.
[166:46] Now we need to inverse this.
[166:48] That's how it is inside the detail.
[166:50] Right now it is on the edges.
[166:52] So click on invert again and now that we move it inside of it and also play with the intensity here.
[167:03] Okay like that.
[167:04] So I think this looks really cool.
[167:05] So now with height we were able to paint in hard surface details for this crate.
[167:10] I think this looks good for an export.
[167:13] Now let's export my changes and see them in engine.
[167:16] So control shift and e to export and the only texture set that we change was the body.
[167:21] So everything else we do not have to export they could be unchecked and for the template since I want the height we will use the template we just created.
[167:29] So the unreal engine five and height template.
[167:32] So now we are exporting the height map right there and select export back and unreal and since I replaced the originally imported textures.
[167:41] All I have to do with my base color textures is select them right click and go to re import.
[167:47] So this will bring in the new textures and here they are.
[167:51] We can already see the normal map making an effect but I want to give it that geometric displacement.
[167:57] I need to import the height because that is a new texture.
[168:01] So go ahead and place it in there and don't forget to uncheck sRGB.
[168:07] Now let's get the settings for the body material.
[168:12] Enable use height scroll down here.
[168:15] Don't forget to enable tessellation and for heights use the new imported texture right here.
[168:24] If the object doesn't change make sure it's using nanites.
[168:27] There we go.
[168:28] And just give it a little wiggle so the shadows will update and here it is detail that was completely sculpted in substance painter and we could increase its magnitude down here instead of four.
[168:42] Let's try something like six.
[168:45] Okay.
[168:46] So now we can really see the shadows created by the displacement.
[168:50] That is a practical example of how we can use displacement in painter and unreal to create extra detail without having to model them or sculpt them in another program.
[169:01] Now for the end of this video I will briefly cover how we can take our painting assets and breed them into a pre existing unreal environment because after all this time creating these nice textures and materials and even editing the geometry on my object.


### Asset Showcase [169:02]
**Transcript (timestamped):**
[169:16] Let's see how we can use materials in a practical example and some tips for how to make the materials better feel like they are part of the environment.
[169:25] Feel free to use any environment or world that you created.
[169:28] In my case I'll just use one of Epic Games environments called the electric dreams.
[169:32] So this one is really cool and it's the most detailed environment created for Unreal Engine so far.
[169:37] So go ahead and add it to the library and then you can download it through the Epic Games launcher.
[169:42] This is just like migrating any other assets.
[169:45] So to see where this is in my content drawer press control B to jump to this location.
[169:49] Then I'll go ahead and right click asset actions and then select migrates.
[169:54] Now this will find all the assets that are associated with the asset we are trying to migrate.
[170:00] And in my case since we added the materials onto the static mesh unreal knows that I also want to copy over those materials and the textures that material is using.
[170:10] For example if I did want to migrate our meat mat object then by clicking migrates we're only going to migrate the object itself and not any of the materials because we didn't assign the material to the object here.
[170:22] So I would have to migrate them separately.
[170:25] So let's go ahead and go back to the migration for this and then navigate to the new projects content folder and select it.
[170:33] In our new project we will find the migrated assets in the original folders that they were in.
[170:39] So in my case the static mesh was in a folder called Meshes.
[170:42] So now my content browser will go to Meshes and there it is.
[170:46] OK great.
[170:47] So now that's in my project.
[170:48] Let's find a nice little location to plop it down.
[170:51] I think over here looks good and do keep in mind that I did make some changes to this environment.
[170:57] All I did was that I flew around.
[170:59] I found some nice assets that I like.
[171:02] For example maybe this rock right here.
[171:06] And then I just copied and pasted it over in this location to create a nice scenic staging area to show off the object.
[171:14] So within here I will go ahead and grab my object and place it right there.
[171:20] And immediately you will notice that there are some weird texture projections going on to my object and that is because of decals.
[171:28] So these are unreals built in decals that you will often find in the world.
[171:32] If you do not see the decal icon make sure to press the G key to go out of game view mode.
[171:37] Now that I can see the decals affecting the mesh I can select my decal.
[171:42] And when I move this around we'll see that this is just a projection of another material.
[171:47] And I do not want this moss material on top of our object especially since we spent such a long time creating our own nice material.
[171:55] We do not want to hide it right now.
[171:57] So what I can do is that I can grab the decals and then just move it or scale it.
[172:02] That's how it's only affecting the area.
[172:04] I want this decal affecting or an easier way to go about it is to just select my object type in decals and uncheck receive decals.
[172:15] That will prevent my world from affecting the object.
[172:18] And now I can go ahead and place it right here like this right off the bat.
[172:23] Right off the bat my asset looks really amazing.
[172:26] It feels like it belongs in this forest almost like this is maybe an alien world and the military left behind some crates for the player to find or as a background object to an animation.
[172:38] But maybe there is a chance depending on the environment that you think the color of the asset is off or that the materials look weird.
[172:45] And that is because of the environment post processing.
[172:48] So you can change the color of your world as a whole within the post process volume.
[172:53] And we can see within the outliner right now if I type in post process volume down here is the post process volume being used.
[172:59] If I hide that temporarily then my world is a lot more orange.
[173:04] So generally with post process volumes they completely change the color feel and look of your world within another project or another level that might not be using a post process volume.
[173:14] Or using a different one.
[173:16] Then when you import it into another world your asset would look just a little bit different.
[173:21] This is why adjusting colors is important and why it is included in the master material.
[173:26] So let's hop back into my base color.
[173:31] And now you can always change the tint here the brightness the contrast and the saturation to make the object better fit in with the world or whatever color grading the level is using.
[173:43] With these three parameters I can quickly completely change the look of my material.
[173:48] Now in my case I do like the default values so I'll just leave them as is.
[173:54] And with that we are finished with a tutorial.
[173:57] We can see how quickly with substance painter and Unreal Engine we were able to create realistic materials that fit in a realistic environment.


### Ending [174:03]
**Transcript (timestamped):**
[174:06] And what is really cool is that we are leveraging a lot of the features of Unreal Engine 5.
[174:11] We have advanced lighting with Lumen and we are using nanodisplacement.
[174:16] Here's the same crate imported into the environment that we created in the Unreal Engine 5 beginner tutorial.
[174:22] Goes to show how these materials and substance painter workflow can be used for any world.
[174:28] If you like this video and want to support the channel then you can check out the Unreal Masterclass.
[174:33] The Masterclass is an expanding collection of exclusive lessons and tutorials for Unreal Engine 5.
[174:39] In it we take an even deeper dive into Unreal going over animation, architectural visualization, advanced blueprints, programming,
[174:48] how to create a game completely from scratch and much more.
[174:52] The Masterclass isn't just one course.
[174:54] It is a collection of different courses covering every aspect of the engine.
[174:58] So whether you want to learn game development or animation the Masterclass is for you.
[175:03] You can check it out in the description below.
[175:06] And with that we conclude the end of this tutorial.
[175:09] Congratulations on creating your first substance painter projects.
[175:13] Make sure in the comment section below to share your creations.
[175:16] I would love to see them.
[175:18] So until next time.



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
