---
title: Substance Painter Beginner To Pro - Course
source: YouTube
url: https://www.youtube.com/watch?v=UCKwN3QA_FM
author: TriGon
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated on screen; modern Baking Mode UI (Common Settings / cage wireframe / matching-error red-green heatmap) consistent with a post-8.3 era build"
tags: [layers, fill-layer, paint-layer, masks, smart-material, smart-mask, generator, anchor-point, blend-mode, baking, mesh-maps, ambient-occlusion, curvature, high-to-low-poly, cage, id-map, texture-set, pbr, metal-rough, basecolor, roughness, metallic, height, normal-map, alpha, tri-planar, procedural, export, export-preset, channel-packing, game-engine, unreal-export, beginner, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/substance-painter-beginner-to-pro---course/
frame_count: 17
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Substance Painter Beginner To Pro - Course

**Source:** [YouTube](https://www.youtube.com/watch?v=UCKwN3QA_FM)
**Author:** TriGon
**Duration:** 168m3s | 26 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Introduction [0:00]
**Transcript (timestamped):**
[0:00] Welcome to the course, in this course we are going to be learning how to texture in Substance Painter.
[0:06] We are going to be starting from the very basics, going up to an advanced level.
[0:12] And we are going to be doing that by first off taking a look at the basics of Substance Painter.
[0:18] After taking a look at the basics, we are going to go ahead and texture our first asset, which is going to be this letter belt.
[0:26] Now this course is beginner friendly, as we are going to go over everything and we are going to go very slow and structured.
[0:34] And at the end of the video you will have seen the complete workflow of creating these textures.
[0:40] And you can apply it to your own models.
[0:43] In this video will only be part of the full course, don't worry, we are going to completely texture the whole letter belt and you will learn all the basics.
[0:52] But in case you do want to learn more and how to texture more complicated assets and more complicated materials.
[1:01] I will be linking the full course in the description down below, or you can click the link in the video that is going to pop up over here.
[1:10] And this is also going to contain all the model files, so you can follow along with the same model.
[1:16] And that also applies to the letter belt, you will have the model so you can follow along one by one with the course.
[1:23] And this will be an ongoing course, meaning that the more time goes by, the more chapters will be added to the course.
[1:31] Meaning that you will learn more and more complicated workflows.
[1:36] And by signing up to the course platform, you will be directly supporting my channel, allowing me to keep making these videos.
[1:46] And the videos on the course platform will be subtitled in multiple languages, you will see the languages on the screen right now.
[1:56] So yeah, without further ado, enjoy the course.


### Opening Painter [2:04]
**Transcript (timestamped):**
[2:04] So when you open the software, it's going to look a little bit like this.
[2:09] You can hit close, then we go to file, open sample, I'm going to be opening the preview sphere sample.
[2:23] So let's go ahead and familiarize ourselves a little bit more with the UI.
[2:30] And on a note, if your UI looks different, you can go to window and hit reset UI.
[2:37] This will resetted to the default.
[2:41] So over here, we have our viewport.
[2:44] Over here, we have our 2D viewport, where we can see our texture in a 2D format.
[2:53] To switch between these two, we can hit F1, actually F2, to go to the 3D viewport.
[3:01] Then we hit F3 to go to the 2D.
[3:05] And if we hit F1, we can show both.
[3:09] Most of the times you're going to be working with just the 3D viewport, as that's really all that you need.
[3:15] So F2.
[3:18] Let's go ahead and make this UI look a little bit less complicated.
[3:23] So on the right, we have the texture set list.
[3:26] We can just left mouse click the name.
[3:29] And then we can drag it anywhere in the UI.
[3:33] Just going to drop it into the layers.
[3:36] Then we're going to do the same for the properties fill.
[3:39] We're going to change the position of this to be over here.
[3:46] And then lastly, I want to take the assets.
[3:48] I'm just going to move them down here.
[3:54] So we're going to go ahead and move them down here.
[4:00] So let's talk a little bit about navigation.
[4:04] If we hold down alt, middle mouse click, we can pan the view.
[4:10] If we hold down alt, left mouse click, we can rotate the view.
[4:16] Now finally, we have alt, right click mouse to zoom in in the view.
[4:23] So you're practically always holding down alt and just switching between the mouse clicks.
[4:29] To navigate.
[4:31] And then we also have F to focus the view.
[4:34] This is going to center your object in the viewport.


### Exploring Layers [4:39]
**Transcript (timestamped):**
[4:40] So let's get started with some actual texturing.
[4:44] So over here, a texture set list, we can change that to layer.
[4:49] Can drag this out a little bit by left mouse clicking.
[4:52] Get some more space.
[4:54] And everything that you will do in painter is going to be on a layer.
[5:00] Let's start off by just selecting layer one and we're going to say delete.
[5:09] We're going to delete everything that was in our layers stack.
[5:13] That's going to leave us with a blank material.
[5:18] So there's two types of layers.
[5:21] We have the normal layer.
[5:23] This layer, we can paint things.
[5:29] If we go to properties, paint and we scroll down a little bit,
[5:34] you can change the color of that paint.
[5:40] And just like that.
[5:44] This way, you're going to be using a lot less than the next layer.
[5:48] I'm going to show, which is the layer that you're going to be working with most of the time,
[5:53] which is a fill layer.
[5:57] So what this layer does, it fills the whole mesh, everything with the base values.
[6:05] So over here, our color is set to gray and if we change this to red,
[6:10] everything is going to become red.
[6:13] If we adjust the roughness, it's going to become more shiny or less shiny.
[6:23] We up the metallic, the one.
[6:25] Now our surface metallic, if we up the shine on this, we have a nice shiny metallic material.
[6:33] We're going to be talking more about roughness and metallic later on.
[6:36] Now let's focus on just the layers.
[6:40] So a good practice in substance paint is to always name your layers.
[6:45] For example, fill layer one.
[6:47] You can double click this and call this red
[6:52] metal.
[6:58] Now we can create a new fill layer, which is called
[7:04] blue.
[7:06] Let's just go by blue and give this a blue.
[7:09] Color.
[7:12] So we cannot see the red metal anymore, because the blue is on top of the red metal.
[7:20] The whichever layer is on top is the one that's going to be shown.
[7:25] Let's say we take the red metal and we put that one on top.
[7:30] Now it's going to show that instead of the blue.
[7:32] And we can create as many layers as we would like.
[7:39] We can keep rearranging them whenever we want.


### Exploring Channels [7:44]
**Transcript (timestamped):**
[7:45] So let's go ahead and delete all our layers again.
[7:48] We can shift, left mouse click.
[7:51] The last one to select everything in between our selection.
[7:56] We're going to say delete.
[7:58] Let's take a proper view at what channels we have.
[8:03] The channel refers to one of the properties of the material.
[8:07] So we have a color channel, a height channel, roughness channel, metallic channel,
[8:13] normal channel, normal channel.
[8:17] We can ignore this and we can ignore this now.
[8:20] So let's start off by trading a red color.
[8:23] We can go here, we can make this red.
[8:29] And anytime you want to see a channel, we can go from the material channel.
[8:35] We can go to the base color channel, which is the color channel.
[8:39] Now we're going to see just that texture.
[8:43] If I hit the base color channel, it will be the base color channel.
[8:49] If I hit F3, we can see our 2D texture.
[8:54] And since we just have a single color, just going to be a single flat color.
[8:59] I'm going to hit F2 to go back to our 3D.
[9:03] And we can hit M to go back to material.
[9:09] So we can also hit the C key to go to the channel view.
[9:13] And if we hit C again, it's going to show the next channel, the height.
[9:19] The height channel is going to be used for adding some height to a material.
[9:28] To quickly demonstrate this.
[9:31] Let's go ahead and click build my path.
[9:36] This is going to be useful.
[9:38] You should always have this on your side.
[9:40] We can go to start the assets, materials.
[9:44] Actually, we need to unclick this materials because we want to use a map.
[9:49] Let's say in a height, we take anything, we take this thingy.
[9:54] We can take it with the last mouse and drop it in our height slot.
[10:01] Now you can see we can add some detail to that.
[10:07] Now let's go ahead and move on to the next.
[10:12] Move on to the next channel.
[10:13] Again, we can go to material and height.
[10:16] We can take a look at that channel.
[10:24] Whichever part is white is going to be pushed up.
[10:27] And if it's black, it's not going to be pushed up.
[10:31] If we take a look at this white line, we go M for material.
[10:36] You can see it will get height on that.
[10:38] It's not real height, it's just the light reflecting to it.
[10:44] Now let's go to roughness, like I showed you earlier.
[10:50] White is going to be very rough material.
[10:54] If we make it all black, it's going to be super shiny.
[10:59] Again, we can go here and we can put roughness.
[11:02] You can see that texture.
[11:05] Now let's go with something in the middle.
[11:08] It doesn't really matter.
[11:10] And then the last channel that we're going to be worrying about is metallic.
[11:15] This channel is used to tell material,
[11:19] Hey, am I a metal material or am I not a metal material?
[11:25] We put it to one, our material is metallic.
[11:29] We put it to the other.
[11:31] One, our material is metallic.
[11:34] We put it to zero.
[11:36] It's not metallic.
[11:39] This channel is a little bit special,
[11:41] as you usually only want to stick to values of zero and one.
[11:46] So generally speaking, there's some exceptions.
[11:50] You wouldn't be using a value of zero point seven, for example, or like this.
[11:56] Either the material is metal or it's not metal.
[12:01] And let's go ahead and delete this layer.


### Basics Of Masking [12:08]
**Transcript (timestamped):**
[12:08] So I'm going to create two new fill layers.
[12:12] Let's call this one blue.
[12:15] We can hit control D to duplicate our layer.
[12:20] I'm going to call this one red.
[12:23] Let's do one more.
[12:25] Let's call this green.
[12:28] Let's make the green one green.
[12:31] The red one red.
[12:32] And again, it's not going to be shown in red,
[12:35] because we have the green one on top.
[12:37] If we hide the green layer by hitting this eye icon,
[12:42] it won't be shown.
[12:44] We can see that the red is right there.
[12:47] Let's make this one blue.
[12:49] And again, you won't be able to see it until we hide that.
[12:55] Now, of course, this is not very practical,
[12:58] that we can only have one layer visible.
[13:01] So the way that you can mix and match layers is by masking.
[13:06] Let's say we take the green layer.
[13:11] I'm going to right click on the layer.
[13:14] We can say add white mask or a black mask.
[13:19] If we add a white mask, you will see,
[13:22] we can still see the green layer.
[13:24] If we add a black mask, it will disappear.
[13:28] If we alt click on the mask icon right here,
[13:32] we can preview our mask.
[13:34] Let's make this white.
[13:36] Alt click it.
[13:37] You can see that we have a white mask.
[13:41] So what ever part is white on the mask,
[13:45] it's going to show.
[13:47] So what ever part is white here in this layer,
[13:50] it's going to be green on our model.
[13:53] Whatever is black, it's not going to be seen.
[13:57] If we go ahead and paint on this mask,
[14:02] you can see that we can start to erase where it's green.
[14:08] We can start to actually do some stuff with our layers.
[14:14] As you can see here, we have a black square that's being hidden.
[14:19] We paint the black.
[14:21] That's being hidden.
[14:22] We paint the circle with it.
[14:25] You will see that this circle becomes red,
[14:28] because that's the first layer underneath it.
[14:30] So if we hide the red, it's going to turn into blue.
[14:37] Let's go ahead and do a black mask.
[14:40] This is going to have everything disappear.
[14:44] Also to change the color of your mask that you're painting,
[14:50] you go here to the gray scale.
[14:53] You can put it to whichever color you want.
[14:56] Or you can use the short key, the hot key, X to switch on black to white.
[15:06] Let's go ahead and paint out the ring.
[15:12] With a white color, not the best looking mask, but you get the idea.
[15:20] Then I'm pressing X to erase.
[15:29] Now we have a green ring.
[15:35] Now let's do the same for the red layer.
[15:38] This time, I only want to make this one blue.
[15:42] But since I want to have the majority shown,
[15:46] instead of hidden, I'm going to add a white mask.
[15:50] And then with a black color, I'm going to be painting that trim around it.
[16:08] Again, if you mess up, we can use a white color.
[16:12] We can start to say, okay, over here we want to see the layer.
[16:16] And at any time, if we want to change a color,
[16:21] let's say instead of blue, we want to have pink.
[16:26] We just go to the base color and we can adjust the color anytime we want.
[16:32] We can do this for everything.
[16:39] This is going to be a principle that you're going to use all the time,
[16:43] is creating layers and then masking those layers.
[16:48] So be sure to get comfortable doing so.
[16:51] If you didn't quite understand everything that I've shown you, feel free to go back.
[16:56] I also want to show you one more thing.
[17:02] We're not limited to black and white.
[17:05] We can also use gray values.
[17:09] So if we put our gray scale, for example, to 0.5,
[17:16] you will see when we paint now,
[17:21] the effect is going to be less strong than when we put that full white at 1,
[17:27] that full black at 0.
[17:32] And if we put something like 0.8, it's going to be very, very subtle.
[17:38] So the more dark, the more hidden the layer is.
[17:48] And if we use a lighter ray, we'll see that it will only pop through a little bit.


### Saving Your Work [17:59]
**Transcript (timestamped):**
[18:00] So let's go ahead and delete this.
[18:02] I'm going to be creating a new fill layer.
[18:08] Let's make this one yellow.
[18:12] Add a little bit less shine to it by putting down the roughness.
[18:18] We'll be creating a new fill layer.
[18:21] Let's make this one black.
[18:24] Right click at the black mask because we want to hide most of the black.
[18:31] Then we're going to be painting a little smiley face.
[18:39] Because now you should be understanding the basics of substance painting.
[18:45] So the last thing I want to show you is how can we save our work?
[18:50] All that you have to do is go file, save as.
[18:55] Now we can put it anywhere and let's call this, for example, smiley.
[19:02] So now I can do whatever I want.
[19:05] Just mess this up.
[19:07] Now if we go file open or we can say recent files, we can open that file up.
[19:14] You can say discard.
[19:16] It was just saying you have unchanged save.
[19:20] You have unsaved changes.
[19:22] So discard and you'll see that we're back at where we saved.


### Creating The Project [19:28]
**Transcript (timestamped):**
[19:28] So let's go ahead and create our very first real project.
[19:33] So we go file new.
[19:37] Over here you have a bunch of settings for our project.
[19:43] First off, let's go ahead and cover the templates.
[19:47] So these are a bunch of painted templates that you can use.
[19:52] Generally speaking, you can pretty much ignore all of these and just put it to.
[19:59] The first one, BBR metallic roughness.
[20:02] If you're planning to make textures that are going to be used in Unity or Unreal Engine,
[20:11] it can be a good idea to put them on the Unity or Unreal Engine template.
[20:16] And we're going to be covering in a later video what exactly templates are for now.
[20:21] Just put it on the BBR metallic roughness template.
[20:26] Then in file, we're going to need to choose the model that we're going to texture.
[20:31] I'm going to go ahead and select that.
[20:39] We're going to be using the cylinder model.
[20:42] You can find this model in the video is a download link to the cylinder model.
[20:48] So you can work alongside with it.
[20:52] Then the document resolution.
[20:55] It refers to the texture size.
[20:58] So if we put this at 512, for example, we're going to create an image.
[21:04] The image is our texture with a width and height of 512 pixels.
[21:13] The higher the number, the more resolution you're going to have in your texture.
[21:18] Now let's keep this at 248.
[21:22] Normal map format.
[21:24] I like to put this to open GL.
[21:26] Don't worry too much about this.
[21:30] Going to keep this checked on.
[21:32] We're not going to be using Udims.
[21:35] We're going to cover this in a later video as well.
[21:40] We can go ahead and uncheck import cameras and auto unwrap.
[21:46] We're going to ignore baked maps for now.
[21:49] We're going to ignore all the other stuff and we're going to say OK.
[21:53] Now we just created our painted project.
[22:00] I'm going to go ahead and reorganize my UI a little bit.
[22:04] I'm going to track the texture set list to layers properties paint.
[22:09] The left.
[22:10] Let's go ahead and track our assets down.
[22:14] Then we can hit F2 to go full screen on the 3D viewport.
[22:23] Now let's go ahead and talk a little bit about the texture set list.
[22:28] This sounds a little complicated.
[22:31] But all it means is that since we have one texture set right now,
[22:36] we're going to be using one texture for this model.
[22:40] We could be using multiple textures for one model.
[22:43] Then over here you could be switching between the texture sets.
[22:49] So switching between the texture that you want to work on.
[22:53] In this case, all that we need to worry about is double clicking this
[22:57] and we can rename our texture.
[23:00] Let's call this the render.
[23:06] We can also go ahead and change the size of this texture at any time that we want.


### Exploring Smart Materials [23:13]
**Transcript (timestamped):**
[23:14] So now let's get to actually texturing.
[23:18] So we go to layers.
[23:19] Let's also drag this one to the front.
[23:23] Let's go ahead and delete layer 1.
[23:27] We're going to be taking a look at smart materials.
[23:31] So again, we can click over here, filter by path to get some more options.
[23:38] Then over here we can switch between what we want to see of our content browser.
[23:44] So right now we're looking at materials.
[23:48] And look at smart materials, smart masks and so on.
[23:53] So now let's just focus on our smart materials.
[23:59] So these are some presets that we can use that are built up using fill layers like we learned earlier.
[24:07] So let's say if we want a bronze armor material, we can just go ahead and we can select it left
[24:14] mouse and we can drag it either directly on the model or on the layers.
[24:20] This is called your layers stack by the way.
[24:22] Let's just drag it on the model.
[24:25] You can see that we now have a bronze armor on it.
[24:30] So let's go ahead and take a deeper look at what a smart material is exactly.
[24:37] Over here we can see that we have a folder.
[24:41] We can create folders.
[24:42] For example, if we have a fill layer, we can make another fill layer.
[24:47] And then if you select the layers that you want to group together, you can hold down shift,
[24:52] click the next one, then we can right click.
[24:56] We can say group layers or as you can see we can hit control G.
[25:01] Try to get used to using the short key.
[25:04] So we're going to say control G.
[25:06] Now we have a folder and we can name that my folder.
[25:13] So this is basically what a smart material is.
[25:16] If we take a look at bronze armor, you can see that we have a bunch of fill layers and some effects
[25:23] that are grouped together in a folder which is called bronze armor.
[25:28] So knowing that, now we can take a look at how we can adjust a smart material.
[25:35] A good smart material is always defined clearly what each layer is.
[25:41] So over here we can see we have the base metal, we have dirt, surface details, edges, damage and sharpen.
[25:50] So if I look through the names, we can clearly see base metal.
[25:54] If we go there, we can for example choose to change the color of the metal.
[25:59] We take it from a brownish to a white, we're going to get a whiteish metal as you can see.
[26:08] You can go ahead and make this more shiny by making the roughness more black, the more black the more shiny.
[26:16] Let's also go ahead and click the eye.
[26:19] Icon to hide all the other layers on top of it.
[26:32] So you might be thinking now that we just have a fill layer which is a solid color,
[26:37] why do we have these details?
[26:39] That's because we have a finished rough fill effect on top.
[26:43] So if we disable that, you'll see that that this is a solid color.
[26:48] We can do the same for the fill and then you can see that we completely have a boring looking solid material.
[27:02] So we can add fills and effects to break that material up and make it look more realistic.
[27:09] We're not going to cover how to do that yet, I just want you to be aware of why it's not
[27:15] a solid color.
[27:18] And then I'll lay the video, we're going to be taking a look at how we can add that to our
[27:24] self. Now we're just going to be focusing on manipulating smart material.
[27:30] So we can say okay I like the base, let's take a look at the dirt.
[27:36] Dirt's not really visible, let's alt click this.
[27:40] We can see that we basically don't have anything happening with the mask.
[27:46] Click the mask editor, see that we're missing some maps that this material needs.
[27:52] Now let's make it nice and easy, we're going to click over here so we can delete the mask.
[28:01] Now we have a solid black mask.
[28:04] Now we're just going to be painting some dirt in, so I'm going to hit M to switch to our material view.
[28:11] Now over here we can take a look at the brushes, we're going to be changing to a brush.
[28:19] And since we have dirt let's look for a dirt brush.
[28:24] Now over here we have dirt one, we take that.
[28:27] Then over here we can see the color of our brush is black.
[28:32] Let's hit X to go to white.
[28:34] Again hitting X just switches between black and white.
[28:38] Or you can go down.
[28:41] We can take the gray scale up or down.
[28:46] Now let's go with a full white.
[28:49] Now we can start to paint some dirt on our material.
[28:58] Don't worry about how this looks, just get a custom braided to painting some dirt.
[29:09] Now let's say if we want a little bit of dirt we can take this intensity down to maybe point of four.
[29:16] Now we'll be painting the dirt with a lower opacity.
[29:20] Again if we alt click the mask we can check our mask out.
[29:27] We can go even lower to have it more subtle.
[29:32] Then M to go back to material view.
[29:35] Now we can see that we have our dirt.
[29:38] Although this dirt doesn't look like mud how I want it to look like.
[29:45] We're going to click on the layer icon.
[29:50] Now in the base color we're going to be changing this to a brown.
[29:53] Now let's take the roughness down or up.
[29:59] Now we can hit speed to go to channel.
[30:02] I'm going to go to our base color.
[30:05] I'm going to be adjusting that color a little bit more.
[30:11] So we get something that we like.
[30:13] Now I'm going to hit M to see how that all looks like.
[30:17] I'm happy with how that looks.
[30:21] Enable the surface details.
[30:28] This doesn't really do anything because we're lacking a mask.
[30:32] Now let's just delete this.
[30:34] Let's delete and edges damage.
[30:38] Let's also add some more details.
[30:40] Now let's just delete this.
[30:43] Let's delete and edges damage.
[30:46] Let's also delete that one.
[30:49] And then we're going to be enabling our sharpen.
[30:53] Now we've added our first smart material.
[31:01] What I want to show you with this is why smart materials are so practical.
[31:07] Because at any time if you want to make any changes to your material
[31:12] you can just go to a specific layer.
[31:16] Then we can go ahead and change the values of that layer.
[31:22] Which is going to result in a different looking material.
[31:26] So let's go ahead and delete this.
[31:30] Let's go back to our smart materials.
[31:33] I'm going to be creating something that looks a little bit nicer.
[31:38] Let's go ahead and go with maybe machinery.
[31:42] Let's drag that. See how that looks.
[31:44] It looks very boring.
[31:46] Delete that one.
[31:48] Maybe jade.
[31:50] That one looks pretty cool.
[31:52] Let's go with that one.
[31:54] But I do want to make this a white jade.
[32:00] So instead of looking at the video, pass the video.
[32:04] Try to make it white yourself.
[32:08] And if you didn't figure out how to do it, I'm going to show you now.
[32:12] We open up our smart material.
[32:16] We go to base.
[32:18] We adjust the base color to a white.
[32:24] Now in the AO darkness.
[32:26] I'm going to be changing this to a white as well.
[32:30] As it's adding color.
[32:32] Blue with colors.
[32:34] Let's make this a white ish as well.
[32:36] Vines has a little bit of green.
[32:38] Let's go ahead and make that white.
[32:42] We're just going to be going through all the colors.
[32:44] And we're going to be making everything white or gray.
[32:50] Now we have a white looking material.
[32:54] It's also up roughness a little bit.
[32:56] The base.
[32:58] So we have some nice looking reflections.
[33:03] And then lastly, let's go ahead and add a second.
[33:07] Smart material.
[33:09] Let's go with a leather.
[33:11] A smart material we can look for.
[33:13] Leather.
[33:15] Then we can just take one that we like.
[33:17] Go ahead and try to go with the.
[33:19] Leather.
[33:21] Colfgrain.
[33:23] I see how that looks.
[33:25] I'm just going to drag it in the layers stack.
[33:27] If I drag it underneath it.
[33:29] I'm going to drag it underneath it.
[33:31] If I drag it underneath nothing happens.
[33:34] Let's go ahead and delete that.
[33:36] Instead I'm going to drag it on top.
[33:38] Just laying on top of it.
[33:40] Now you can see that we have a leather.
[33:42] Since I want to show both.
[33:44] We need to create a mask.
[33:46] I'm going to right click.
[33:48] I'm going to say add black mask.
[33:50] Now we have a black mask.
[33:52] I'm going to add black mask.
[33:54] I'm going to add black mask.
[33:56] I'm going to add black mask.
[33:58] I'm going to add black mask.
[34:01] Then we can go ahead.
[34:03] And we can use.
[34:05] Polygon.
[34:07] Pill.
[34:09] So there's a tool that you're going to be using all the time.
[34:13] Now over here we can say.
[34:15] This polygon.
[34:17] Needs to be filled with white.
[34:19] So we take a look at the mask.
[34:21] You can see this polygon is white.
[34:23] Which means it's going to show.
[34:25] That smart material.
[34:27] This works the same as masking.
[34:29] As masking in Photoshop.
[34:31] To that.
[34:33] Control Z.
[34:35] To go back.
[34:37] Let's go ahead and drag.
[34:39] Just align like this.
[34:41] Over the top.
[34:43] Now when we go back to paint.
[34:45] The white frame will disappear.
[34:47] Now we have a model.
[34:49] With some stone.
[34:51] And some leather on it.
[34:53] So I think my leather would look better.
[34:55] If it was a black leather.
[34:57] So it matches better with the white.
[34:59] We can open up the leather.
[35:01] We go to base.
[35:03] And we adjust the color.
[35:05] That's a black leather.
[35:09] Let's also go ahead.
[35:11] And mess with the roughness.
[35:13] To make it more or less shiny.
[35:17] Let's go with something like that.
[35:21] So by now you should be.
[35:23] A little comfortable.
[35:25] With dragging smart materials.
[35:27] Into the layers stack.
[35:29] Adjusting the values.
[35:33] You don't feel comfortable yet doing so.
[35:37] You can go ahead and take a look again.
[35:39] At this lesson.
[35:41] And go over it again.
[35:43] Because this is going to be a very important principle.
[35:45] In texturing.
[35:47] You should be feeling somewhat comfortable.
[35:49] With it at this point.
[35:51] Don't worry though.
[35:53] In much more depth.
[35:55] In the later videos.


### Exploring Filters [35:58]
**Transcript (timestamped):**
[36:01] Let's go ahead and delete all this.
[36:05] I'm going to be talking about.
[36:07] Filters.
[36:09] Which is going to be another very important.
[36:11] Useful feature.
[36:13] Let's go ahead and choose one of the ladders.
[36:15] Maybe this one.
[36:19] And filters are very practical.
[36:21] Because they allow you to quickly.
[36:23] Adjust things on the fly.
[36:27] Let's say.
[36:29] If we don't like the color of this material.
[36:33] We could either open up.
[36:35] Our smart material.
[36:37] Look for where we're adding the color.
[36:39] So maybe over here.
[36:43] And we can change the color in here.
[36:47] Or what we can do.
[36:49] Instead of going into our smart material.
[36:51] And look for where we're setting the color.
[36:55] You can go.
[36:57] Filters.
[36:59] You can take a HSL.
[37:01] Which stands for Hue Saturation Lightness.
[37:03] We're going to put this all the way.
[37:05] On top.
[37:07] Of our layers.
[37:09] Within the smart material.
[37:11] And if we want to make.
[37:13] This a different color.
[37:15] You can adjust the hue.
[37:17] For example.
[37:19] The color of the material.
[37:23] Let's say we want.
[37:25] A brownish looking material.
[37:29] You can get like a yellowish.
[37:31] Then we're going to.
[37:33] Down the saturation a little bit.
[37:35] As more with the hue.
[37:39] And maybe we want this to be a little bit less.
[37:41] Bright.
[37:43] And we can lower.
[37:45] The color.
[37:47] So you might be thinking.
[37:49] Why should I do this.
[37:51] Instead of just going to the base.
[37:53] And doing the color over there.
[37:55] And.
[37:57] If you remember from the last.
[37:59] Video.
[38:01] If we go to.
[38:03] Smart materials.
[38:05] And we look for that jade material again.
[38:07] If we drag this on top.
[38:09] Let's say we want to make this a red.
[38:11] Material.
[38:13] We can go to base.
[38:15] We can make this red.
[38:17] But as you see.
[38:19] We still have a lot of other colors in it.
[38:21] Because we have so many elements.
[38:23] In this.
[38:25] Material that are making up the color.
[38:27] It would be more time consuming.
[38:29] To go into every layer.
[38:31] And make that red.
[38:35] Just going to undo all this a little bit.
[38:37] A stragg to jade.
[38:39] Again.
[38:41] Actually we already had one.
[38:43] That's the later one.
[38:45] So instead of going layer by layer.
[38:47] Adding red tones to it.
[38:53] We can just go to filters.
[38:55] Hue saturation.
[38:57] Drag this all the way on top.
[39:01] Now we can say hue.
[39:03] And we're going to change that until it turns red.
[39:05] So we're going to change that until it turns red.
[39:09] Up to saturation.
[39:11] And put the lightness down a little bit.
[39:17] So that's going to be a lot faster.
[39:21] One thing.
[39:23] It's important where you place the saturation effect.
[39:25] One thing.
[39:27] We take this and we put it all the way down.
[39:29] We take this and we put it all the way down.
[39:31] It's only going to be applied.
[39:33] To our base.
[39:37] It's going to be applied to everything.
[39:39] That's underneath our effect.
[39:43] So this can allow for rapid iteration.
[39:45] On the look of your material.
[39:49] We don't need to go layer by layer.
[39:51] And we can just adjust things.
[39:55] Let's go ahead and delete our jade.
[39:57] And go back to our letter.
[39:59] And go back to our letter.
[40:03] Effects are not limited to just color.
[40:05] We can apply it to each channel.
[40:11] Let's say the roughness that we have over here.
[40:13] Again roughness decides how shiny the material is.
[40:15] Again roughness decides how shiny the material is.
[40:17] Or how rough.
[40:21] So let's say I want this material.
[40:23] So let it to be more rough.
[40:25] Again we could look in our
[40:27] dark material.
[40:29] Probably have to go with the first one.
[40:31] And look for the roughness.
[40:33] But sometimes we don't want to look.
[40:35] And we just want to do quick adjustments.
[40:41] So we can use any effect that we have.
[40:45] But now I'm just going to use the HSL again.
[40:47] Keep it nice and simple.
[40:51] And I'm going to drag that on top.
[40:53] So if we want something to be more rough.
[40:59] It needs to be lighter in color.
[41:01] We can drag up the lightness.
[41:03] You will see.
[41:05] That it's not just in roughness.
[41:07] But the color.
[41:09] That's because on top of our filter.
[41:13] We have some buttons.
[41:15] Which are going to decide to what channel
[41:17] to apply the effect.
[41:19] If we put this to height.
[41:21] It will also apply to height.
[41:23] If we apply it to roughness.
[41:25] It will apply to roughness.
[41:27] You can see as soon as we applied it to roughness.
[41:29] Our material became less shiny.
[41:33] The one little tip that you should remember.
[41:37] If you just want it to be applied to one channel.
[41:39] You can hold down alt.
[41:41] And click that channel.
[41:43] I'm holding alt and clicking roughness.
[41:45] Now it's only going to be applied to the roughness.
[41:47] If I hold down alt color.
[41:49] Only to the color.
[41:51] Let's put it to roughness.
[41:55] Then we can decide with the slider.
[41:57] How shiny the material is.
[42:01] Or how rough the material is.
[42:03] Let's go with a very.
[42:05] Rough looking.
[42:07] Leather.
[42:11] For good practice.
[42:13] If we're using filters.
[42:15] Let's go ahead and make sure that we name our filters.
[42:19] Because this quickly becomes very.
[42:21] Difficult to keep track of.
[42:23] If we have multiple effects.
[42:27] So what we want to do is we take our first one.
[42:29] And we say.
[42:31] Color.
[42:35] Adjustment.
[42:37] Then the next one we're going to call.
[42:39] Roughness.
[42:43] Adjustment.
[42:45] Adjustment.
[42:47] So this way we know exactly what it does.
[42:49] And we can easily toggle it off.
[42:51] And on.
[42:53] If we say.
[42:55] Hey.
[42:57] This letter is too rough.
[42:59] Will be very easy to open our.
[43:01] Material.
[43:03] Look on the top.
[43:05] To where we have our filters.
[43:07] Select the roughness.
[43:09] Then to adjust that filter.
[43:11] We have to click.
[43:13] Over here on our filter.
[43:15] Then we adjust that.
[43:17] Now we have a shiny.
[43:19] Leather again.
[43:23] So filters are very nice.
[43:25] Quickly iterate.
[43:27] Over your material.
[43:31] That's a little extra.
[43:33] That shows some.
[43:35] Other filter stuff.
[43:37] I'm going to keep this very nice.
[43:39] And simple.
[43:41] And this is going to sharpen everything up.
[43:43] So if we hit C.
[43:45] C, C, C, C.
[43:47] And we look for the base color.
[43:49] You can see that we can adjust the sharpness.
[43:51] Of that.
[43:53] That's very nice.
[43:55] And we can also.
[43:57] Adjust.
[43:59] That's very nice.
[44:01] And we can see that.
[44:03] That's very nice.
[44:05] So we have a very nice.
[44:07] That's very nice.
[44:09] And we have just a sharpness.
[44:11] Of that texture.
[44:13] This can help make it look a little bit more detailed.
[44:15] Usually.
[44:17] Don't want to go with a very extreme texture.
[44:19] With a very extreme.
[44:21] Sharpness.
[44:23] Intensity.
[44:25] As it will make the texture look very burnt.
[44:27] And pixelated.
[44:29] Usually you want to keep this nice.
[44:31] And subtle.
[44:33] Now we have a nice.
[44:35] Sharp looking.
[44:37] So.


### Saving The Project [44:39]
**Transcript (timestamped):**
[44:39] Finally.
[44:41] Now that we're all ready.
[44:43] Let's go ahead and save our project.
[44:45] Let's go ahead and save our project.
[44:47] Let's go ahead and save our project.
[44:49] So we don't lose our work.
[44:51] We go.
[44:53] And we say save.
[44:55] S.
[44:57] S.
[44:59] S.
[45:01] Then over here we're going to need to choose a name.
[45:03] S.
[45:05] So you want to name your project.
[45:07] Based on the model.
[45:09] That you text string.
[45:11] Let's say you're modeling.
[45:13] Character. Night.
[45:15] The night is called dark night.
[45:17] Then you'd call this project.
[45:19] Dark.
[45:21] Night.
[45:23] Or something along those lines.
[45:25] Now let's go ahead and call this.
[45:27] Thillender.
[45:29] Texturing a cylinder.
[45:31] Now we just say save.
[45:33] That's it.
[45:35] Now anytime we close.
[45:37] Painter we can go ahead and say file open.
[45:39] We can go ahead and open.
[45:41] File.
[45:43] So we can open our cylinder.
[45:45] So if you do want to find this file.
[45:47] I'm going to be.
[45:49] Putting it down below the video.
[45:51] So you can download it.
[45:53] And have a look at it.
[45:55] In case you want to.
[45:57] If not.
[45:59] This is going to be the end of this chapter.
[46:01] Next chapter we're going to be taking a look.
[46:03] Creating a more advanced project.
[46:05] Which is going to be a little bit more useful.
[46:07] By actually texturing.
[46:09] An asset in production.
[46:11] So make sure that everything.
[46:13] That I call fit in this chapter.
[46:15] Is clear.
[46:17] So we can move on to the next chapter.
[46:19] And we can make it.
[46:21] A little bit more complicated.
[46:23] And fun.
[46:25] So to start this new chapter.


### What Are Baked Maps [46:27]
**Transcript (timestamped):**
[46:27] Off.
[46:29] We're going to be creating a more advanced project.
[46:31] We're going to be texturing.
[46:33] This letter belt.
[46:35] That I made a while ago.
[46:37] I'm going to show you how I would do this.
[46:39] In a production pipeline.
[46:41] So we're going to act.
[46:43] Like this is a real asset.
[46:45] And we're going to go through the whole workflow.
[46:47] Of texturing it.
[46:49] So before we jump into that.
[46:51] Let's quickly explain what a baked.
[46:53] Map is.
[46:55] So we're going to go ahead and.
[46:57] Map is.
[46:59] So whenever you're doing something in 3d.
[47:01] You're going to have a high.
[47:03] Polly.
[47:05] And a low Polly.
[47:07] The high Polly is going to be very dense.
[47:09] In polygons.
[47:11] Because we're going to put all our skull.
[47:13] Detail into this.
[47:15] Then once we finish the high Polly.
[47:17] We need to have a low Polly.
[47:19] This will be a version of that.
[47:21] Mesh.
[47:23] With less polygons.
[47:25] More optimized to put.
[47:27] In game.
[47:29] This one will also have UVs.
[47:31] In which we're going to put.
[47:33] The textures on the.
[47:35] In painter.
[47:37] But.
[47:39] Before we get the texturing.
[47:41] We need.
[47:43] We need to get the detail from a high Polly.
[47:45] Back onto our low Polly.
[47:47] Because we don't want to lose all this work.
[47:49] So.
[47:51] I'm going to be.
[47:53] So I'm going to be.
[47:55] Showcasing two.
[47:57] Big maps.
[47:59] As an introduction to this chapter.
[48:01] And let's start off with a normal map.
[48:03] The normal map.
[48:05] Is going to be responsible.
[48:07] For the detail.
[48:09] If we go to.
[48:11] Maya.
[48:13] We can put a normal map on this.
[48:15] And then it will change.
[48:17] How the light.
[48:19] Reacts.
[48:21] Making it look more detailed.
[48:23] This is going to sound a little bit.
[48:25] Fake and complicated.
[48:27] But don't worry.
[48:29] You don't need to know how anything of this works.
[48:31] I just want to let you quickly.
[48:33] Know more or less.
[48:35] How it works.
[48:37] But don't worry if you don't get it.
[48:39] It's not important.
[48:41] So we go to Photoshop.
[48:43] We can take a quick look at.
[48:45] How our normal map looks.
[48:47] So you'll see like a blueish reddish.
[48:49] Map.
[48:51] Which is going to have all our details.
[48:53] Of our high poly.
[48:55] Then the other.
[48:57] Map that I wanted to showcase.
[48:59] Is going to be the ambient occlusion.
[49:01] Map.
[49:03] Again this map to bring detail back.
[49:05] This mostly going to be to bring.
[49:07] That those back from our high.
[49:09] Polly on a low Polly.
[49:11] These are all baked.
[49:13] Shadows which are going to be.
[49:15] Like fake shadows on a low Polly.
[49:17] But to get that.
[49:19] Shadow of the details of the high poly back.
[49:21] So again like I said.
[49:23] If you don't understand this yet.
[49:25] Don't worry about it.
[49:27] You don't need to know it.
[49:29] And in the next.
[49:31] Video I'm going to showcase you how we can get those.
[49:33] Maps.
[49:35] So let's get started with actually.
[49:37] Texturing our letter bell.


### Setting Up Our Project And Baking Maps [49:39]
**Transcript (timestamped):**
[49:39] Also you can find the letter bell.
[49:41] Model.
[49:43] So we go to the top.
[49:45] You can find the letter bell.
[49:47] Model.
[49:49] Underneath the video in a zip file.
[49:51] And will contain the high Polly.
[49:53] That we need for baking.
[49:55] And the low Polly.
[49:57] So you should download that.
[49:59] Then we can go new.
[50:01] Going to select the template.
[50:03] Again we're going to be sticking to PBR metallic roughness.
[50:05] Select the file.
[50:07] And you want to click it.
[50:09] Belt low.
[50:11] FBX.
[50:13] Set the resolution to 4k.
[50:15] If your computer is not great.
[50:17] You can keep this at 248.
[50:19] You can also change this later on.
[50:21] So don't worry about the resolution.
[50:23] You choose.
[50:25] Open GL.
[50:27] And then the rest we can all leave as it is.
[50:29] Open GL.
[50:31] And then the rest we can all leave as it is.
[50:33] Open GL.
[50:35] Now we just say OK.
[50:37] Open GL.
[50:39] Now we have our project created.
[50:41] So a good habit is.
[50:43] The first thing that you do when you create a project.
[50:45] You go file.
[50:47] And we're going to save the project.
[50:49] I'm going to save out this project.
[50:51] And I'm also going to be.
[50:53] Giving you the file at the last video of this course.
[50:55] In case you do want to dig in my painter file.
[50:57] And look around.
[50:59] And that will be available underneath.
[51:01] And you can also save the project.
[51:03] And you can also save the project.
[51:05] And you can also save the project.
[51:07] And I'm also going to be giving you the file.
[51:09] And that will be available underneath the video.
[51:11] As well then.
[51:13] Of the last video of chapter 5.
[51:17] Let's go ahead and call this letter.
[51:19] Bell.
[51:23] And save.
[51:25] So let's go ahead.
[51:27] And showcase you how to bake your maps.
[51:29] To get the detail from the high poly bag.
[51:31] Like we talked about.
[51:33] In the last video.
[51:35] The one click this cross sign.
[51:37] The one click this cross hand icon.
[51:41] Then it's going to open up some complicated looking stuff.
[51:43] Although we need to do for now is taking.
[51:45] The baking log.
[51:47] And we're going to drag that.
[51:49] To the right.
[51:53] Now over here at high definition.
[51:55] Meshes.
[51:57] We're going to click this page icon.
[51:59] Now we're going to choose a belt.
[52:01] And the score high fbx.
[52:03] Now give some time to load.
[52:05] Once that's there.
[52:07] We can go ahead.
[52:09] And we can go to high.
[52:11] And we're going to hide that.
[52:13] Also we're going to hide the cage.
[52:15] So we can just see the low poly.
[52:17] Now that we have our high poly.
[52:19] Load it.
[52:21] And we've hidden it.
[52:23] We're ready to do a bake.
[52:25] Now we have our high poly.
[52:27] Load it.
[52:29] And we've hidden it.
[52:31] Now we're ready to do a bake.
[52:35] So over here we have.
[52:37] The baked maps that we want.
[52:39] Again now you should recognize the normal map.
[52:41] And the ambient occlusion.
[52:43] Like we talked about.
[52:45] But we have a bunch more world space.
[52:47] ID, curvature, position, thickness, height.
[52:49] Bed, normals and opacity.
[52:53] The last three.
[52:55] You don't really need to worry about too much.
[52:57] We're going to ignore them for now.
[52:59] And let's quickly go over each map.
[53:01] So the normal map is going to give detail.
[53:03] By making the surface react to light.
[53:05] In a different manner.
[53:07] The world space normal is kind of more
[53:09] less the same.
[53:11] You don't really need to worry about it.
[53:13] But you're going to be using it for your
[53:15] masks that you're going to create.
[53:17] The ID map is going to be an
[53:19] important map to create masks.
[53:21] For our smart materials.
[53:23] The ambient occlusion.
[53:25] The ambient occlusion.
[53:27] The ambient occlusion.
[53:29] Again it adds that fake
[53:31] shadow of the high poly.
[53:33] Then for curvature,
[53:35] position and thickness.
[53:37] Don't worry too much about them either.
[53:39] They're just going to be there to help us
[53:41] create masks.
[53:43] The only three important maps
[53:45] they should worry about is the normal map.
[53:47] The ID map.
[53:49] And the ambient occlusion.
[53:53] With the ID we need to
[53:55] change one thing.
[53:57] We need to do the color source from
[53:59] material color to vertex color.
[54:03] And the reason why
[54:05] is because in Zbrush.
[54:07] We've set up a poly paint.
[54:11] And we're basically telling
[54:13] Zbrush hey,
[54:15] for each element we're going to give it
[54:17] a different color.
[54:19] And then we can bake that color down
[54:21] onto a low poly.
[54:23] And with that color we can create
[54:25] selections in paint.
[54:27] Again this sounds complicated,
[54:29] but it will be very easy once
[54:31] you see it in action.
[54:33] But for that
[54:35] to work we do need to say that we need
[54:37] to take the vertex color.
[54:39] Now we're
[54:41] pretty much ready to go.
[54:43] Let's go ahead and put
[54:45] anti-aliasing at 64.
[54:49] Actually for now I'm just going to do
[54:51] a little bit of baking to showcase something.
[54:53] Let's put the output size to
[54:55] 4k.
[54:57] Even if your project is set at 1k
[54:59] or 2k.
[55:01] It's best to bake it in double the resolution.
[55:03] Let's say
[55:05] if your final texture is going to be in 2k
[55:07] you should be baking in 4k.
[55:11] One exception.
[55:13] If your final texture is going to be 4k
[55:15] just bake it at 4k
[55:17] because 8k is going to be an extreme
[55:19] size to work with.
[55:21] But for now we can just
[55:23] hit bake selected
[55:25] textures.
[55:29] Depending on your PC
[55:31] this can take a little bit longer
[55:33] or a little bit shorter.
[55:37] Now if we take a look
[55:39] at our low poly
[55:41] you can see that we have all the detail
[55:43] back of our high poly.
[55:45] Now we actually get something that looks
[55:47] quite nice.
[55:53] One thing that you might
[55:55] notice is that we have a few
[55:57] weird things going on
[55:59] where we have intersections.
[56:03] For example over here it's baking
[56:05] projecting the buckle
[56:07] onto the leather belt.
[56:09] One way to avoid that
[56:11] is to separate your mesh
[56:13] in different meshes.
[56:15] So if we take a look at the Maya
[56:17] you can see that we have a
[56:19] buckle low with just the buckle.
[56:23] A belt low with just the belt
[56:25] and a buckle clip.
[56:27] The reason I
[56:29] am separating the clip
[56:31] from the buckle for exception
[56:33] for exception
[56:35] for example, sorry
[56:39] is that these are intersecting
[56:41] with each other.
[56:43] So if we were to bake them together
[56:45] in the same baking group
[56:47] we would get some
[56:49] projection errors over here.
[56:51] And then in ZBrush
[56:53] you want to separate
[56:55] the high polys
[56:57] as well.
[56:59] You can see you have the belt high, the buckle high
[57:01] and the buckle clip high.
[57:05] So in order for that to work
[57:07] in Painter we need to do one thing
[57:09] we need to go to
[57:11] Match and say by mesh name.
[57:17] So when you are doing this it is important
[57:19] that your mesh names are the same.
[57:21] The belt underscore low, buckle underscore low
[57:23] if we take a look in ZBrush
[57:25] you will see that they match.
[57:27] The only thing that should
[57:29] match is the suffix.
[57:31] So after the name
[57:33] it should be underscore low
[57:35] or underscore high.
[57:37] So we go to Painter
[57:39] we can check if the matching by name
[57:41] is set up correctly
[57:43] by going to Match and by name.
[57:45] You can see that the buckle low
[57:47] has the buckle high and so on.
[57:49] If this is a mismatch
[57:51] it will put
[57:53] a red name here
[57:55] with the mismatched name.
[57:59] So now if we take a look at this
[58:01] little baking issue
[58:03] if we bake the text just again
[58:09] we will see that
[58:11] the text is not
[58:13] in the same way.
[58:15] You can see that that
[58:17] disappeared
[58:19] because right now it is just baking
[58:21] the buckle into the buckle
[58:23] that will give you
[58:25] much nicer bake.
[58:29] So after you bake you want to check
[58:31] all over your mesh
[58:33] if you have any
[58:35] issues popping up with your bake
[58:39] it seems that everything
[58:41] is baking fine
[58:43] except for this
[58:45] area.
[58:53] When you have a little bake
[58:55] issue with that one of the first things
[58:57] that you can check is your UVs.
[58:59] If those are all alright
[59:01] it means that you need to adjust
[59:03] the settings a little bit.
[59:05] So what we can do is
[59:07] we are going to enable the cage surface
[59:09] the cage wireframe
[59:11] and let's show the high poly mesh.
[59:13] The next step
[59:15] we are going to hide the low poly.
[59:21] Go ahead and make the opacity of the cage
[59:25] a little bit stronger.
[59:27] Let's give this another color
[59:29] go with like
[59:31] greenish color or whatever.
[59:37] What does this mean
[59:39] this cage?
[59:41] We take a look at the low
[59:43] let's hide the high poly actually
[59:47] you will see that the cage
[59:49] has the same
[59:51] wireframe
[59:53] as our low poly.
[59:57] We take a look at this
[59:59] and go to Maya
[60:01] you will see that it will have the same.
[60:03] It's basically an inflated mesh
[60:07] and we can choose how inflated it is.
[60:13] It's going to look for the high poly
[60:15] until it hits the cage.
[60:19] So imagine it going like this
[60:21] and looking for the high poly.
[60:25] But sometimes your cage
[60:27] can start to intersect
[60:29] and can result in weird baking errors.
[60:33] The best way to bake
[60:35] is you can show your high poly
[60:37] high to low poly
[60:41] and then we want to try to push the cage
[60:43] as close as possible
[60:45] to the high poly
[60:47] without intersecting.
[60:49] As soon as we intersect
[60:51] you can see that we have a matching error
[60:53] in red.
[60:55] So we want to try to push that
[60:57] as close as we can
[61:01] until we have no red.
[61:05] We can see that
[61:07] we have no red.
[61:13] All the way up until here
[61:17] which is probably not enough
[61:19] to fix that issue
[61:21] but let's go ahead and give that a try.
[61:25] We are going to hide everything except the low poly.
[61:27] Let's try to bake that again.
[61:35] You can see that wasn't enough to fix it.
[61:41] So sadly whatever value
[61:43] I put I wasn't able to fix
[61:45] this issue right here.
[61:47] This is one of the
[61:49] more painful parts of baking with Painter.
[61:53] Painter doesn't give you a lot of options
[61:55] to fix baking issues.
[61:57] Which is why I personally
[61:59] in my own work I bake with Mama Set
[62:01] because we have more control over
[62:03] the bake.
[62:05] And then I import those baked maps
[62:07] in Painter and texture with them.
[62:09] But for now let's keep it
[62:11] nice and simple.
[62:13] We are going to just be working
[62:15] with that little issue.
[62:17] If you really wanted to fix it
[62:19] in Painter you could do like
[62:21] two bakes.
[62:23] And you separate this mesh
[62:25] from this and then combine
[62:27] the two maps that you baked in Photoshop
[62:29] and you paint it out.
[62:31] But for now let's just
[62:33] focus on this.
[62:37] So if everything bakes
[62:39] well how you want it to bake
[62:41] then we can go ahead
[62:43] and go to NTA lysing.
[62:45] Put this at 64.
[62:47] Then we are ready to bake.
[62:49] Again this is going to make everything
[62:51] look a little bit nicer and softer.
[62:53] But this is going to take a little bit more time.
[62:55] This is why you usually first do a quick test bake.
[62:57] With a little bit of a lower resolution.
[62:59] Especially if you have a computer
[63:01] that's not too fast.
[63:03] Then once we are happy with the bake
[63:05] we put super sampling on 64
[63:07] and we bake the textures.
[63:09] And we are ready to bake.
[63:11] Let's go ahead and start.
[63:13] So let's start with the text.
[63:15] We are going to do a quick test bake.
[63:17] With a little bit of a lower resolution.
[63:19] Especially if you have a computer
[63:21] that's not too fast.
[63:23] Then once we are happy with the bake
[63:25] we are ready to bake.
[63:27] Music playing
[63:53] You will see that it looks
[63:55] a little bit nicer.
[63:57] The bake.
[63:59] We can preview each baked map by hitting B.
[64:01] Then we can just go
[64:03] in between the bakes.
[64:05] Music playing
[64:07] You can see our ID is empty.
[64:09] Seems that we forgot
[64:11] to put it to vertex color.
[64:13] Music playing
[64:15] Let's put that to vertex color.
[64:17] Music playing
[64:19] I am going to go ahead and disable the other maps.
[64:21] Because I only need to bake
[64:23] the ID map again.
[64:25] That will make it a little bit faster.
[64:27] We only bake one map.
[64:29] Music playing
[64:31] Also let's go back to our settings.
[64:33] For the ID map we should
[64:35] put the NTA lysing at none.
[64:37] Music playing
[64:39] Then we can just bake that texture out.
[64:41] Music playing
[64:43] You will see that we get our colors back now.
[64:45] Music playing
[64:47] So that's it for baking the maps.
[64:49] In the next video we are going to be
[64:51] setting up our project.
[64:53] Music playing
[64:55] But before we do so let's go ahead
[64:57] and make a quick save.
[64:59] Music playing
[65:01] So we don't need to bake again
[65:03] in case paint crashes at some point.
[65:05] Music playing


### What Are ID Maps [65:06]
**Transcript (timestamped):**
[65:07] So if we switch back to the
[65:09] paint brush icon we can go
[65:11] to painting mode.
[65:13] Music playing
[65:15] And let's go ahead and talk a little bit more
[65:17] about ID maps.
[65:19] We covered it really quick
[65:21] earlier in the Zbrush.
[65:23] Music playing
[65:25] Where I showed you the colors and we can use
[65:27] these colors to mask
[65:29] out our stuff and paint them.
[65:31] Music playing
[65:33] So we can go over here
[65:35] in the mesh maps and we can say ID.
[65:37] Music playing
[65:39] Music playing
[65:41] Now I noticed that I have
[65:43] a little big error.
[65:45] We forgot to go ahead
[65:47] and match it by mesh name.
[65:49] So I'm just going to re-bake
[65:51] and then we get back.
[65:53] Music playing
[65:55] So you can see after we bake with
[65:57] match by name
[65:59] that that error is gone.
[66:01] Music playing
[66:03] So let's say I want to
[66:05] mask the blue.
[66:07] We can create a fill layer.
[66:09] Music playing
[66:11] We right click and instead of clicking
[66:13] add white mask or black mask
[66:15] we can say add mask with
[66:17] color selection.
[66:19] Music playing
[66:21] On the left we can choose pick color.
[66:23] Music playing
[66:25] Now we can choose a color where we want
[66:27] that mask to be applied to.
[66:29] Music playing
[66:31] Let's go ahead and make this blue.
[66:33] Music playing
[66:35] You can see that it just applied to what was
[66:37] blue.
[66:39] Music playing
[66:41] So we can do this again.
[66:43] Color selection.
[66:45] Hit the yellow part.
[66:47] Music playing
[66:49] And make this yellow.
[66:51] Music playing
[66:53] So you can see this is a very nice way
[66:55] to get masks that work
[66:57] with your high poly
[66:59] without needing to paint the mask manually.
[67:01] This is very fast.
[67:03] Music playing
[67:05] You will use ID maps
[67:07] for any asset that you will texture.
[67:09] Music playing
[67:11] And let's do the last one for the stitches.
[67:13] Music playing
[67:15] Music playing
[67:17] Music playing
[67:19] So whenever you do
[67:21] ID maps we have a few
[67:23] settings that we can mess around with.
[67:25] Music playing
[67:27] So let's say I want
[67:29] a certain material
[67:31] or more than just one color
[67:33] we can do pick color again
[67:35] and we can choose a second color.
[67:37] We are not limited to just one color.
[67:39] Music playing
[67:41] We can go ahead and adjust
[67:43] the hardness
[67:45] and the tolerance.
[67:47] Music playing
[67:49] These settings are more useful.
[67:51] For example when you have two colors
[67:53] in your ID map that are very similar
[67:55] to each other.
[67:57] Music playing
[67:59] Here we can say how, for example
[68:01] if we have this
[68:03] green, if we had
[68:05] another color that was similar to the green
[68:07] if we up the tolerance
[68:09] it would pick up on that
[68:11] similar green.
[68:13] Music playing
[68:15] Now don't worry too much about it as we have a very
[68:17] simple ID map.
[68:19] Music playing
[68:21] We can also use ID maps
[68:23] in a different way.
[68:25] Music playing
[68:27] Let's say we have a white mask
[68:29] everything is blue.
[68:31] Music playing
[68:33] And then I want to have the stitches
[68:35] out of this.
[68:37] So what we can do is we can add
[68:39] color selection.
[68:41] Music playing
[68:43] Then we say background is white.
[68:45] Music playing
[68:47] And then we have
[68:49] an output value that is black.
[68:51] Music playing
[68:53] Now if we pick a color
[68:55] anything that we pick will be filled
[68:57] with black.
[68:59] Music playing
[69:01] Music playing
[69:03] Music playing
[69:05] If you don't get it completely
[69:07] don't worry in the next video
[69:09] we are going to start blocking out our materials.
[69:11] Music playing
[69:13] And we are going to be using this a lot
[69:15] and it should become even more clear.
[69:17] Music playing


### Blocking Out Materials [69:18]
**Transcript (timestamped):**
[69:19] So let's get started
[69:21] with our actual texturing.
[69:23] Music playing
[69:25] So whenever I am starting my textures
[69:27] I like to block out the materials
[69:29] and the masks.
[69:31] Music playing
[69:33] The first thing that I am going to be looking at
[69:35] is what materials do we have.
[69:37] Music playing
[69:39] So over here we are going to have two materials.
[69:41] A leather material for the belt
[69:43] and then a metal material
[69:45] for the buckle.
[69:47] Music playing
[69:49] We are going to create a fill layer
[69:51] and let's call this ladders.
[69:53] Music playing
[69:55] Actually let's call this
[69:57] leather
[69:59] and we are going to group that
[70:01] and let's call this leather as well.
[70:03] Music playing
[70:05] Then we are going to duplicate this
[70:07] Ctrl D to duplicate
[70:09] Music playing
[70:11] Or you can do Ctrl C and Ctrl V
[70:13] or go here
[70:15] and duplicate layers.
[70:17] Music playing
[70:19] Let's call this one metal.
[70:21] Music playing
[70:23] Let's actually go
[70:25] leather base
[70:27] values.
[70:29] Music playing
[70:31] This one we are going to be changing to
[70:33] metal base
[70:35] values.
[70:37] Music playing
[70:39] Now for our leather let's set up some
[70:41] quick base values.
[70:43] Music playing
[70:45] So we are going to go with a brown belt
[70:47] so we are going to make this brown.
[70:49] Also let's hide the metal on top.
[70:51] Music playing
[70:53] Let's make a nice shiny leather.
[70:55] Metal should be at black
[70:57] because it's a non-metalic
[70:59] surface
[71:01] and then the normal we can ignore.
[71:03] Music playing
[71:05] Let's do the same for the metal.
[71:07] This should be at one or white
[71:09] because it's metal.
[71:11] Let's make this
[71:13] a little
[71:15] less shiny.
[71:17] Then we are going to be using
[71:19] a nice bright white color.
[71:21] Music playing
[71:23] Music playing
[71:25] Now we have our
[71:27] values blocked out.
[71:29] Let's go ahead and do the masks.
[71:31] Music playing
[71:33] So there's two ways of doing this.
[71:35] We can either right click add mask with color selection
[71:37] pick color and pick
[71:39] the red color.
[71:41] Music playing
[71:43] But my preferred way is when we have
[71:45] a whole object
[71:47] that will just be a single mask.
[71:49] Music playing
[71:51] Let's add black mask.
[71:53] We can go to
[71:55] Polygon fill
[71:57] and set the mode to
[71:59] Mesh fill.
[72:01] Use a value of one which is pure white.
[72:03] Then we just click the whole
[72:05] mesh.
[72:07] I'm going to repeat that for this.
[72:09] Music playing
[72:11] Now for the leather we cannot do the same.
[72:13] Music playing
[72:15] Actually we can for the first
[72:17] part of the leather.
[72:19] Music playing
[72:21] Let's do that.
[72:23] Let's say add black mask.
[72:25] Music playing
[72:27] Then we go to Polygon fill.
[72:29] Music playing
[72:31] We're going to click that one.
[72:33] Music playing
[72:35] If we alt click it we can check if the mask is correct
[72:37] and that looks fine.
[72:39] Music playing
[72:41] So now let's make this a little bit more complicated.
[72:43] Music playing
[72:45] Let the base value so we're going to say control G group it.
[72:47] Music playing
[72:49] Then control D.
[72:51] Music playing
[72:53] Let's call this bottom.
[72:55] Music playing
[72:57] Move the smile up and actually let's call this top layer.
[72:59] Music playing
[73:01] Let's hide the top layer for now
[73:03] and worry about the bottom.
[73:05] Music playing
[73:07] So leather is not just shiny.
[73:09] Music playing
[73:11] Leather exists mostly of two layers.
[73:13] Music playing
[73:15] So leather is a very rough layer.
[73:17] Music playing
[73:19] And on top of that is going to be a thin shiny leather
[73:21] as you can see in our model.
[73:23] Music playing
[73:25] So for the bottom let's make this very rough.
[73:27] Music playing
[73:29] This is almost pure white value.
[73:31] Music playing
[73:33] And for the top let's make this very shiny.
[73:35] Music playing
[73:37] Now we need to go to the top layer.
[73:39] Music playing
[73:41] I'm going to say add mask with color selection.
[73:43] Music playing
[73:45] Now we're going to be using our ID map.
[73:47] Music playing
[73:49] Now we're going to be clicking the blue.
[73:51] Music playing
[73:53] So now you can see that we have one part being shiny
[73:55] and the other part being rough.
[73:57] Music playing
[73:59] To make that even more clear we can change the value to pink.
[74:01] Music playing
[74:03] Just to showcase that.
[74:05] Music playing
[74:07] One problem this is also
[74:09] adjusting the stitches.
[74:11] Music playing
[74:13] We want a different value for the stitches as well.
[74:15] Music playing
[74:17] So we can do another hill.
[74:19] Music playing
[74:21] Let's group that.
[74:23] Music playing
[74:25] Let's go ahead and add mask with color selection.
[74:27] Music playing
[74:29] I select our stitches.
[74:31] Music playing
[74:33] You can pick that eye color here.
[74:35] Music playing
[74:37] And if we hold down shift you can click
[74:39] a color from the base color.
[74:41] Music playing
[74:43] If we don't it will have the color of the reflections
[74:45] and that's a hold down shift and click it.
[74:47] Music playing
[74:49] Now we're just going to bump up the value
[74:51] and saturation up a little bit.
[74:53] Music playing
[74:55] Maybe a little bit less.
[74:57] Music playing
[74:59] Something like this.
[75:01] Music playing
[75:03] Let's make the stitches very rough as well.
[75:05] Music playing
[75:07] And now we've blocked out our materials really quick.
[75:09] Music playing
[75:11] You should be aiming
[75:13] to get a quick representation
[75:15] of what your final textures
[75:17] is going to look like.
[75:19] Music playing
[75:21] Let's see it as a quick block out.
[75:23] One of the most important parts
[75:25] is that we now have all the masks
[75:27] set up already.
[75:29] We just need to replace the folders.
[75:31] Music playing
[75:33] The content of them.


### The Power Of Effects [75:35]
**Transcript (timestamped):**
[75:35] Music playing
[75:37] So before we get to creating
[75:39] our nice first
[75:41] smart material by ourself
[75:43] out of layers.
[75:45] I want to showcase you once again
[75:47] the power of effects.
[75:49] Music playing
[75:51] This is because we're going to be using that a lot
[75:53] to create our smart material.
[75:55] Music playing
[75:57] For example here we have our stitches
[75:59] and we want them to be a little bit brighter
[76:01] and
[76:03] the colors are the stand out from the rest.
[76:05] Music playing
[76:07] So what we did is we added a fill layer.
[76:09] Music playing
[76:11] But this is a pretty destructive workflow.
[76:13] Music playing
[76:15] Let's say hey I don't want the leather to be brown.
[76:17] Music playing
[76:19] Actually I want like a blueish leather.
[76:21] Music playing
[76:23] Now if we make like a blueish leather.
[76:25] Music playing
[76:27] Music playing
[76:29] You will see that the stitches don't make sense
[76:31] anymore.
[76:33] Music playing
[76:35] So something that we can do instead.
[76:37] Music playing
[76:39] Let's go ahead and just
[76:41] Music playing
[76:43] Go to filters
[76:45] Music playing
[76:47] HSL
[76:49] Let's go ahead and drag that
[76:51] In here.
[76:53] Music playing
[76:55] I'm going to be calling this stitches.
[76:57] Music playing
[76:59] And we say
[77:01] Music playing
[77:03] You can find it. We say copy mask.
[77:05] Music playing
[77:07] Copy mask or control alt C.
[77:09] Music playing
[77:11] On this layer we are going to say paste mask
[77:13] Music playing
[77:15] Or control alt V.
[77:17] Music playing
[77:19] So again we get used to using the shortcuts.
[77:21] Music playing
[77:23] Now we can delete the stitches
[77:25] Folding as we don't need it anymore.
[77:27] Music playing
[77:29] So now instead of thinking of
[77:31] Colors and whatever
[77:33] We are thinking in values.
[77:35] Music playing
[77:37] So if we go here to the HSL
[77:39] You can see the color.
[77:41] Music playing
[77:43] We don't want like a light brown color.
[77:45] We want the color that's lighter.
[77:47] Music playing
[77:49] So let's go ahead and just bump up the lightness.
[77:51] Music playing
[77:53] Maybe a little bit lighter and
[77:55] A little bit more saturated.
[77:57] Music playing
[77:59] So now let's say if we made a blueish
[78:01] Leather
[78:03] Music playing
[78:05] You will see that the stitches
[78:07] Automatically stay true to that color.
[78:09] Music playing
[78:11] Because all they were saying is ok.
[78:13] We have stitches and we want them
[78:15] To be a little bit lighter.
[78:17] Music playing
[78:19] So this is a way that you become a little bit less destructive
[78:21] In your text string and will be easier
[78:23] To update your material.
[78:25] Music playing
[78:27] One thing that we can do is we can add filters
[78:29] To filter layers.
[78:31] Music playing
[78:33] So this is just a normal layer
[78:35] Which holds a filter.
[78:37] Music playing
[78:39] As you can see we have layer
[78:41] And holds a filter.
[78:43] Music playing
[78:45] So what we can do is we can go
[78:47] On the magic wand icon
[78:49] At filter.
[78:51] Now this is a filter that is empty.
[78:53] Music playing
[78:55] Actually it wasn't the wrong one.
[78:57] Music playing
[78:59] So add a filter.
[79:01] Music playing
[79:03] Now we have an empty filter.
[79:05] Music playing
[79:07] Now we can look on our filters.
[79:09] Music playing
[79:11] We can search for our filter and we are going to go to
[79:13] Contrast.
[79:15] Music playing
[79:17] So I am going to drag that one in the filter slot.
[79:19] Music playing
[79:21] You can look for it over here.
[79:23] Music playing
[79:25] Again we want this to be just in one channel.
[79:27] Music playing
[79:29] So we are going to alt click that channel.
[79:31] Music playing
[79:33] And we want the roughness.
[79:35] Music playing
[79:37] So alt click the roughness.
[79:39] Music playing
[79:41] Make sure this is going to be all the way to white.
[79:43] Music playing
[79:45] To get very rough stitches.
[79:47] Music playing
[79:49] So we are just doing anything because
[79:51] The first layer is already white.
[79:53] Music playing
[79:55] Let's say if we adjust this
[79:57] Music playing
[79:59] We will make this a little bit more shiny.
[80:01] Music playing
[80:03] You will see that the stitches will always stay
[80:05] Music playing
[80:07] Keep it rough.
[80:09] Music playing
[80:11] And let's go with that.
[80:13] Music playing
[80:15] In a non destructive way.
[80:17] Music playing
[80:19] And generally speaking it is also going to be faster
[80:21] Music playing
[80:23] to build up your materials.


### Adding Variation [80:24]
**Transcript (timestamped):**
[80:25] Music playing
[80:27] So let's take a look at how we can actually create
[80:29] Music playing
[80:31] a nice looking smart material from stretch
[80:33] Music playing
[80:35] And to do that I am going to be focusing
[80:37] Music playing
[80:39] on our top layer.
[80:41] Music playing
[80:43] So we are going to add some values
[80:45] And we are going to say control G
[80:47] To group it.
[80:49] Music playing
[80:51] Let's call this base values.
[80:53] Music playing
[80:55] Now we want to have a little bit of
[80:57] Music playing
[80:59] variation in the color.
[81:01] Music playing
[81:03] Again I am hitting the C key
[81:05] Music playing
[81:07] To swap between the channels.
[81:09] Music playing
[81:11] So what we could do is add the fill layer
[81:13] Music playing
[81:15] And hide this.
[81:17] Music playing
[81:19] And make it a little bit lighter.
[81:21] Music playing
[81:23] And then add a mask with variation.
[81:25] Music playing
[81:27] But again this is a very annoying thing to do.
[81:29] Music playing
[81:31] And very destructive if we change the base color.
[81:33] Music playing
[81:35] So like I showcased you earlier.
[81:37] Music playing
[81:39] We want this value to be a little bit
[81:41] Music playing
[81:43] Lighter.
[81:45] Music playing
[81:47] Then we call this lighten.
[81:49] Music playing
[81:51] Then we are going to add a new filter.
[81:53] Music playing
[81:55] We are going to use a contrast
[81:57] Music playing
[81:59] Illuminance.
[82:01] Music playing
[82:03] We are going to lighten up the roughness as well.
[82:05] Music playing
[82:07] Actually keep this a base color.
[82:09] Music playing
[82:11] You can see that we can lighten that up.
[82:13] Music playing
[82:15] Which means it becomes more rough.
[82:17] Music playing
[82:19] And switch back to M from material.
[82:21] Music playing
[82:23] So that is great. Now we have something that lightens our material up.
[82:25] Music playing
[82:27] But we need to work on the variation.
[82:29] Music playing
[82:31] We need a mask. We need right click.
[82:33] Music playing
[82:35] Then over here we can add a fill to that mask.
[82:37] Music playing
[82:39] Which now means that we can fill it with anything that we want.
[82:41] Music playing
[82:43] The default is going to be a slide
[82:45] Music playing
[82:47] From 1 to 0.
[82:49] Music playing
[82:51] If it is 0 it is filled with black. So you will see nothing.
[82:53] Music playing
[82:55] One is pure white so you will see everything.
[82:57] Music playing
[82:59] But what we want to do instead of using a slide.
[83:01] Music playing
[83:03] We want to go ahead and start the assets.
[83:05] Music playing
[83:07] Play the search as well.
[83:09] Music playing
[83:11] We are going to go to procedural.
[83:13] Music playing
[83:15] Let's go to grunches for example.
[83:17] Music playing
[83:19] We can go to noises or whatever.
[83:21] Music playing
[83:23] Let's work with a noise for now.
[83:25] Music playing
[83:27] These are going to be tileable images.
[83:29] Music playing
[83:31] Without a visible scene.
[83:33] Music playing
[83:35] For example we can say clouds 3
[83:37] Music playing
[83:39] We drag that in here.
[83:41] Yes we alt click the mask.
[83:43] Music playing
[83:45] We can see what we are working with.
[83:47] Music playing
[83:49] Let's go ahead and change the UV projection to try a planar projection.
[83:51] Music playing
[83:53] This is going to help by blending in the scenes.
[83:55] Music playing
[83:57] So for example on UV projection.
[83:59] If we have a seam in the UVs, you can clearly see it.
[84:04] We put it to Tri-Plane, you're not going to be able to see the seams as much.
[84:11] Go ahead and put the Tiling up, which means we're scaling our map down.
[84:22] We can adjust the balance and the contrast to play with it until you get a value that you like.
[84:30] Now if we hit C to go to Color again, you can see that we have now a nice broken-up surface.
[84:37] We got some light and some darks. I think the contrast could be a bit more, so I'm going to
[84:43] up that a bit. That's looking good. One problem, this is a very obviously repeating pattern.
[84:53] We can fix that by adding a new Hill.
[84:59] Then we're going to choose a new map. This time let's go ahead and use a Crunch.
[85:06] These are going to be a little bit more dirty looking. Let's go with this one for example.
[85:12] I'm going to put this to Tri-Plane again, adjust the Tiling.
[85:22] Let's go ahead and rotate this a little bit so it follows the mesh a bit better.
[85:30] Then now we're going to put this to Multiply. What this is going to do
[85:36] is going to go ahead and if you take a look at this black
[85:46] it's going to apply all those blacks on top of what we had. That's going to break up the
[85:54] Tiling of that first map really nice. Go ahead and go with a less big Tile.
[86:02] We're trying to break that up. Usually it's enough with just having one breakup, but you can go
[86:10] as many as you want. You can add five on top of each other and
[86:16] if you like the result it's all nice. For now let's keep it simple and just have one
[86:21] multiply on top of this.
[86:28] So now what we're going to do is we're going to go ahead and duplicate this.
[86:33] Let's change the name and we're going to call this Darken.
[86:41] I'm going to hide the Lighten. This one's going to be used to darken the values.
[86:46] So to put this down, usually I up Saturation as well when I darken Stuff.
[86:53] Just so we get a nice colorful effect. Let's go ahead and change up these maps.
[87:03] So I'm just going to hide that breakup on top of it. Now, Clouds 3 we can go ahead and
[87:11] choose a different map. You can just drag maps on and see which ones you like and which ones you
[87:17] don't like. I think this one looks pretty interesting right from the start. So that's nice.
[87:25] Let's mess with the size. I think something like that is pretty cool. I'm going to be messing with
[87:33] the balance and the contrast until we get something that we like. I think something like that is nice.
[87:41] Now again let's add some breakup on that. Go with a different map.
[87:53] And we can also mess with different blending modes. Maybe instead of taking away we want to add stuff.
[88:00] The easiest way to mess with this is you just alt click it so you can see a mask.
[88:07] You just click normal for example. Then we can hit arrow key down.
[88:13] Hit normal and then arrow key down. That way we can go through the blending modes.
[88:20] We can look for one that's interesting to us.
[88:23] Just trying to look for my effect that looks interesting. I think like this it looks pretty
[88:30] interesting. Then we can also still tone this down. We do the opacity lower or higher. Let's go with
[88:40] like 70. And then on top of that we can add levels. We can adjust the levels of this mask.
[88:53] Which basically means that we can push the whites and the blacks closer to each other
[88:59] or further away to have more contrast. So we start off with a pretty simple looking mask.
[89:08] Then we can make it a little bit more interesting.
[89:17] Now looking at the material I think we should have more dark values. We're going to up the balance
[89:25] all the way. Let's mess with the contrast. We're going to do the same here. Mess with those values.
[89:33] Also if this is really slow for you again you can just
[89:38] put the stick to K and it will be way faster. Don't worry you're still texturing at 4K.
[89:44] And later when we export we can just put it back at 4K.
[89:53] So I think I like something like this. Now let's go ahead and enable our lighten.
[89:59] Let's put the lighten on top of the darken. See how that looks. I think that looks a little bit nicer.
[90:06] I think our darken is very strong.
[90:11] Also let's go ahead and adjust our contrast luminous. So our roughness make that darker as well.
[90:21] Let's tone down the darkness a little bit.
[90:24] And we can change it.
[90:28] Something like this. So I think now looking to this overall. I think it's a little bit too shiny.
[90:38] We can go back to our base value. Now we can decrease the roughness.
[90:45] And since we have everything set up with filters you will see if we change that base everything is
[90:52] going to be updated because we're working with a non-destructive workflow.
[91:07] I want to have a little bit more variation in the roughness. So we can go to lighten.
[91:14] Let's go ahead and up the value here so we have some more contrast.
[91:20] A little bit too much. And something like that is looking pretty nice.
[91:30] I'm going to do one more. Let's duplicate the lighten. Let's call this saturation.
[91:36] This one that I usually like to add. With this one I'm looking for something very subtle. So I'm
[91:45] going to delete that breakup. I'm going to be using crunches splash the dusty. Just something very
[91:53] simple with not too much going on.
[91:55] I want to keep this very subtle. Just going to be upping. Also let's get rid of the contrast
[92:08] on that one. We don't need to break up in the roughness for this in my opinion.
[92:15] And let's go ahead and up the saturation on that.
[92:20] Make the lightness as well a little bit.
[92:27] Not entirely convinced on that. So let's mess with the size.
[92:34] Something like that.
[92:41] I think we have a little bit too much. So actually let's bring back a fill.
[92:46] Put it to multiply. Let's take away a little bit. Let me use a clouds tree.
[92:54] Put it to try playing a projection. I'll click the mask. See what we're doing.
[93:01] Up the contrast and adjust the size.
[93:05] So now if we put the balance up we're going to have more saturated spots. If we put it down we're
[93:16] going to have less. Let's go with something like this.
[93:27] Now we're just adding some very subtle looking details.
[93:31] Which is nice.
[93:40] Let's go ahead and take our saturation light and darken.
[93:44] Select them all. Control G. We're going to call this
[93:51] break up. Because it's breaking up our base values.
[93:55] One thing that you might notice is that everything seemed to have disappeared once we did that.
[94:03] That's because when we have filters in a group we need to go ahead and go to the blending mode and
[94:10] set this to pass through. Now you will see that we have it back. One thing we have a filter for
[94:17] the base color channel and for the roughness. If we go roughness you will see that we have nothing.
[94:24] That's because we need to go to the roughness. Now for here you will see it's set to normal and we
[94:30] need that it to pass through. By the way of doing it is let's go back to normal and to base color.
[94:39] We can just right click and pass through and say apply to all channels.
[94:45] Now we have all our break up in its own little break up layer.
[94:50] One thing I want to have some big break up in the roughness. This is what I always like to have on top.
[95:01] So I'll go to my filters. Go to contrast and luminance. Also I'm using the contrast and
[95:12] luminance filter just for the roughness. Just to have a little bit more clarity of okay when we
[95:19] have a HSL it means that it's for the color. If we have a contrast luminance it's going to be for the roughness.
[95:29] Let's go ahead and put the roughness more black on this one. I'm going to add black mask
[95:37] fill. Let's go ahead and add a grunge to this.
[95:53] I think this one could be interesting. I could alt click the mask see what's going on. Try planar.
[96:01] Let's put the balance down. So for this I just want some big spots with different values.
[96:12] Go ahead and put some offset on it to change where the white spots are. Maybe something like that.
[96:22] Go ahead and click see again. See to see the roughness and see how that is looking.
[96:36] And I think like this we have some interesting variation in roughness.
[96:41] So let's call this big breakup. Let's also go ahead and try to see how it looks if we add a HSL to this for the color.
[97:01] I think that looks pretty cool actually. So let's keep it.
[97:11] So let's go ahead and add a little bit of the roughness.
[97:21] That's going to make it look quite nice and interesting.
[97:26] So let's recap a little bit by adding variation to our values. We can make a material look more
[97:34] realistic and interesting. If everything is a single value it's going to look fake and
[97:42] interesting and detailed and everything. By adding some quick variations with masks we can go ahead
[97:50] and create interesting looking materials. You can see the more variation the more breakup we add
[97:58] the better it starts to look.
[98:04] It's also important that you have smaller breakups and bigger breakups. Think about the primary,
[98:12] secondary, tri-tary structure which in short words is we need to have small structures.
[98:21] We need to have bigger structures and we need to have really big structures.
[98:28] So right now our big breakup would be our primary breakup. Then our secondary breakup would be the
[98:37] light and darken. Then our tri-tary breakup would be our small saturated spots that we've put in.
[98:46] So by reinforcing this structure of primary, secondary, tri-tary we can ensure that we have
[98:54] interesting looking breakup. So now that we finished our base values we need to add some


### Adding Details [98:58]
**Transcript (timestamped):**
[99:04] actual details in the normal map. And to do this we're going to create a new layer. We're going to
[99:12] be creating a fill layer. Let's go ahead and call this details. So over here we want to have some
[99:21] details for our material. Since we have a leather material let's go ahead and add some leather
[99:28] details. The one add a black mask then we're going to add a fill. Now over here we can just look in
[99:36] texture for leather. Now you can either use a tiling leather map that you downloaded online
[99:47] from somewhere or you can use the default one in Painter. For now we're just going to be using
[99:54] the default one in Painter. So if we alt-click this map you can see our leather. This one I don't want
[100:05] to set to Tri-Plane on projection because I want the details to follow the direction that I've
[100:12] set in the UVs. Now let's go ahead and adjust the tiling of it so we can get the smaller details of
[100:24] the leather or we can get bigger details of the leather. So a good rule is to go a little bit
[100:35] bigger than you'd have in real life. The sample in real life would be more like 2.8 maybe. That is
[100:46] very small looking detailed leather but this is not going to read well once we zoom out.
[100:55] Usually when you do stuff for games you want to over exaggerate the size of things a little bit
[101:01] so they read better from a distance. So maybe we can go with 1.8 instead. Let's alt-click this
[101:11] and if we take a look at this everything that's going to be white is going to be shown everything
[101:18] that's going to be black is going to be invisible. I think in our case it would be easier if this
[101:26] map was inverted in color so we can go ahead and do levels. Now we can say invert.
[101:33] Now you can see we just have some leather crack details showing through.
[101:43] So what we can do now is we're going to alt-click
[101:47] height because we only want to put some height for now. Again just like with the channels
[101:53] we will just have it in height channel now. Now we're going to add a little bit of height.
[101:58] This should be going in. Also it's a little noisy this map. What we can try to do is we can add a filter
[102:07] and blur. This is going to blur out our mask a bit. Let's keep this at a very subtle value of
[102:17] maybe point 1. That looks still a little bit too much 0.7, 6. Just want to see how low I can go
[102:30] until it becomes noisy again. So I think like 6 is a good value.
[102:38] This is just going to make it look a little bit softer and less noisy. Right now we just have
[102:47] noise. Now we're actually getting some details. I think we can also bump this up to maybe point
[102:57] 9. We get it looking nice and soft. Let's also go ahead and try the other leather.
[103:10] Just going to clear this and look for the leather.
[103:16] Let's see how this looks if we put this one in here.
[103:20] I do think I prefer the first one so let's undo that. Maybe let's go with 1.4 instead.
[103:30] So it becomes a little bit more readable. Maybe 1.3.
[103:43] Clicking mess as long as we want with the size. I think I'm going to go with 1.1 so it's nice
[103:49] and readable. Let's go ahead and get a little bit more depth maybe.
[104:00] Just like this. Now we have some details in the height which is going to make it look
[104:07] more detailed in the normal plus height mesh. You can see we have those details going through.
[104:14] But we also want this to be in the color. What we can do is we can add a fill.
[104:26] Actually we can add a filter. Excuse me. The filter.
[104:34] We're going to add a HSL.
[104:36] Then we're going to go ahead and put the lightness up or down. You will see nothing happens.
[104:45] Because right now we have our blending mode set to normal. Let's change this to pass through.
[104:52] Now you will see it will start to do things.
[104:56] Bump up the saturation. It's not just becoming white.
[105:02] And look for something that looks nice and natural.
[105:08] And again because we're doing this with filters we were to change our very first base value to
[105:14] like a green. You will see that now we have a perfectly looking nice green leather.
[105:20] Let's go back to our details. We're going to add one more filter. Also right click the pass
[105:32] through. Apply to all channels. Actually let's undo that. I don't want it in the height so control
[105:39] C. Let's go to height and roughness. I'm going to put this to pass through. Now if we go to the
[105:47] roughness channel. Go ahead and fill this with a contrast luminance filter. We're going to make this
[105:57] very rough. So now this looks all messed up because we forgot to alt click the roughness.
[106:11] Now you can see we have some leather details.
[106:17] This is looking very strong the details. So let's go ahead and adjust it a little bit. I think we can
[106:24] turn down the color a little bit more. Something like this. Let's mess with the height.
[106:33] Do something like this. Now that's starting to look a lot better.
[106:51] Now I want to add a little bit of a breakup in our details. If we alt click this
[106:58] we can go ahead and add a fill. Go ahead and clear the search. Just like before we can add
[107:09] something here. Let's go with that clouds. Clouds too. Try playing up the projection so we don't
[107:17] have the scenes popping through. We're just tiling a little bit. Up the contrast and the balance
[107:25] down a bit. Let's set this through multiply. So now wherever we have that dark value the effect
[107:36] is going to be less strong of the details. Up the tiling. Just the balance.
[107:46] Just something like this.
[107:55] I think we're taking away too much detail. We can just go ahead and adjust the opacity of this.
[108:03] If we turn it down we get everything back. Let's just start turning it up until it's nice and
[108:10] subtle. The variation. That's looking pretty nice. Do you think that perhaps we can make a little bit
[108:22] more light details? Saturation a bit.
[108:28] Maybe something like that.
[108:42] I can see this starting to look like a pretty natural worn out looking leather.
[108:50] And that should do it for our details.
[108:52] Right now we have base values and then we have details.


### Adjusting Our Material [109:03]
**Transcript (timestamped):**
[109:04] Now there's going to be one more layer to create a mark material which is going to be
[109:12] adjustments. So we have base values. We can right click this. Give this a color.
[109:19] It's the same for the details. Then we're going to have one more holder with some adjustments.
[109:30] The adjustments are meant to quickly change the look of our material.
[109:36] Let's say we want to adjust the color a little bit. We can say color balance or color correct.
[109:42] It's a little bit nicer. Put this on top. Let's group this. Let's call this adjustments.
[109:51] Give this a blue color. Let's put this to pass through. Apply to all channels.
[110:01] So now we can start to color correct this a little bit. You can say let's up the contrast.
[110:07] Maybe up the luminosity a little bit. Maybe down the saturation.
[110:15] Mass with the midtones.
[110:21] Now we can very quickly get a totally different feeling leather.
[110:27] So I do like how that looks. Maybe it's a little bit too strong on the pack.
[110:38] So we go to base color. Now we can change the opacity of that in the base color channel.
[110:45] We can do this to something like 79 perhaps.
[110:56] We can do the same for the roughness. So let's call this color.
[111:05] We're also going to do a color correct. Let's call this roughness.
[111:09] Go to the roughness channel.
[111:17] Alt click rough. Now we can start messing with the values.
[111:39] So let's go to the roughness channel.
[111:51] Good M to check the material.
[112:00] I think it's a little bit too shiny but I like the new contrast that we have in it.
[112:05] Values. We're gonna go ahead and tone that roughness down a little bit.
[112:14] Now I think we have a very nice looking leather.
[112:22] I'm gonna add one more breakup for the color.
[112:27] Do a color balance this time. I'm gonna put that on top of the color just to keep the color
[112:34] all together. Let's call this color too.
[112:42] Maybe we can mess a little bit with colors here.
[112:55] This one doesn't seem to be doing a whole lot until we get to the shadows.
[113:04] We could make it a little bit more saturated perhaps.
[113:34] Then I do want to mess a little bit more with this.
[113:39] Maybe you can add a level to this.
[113:42] I'll take the channel base color and let's push these values around a little bit until
[113:48] we get something that looks cool.
[113:57] Go with something very extreme for now.
[114:04] Then maybe we can tone this down and see how that starts to look.
[114:09] Very subtle, I think that's nice.
[114:13] But now we want to add a little bit of variation.
[114:15] So we can add a black mask, a fill.
[114:22] Now we can do a cloud, a tri-planar.
[114:28] Let's up the contrast and go with a very small balance.
[114:36] And up the tiling a little bit.
[114:39] Maybe a little bit down the contrast and balance.
[114:44] Now we're just going to get a few spots where the color gets a little bit more intense.
[114:51] So even when we're adjusting stuff, this is still an opportunity to add some more break-up
[114:57] and variation within our material.


### Refining Our Details [115:13]
**Transcript (timestamped):**
[115:15] Maybe we can go back to our details at this point.
[115:22] Mess a little bit more with the height and the size.
[115:27] I'm showing you that you can always jump around and mess with layers, which is very nice.
[115:33] We can keep on changing the look of our material.
[115:44] I think I'm pretty happy with the point we have.
[115:49] Maybe we can up the height a little bit and try to add a little bit more blur.
[116:10] Maybe mess a bit more with clouds at less contrast and a lower balance.
[116:35] So I feel like our roughness isn't really popping through in the details.
[116:42] We can try to add levels.
[116:45] This too.
[116:48] Roughness.
[116:49] I'm going to push that out and in a little bit.
[116:54] If that helps.
[117:00] Which definitely doesn't.
[117:05] Let's go ahead and delete that.
[117:08] We're just going to duplicate that layer.
[117:11] I'm going to go ahead and actually let's just delete that instead of duplicating it.
[117:18] Let's make a fill layer.
[117:25] Actually not the best idea.
[117:29] Go ahead and delete that.
[117:31] I'm going to duplicate the details.
[117:33] I'm going to get rid of the HSL.
[117:36] Get rid of the height.
[117:38] We just have the roughness in here.
[117:48] Actually let's talk about a new concept right now.
[117:52] Anchor points.
[117:53] We're not going to get very much in depth about this.
[117:55] We're going to get more in depth in a later video in the course about anchor points.
[118:01] Now we can just delete all this.
[118:08] Now on top of our mask.
[118:10] You can add an anchor point.
[118:13] Now with any layer above this anchor point we can reference it.
[118:17] We can say fill anchor points and we have details mask.
[118:23] That's just going to place our mask in there.
[118:25] Then if we make any adjustments to it it will update over here.
[118:31] So we can call this roughness plus.
[118:36] Let's call this details roughness plus.
[118:42] Let's keep this roughness plus and we're just going to take the details and group it all
[118:46] together.
[118:47] Pass through.
[118:48] Apply to all channels.
[118:52] Actually undo.
[118:53] We don't want it in the height.
[118:56] Let's go roughness and pass through.
[119:02] Now in our roughness.
[119:05] Now that we've referenced the anchor point we can add levels.
[119:11] Who can adjust these values.
[119:15] Now we can try to get a little bit more white.
[119:18] Which is going to result in having more of that roughness in here.
[119:27] This definitely too much.
[119:28] Let's tone it down a bit.
[119:32] Now our details are popping through nicely in the roughness.
[119:43] Let's tone it to look a lot nicer.


### Saving A Smart Material [119:51]
**Transcript (timestamped):**
[119:52] Now let's talk about something very powerful of smart materials.
[119:57] This all that we just did was create our very own smart material.
[120:02] Let's name this details.
[120:14] So at any time that we want to use this smart material.
[120:19] Just like we have all these we can save it.
[120:23] All that we have to do is we're going to group this together.
[120:30] Let's call this letter.
[120:36] I'm going to call this underscore trigon.
[120:45] Now right click.
[120:47] We say create smart material.
[120:52] Just like that.
[120:53] Now over here we have our letter trigon smart material.
[120:59] The reason why I grouped it together and not just used the top layer.
[121:04] That's because you cannot have a mask when you create the smart material.
[121:08] If you do it you will get a very weird thumbnail.
[121:18] So the name of your smart material is going to be what you put in the painting when you
[121:25] created it.
[121:26] So you want to think about this a little bit.
[121:29] Like I could have called this a letter and just create a smart material.
[121:34] But let's say if we say letter we already have a lot of letters.
[121:39] So it's going to be difficult to find your own smart materials.
[121:45] Eventually once you've built up a good library of smart materials you're not really going
[121:51] to be using the default ones that come with Painter anymore.
[121:56] Because generally speaking your own ones are going to be looking a little bit nice.
[122:03] Now let's say I'm in a production environment.
[122:07] I'm starting a new asset but I've already like texted and let it like 20 times.
[122:13] I have a bunch of letter smart materials that I've created before.
[122:19] So let's say I'm starting the project and I need a letter.
[122:23] Now if we look for letter it's going to show all these letters.
[122:27] But if we go letter, try again.
[122:32] It will only show my own materials.
[122:34] So let's say if you're working in a studio environment it can be a good idea that you
[122:39] do letter underscore your name or whoever and then you can look through the materials
[122:45] by name of the artist.
[122:49] Or we can say trygon.
[122:53] Now it's going to show all my materials because they're all underscore trygon.
[122:58] So if I had more it would show my metals, my plastics and everything.
[123:05] And again if I want a specific one I could go like letter underscore trygon and it will
[123:10] show my letters.
[123:12] So that's why it's important to keep a nice name on your smart materials because you want
[123:19] to be thinking about how you're going to be looking for them in the future.


### Adjusting Our Smart Material [123:23]
**Transcript (timestamped):**
[123:25] So let's talk a little bit about how we can actually use our smart materials.
[123:29] I'm going to delete the work that we've done.
[123:35] Let's go back a little bit.
[123:36] Let's say letter base value is duplicates and put this in the top layer.
[123:41] Again, right now we're back at our blockout that we had before.
[123:47] We just have our colors quickly blocked out and our masks.
[123:52] This is what I would do in a production environment.
[123:55] I quickly get a blockout of everything and instead of creating a smart material I will
[124:02] already have all the smart materials created, but at least the vast majority.
[124:08] So then I would just go to my stuff.
[124:12] I need a letter.
[124:13] I go letter trygon.
[124:17] Look for my letters and decide on a letter that I like.
[124:21] Then I would just drop and drag and drop it.
[124:25] Then we can take our letter base and just get rid of it and boom.
[124:30] Now we have textures.
[124:32] This one of the strengths of Substance Painter.
[124:36] It's so easy to do work and then reuse your own work or the work of other people, which
[124:43] is going to save you a tremendous amount of time.
[124:47] When you're just learning I do recommend to create a whole bunch of smart materials and
[124:52] learn from the process.
[124:55] Even if you have like five letters already, if you're learning it's always a good idea
[125:00] to just create new and new materials and learn every time you do it.
[125:09] So let's say again we're in a production environment and we have this letter, but in the concept
[125:14] the letter is black, but it's like very old and worn.
[125:18] So everything matches more or less except for the color.
[125:21] What we can do is we can go look for our smart materials all the way to the base and
[125:26] change that.
[125:28] Or we can just go on top on the adjustment.
[125:33] We go to filters.
[125:34] We put a HSL all the way on top.
[125:39] We say saturation, put it all the way down on lightness, put it down.
[125:44] And now we have a black letter.
[125:49] So you can see how fast and easy it is to adjust your work.
[125:57] Now let's go ahead and delete that as we're going to be sticking to a round letter.


### Reusing Our Smart Material [126:02]
**Transcript (timestamped):**
[126:04] So now let's take a practical look at how we can replace our blockout with smart material
[126:11] preset.
[126:12] So we're going to be using this as our preset, the letter one.
[126:26] Now if we go to bottom, we're going to track the letter dragon in bottom.
[126:34] Delete the letter base values.
[126:37] Also hide the top layer.
[126:41] I'm going to have a look at this and think, okay, this is not how we want it to look.
[126:49] We don't need to let us sell details.
[126:52] So we go details, details, and we go crunch, let the damage.
[126:57] We're going to replace that map, maybe with actually clouds.
[127:03] Could be fine for this.
[127:05] Put clouds in, change the styling, get rid of all this breakup.
[127:13] Also, we don't need to roughness plus on this one.
[127:17] Let's get rid of the anchor point.
[127:21] Let's keep the levels, and actually we can delete those.
[127:27] Let's go for like a noisy field of the contrast, the balance.
[127:37] Now we're getting a little bit of details on here.
[127:42] If this one, I want the height to be more extreme, maybe something like that.
[127:57] Let's try a different styling, maybe eight.
[128:09] Go ahead and change our base value, make it way more rough.
[128:20] Take a look at dark and light, and okay, let's get rid of the adjustments.
[128:26] We're going to simplify this one a little bit.
[128:30] Get rid of the big breakup, get rid of saturation.
[128:35] We're just going to keep the light and dark.
[128:39] This one, we can just be really lazy about it.
[128:44] Styling, let's leave the next one.
[128:53] Check the lighting, go ahead and adjust the tylings and those.
[129:01] Maybe up the rotation a little bit.
[129:05] Just like that, we have a rough looking base layer for our ladder.
[129:12] You can see within just a few minutes, I created a new material, which has a lot of detail and variation.
[129:24] Now we can go ahead and say ladder, let's call this ladder base, try it on.
[129:37] I'm going to go ahead and right click, create smart material.
[129:45] Now if we look for a ladder, let's go to a trigon.
[130:01] Let's not pop it up because we have the base afterwards.
[130:09] If we want to see all, we can go to a trigon.
[130:12] Now we can see we have a ladder trigon for the top and the base.
[130:19] Now let's get our top layer showing.
[130:23] I'm going to say top layer and show it.
[130:26] You're going to see that it's super noisy.
[130:29] That's the noise of the bottom layer is showing through.
[130:33] What we can do is we can go to height, I'm going to say replace.
[130:40] That's going to replace the height of the bottom layer.
[130:46] Just like that, now we have some ladder.
[130:51] I do think we might need a little bit of a bigger break up actually on the base.
[130:57] We can go back to break up.
[131:03] Go to filter, HSL.
[131:08] Make this one really dark and maybe saturated.
[131:17] Then add a black mask, fill and let's add a clouds.
[131:25] I want to make sure that this is nice and big for a big primary break up.
[131:40] See now we have some big primary break ups.
[131:42] It's probably a bit too much.
[131:49] Something like this.
[131:51] Maybe the tail in F2.
[131:54] Change the rotation, try to get spots in a more visible place of the camera.
[132:01] Let's go ahead and tone that down a little bit, the darken.
[132:06] Just like that.
[132:11] I think that looks a little bit nicer and more natural.
[132:20] Now we can do this again.
[132:24] Now the ladder is finished.
[132:27] Let's worry about the metal.
[132:29] Go to the dragon, make sure we're on smart materials.
[132:34] Now we can pick any that we'd like.
[132:37] Let's go with the base.
[132:39] Drag this here.
[132:42] Delete all block out.
[132:50] Make this metallic and let's make it nice and shiny.
[132:57] Now once you're working with something that you're going to change a lot.
[133:01] It's a good idea just to kind of go layer by layer.
[133:05] Let's go by base values, that is good.
[133:08] Let's go to break up.
[133:12] So I'm not liking that.
[133:14] Let's go darken.
[133:17] Let's take a look what we're doing over here.
[133:20] Start off with this one.
[133:25] Adjust the balance.
[133:28] Maybe something like that.
[133:35] Something like that.
[133:37] Take a look.
[133:44] I don't want so much break up in the color.
[133:47] I just want a lot of break up in the roughness.
[133:54] Same for lighten.
[133:56] I think that one's pretty nice already.
[133:58] All we have to do is go ahead and adjust the rotation.
[134:05] So it follows the buckle a little bit better.
[134:10] And again let's go ahead and make the contrast more intense.
[134:24] Maybe something like that.
[134:29] It's probably a little bit too much contrast.
[134:32] So let's tone that down.
[134:39] Let's add details.
[134:46] So over here let's go with just nice looking crunch.
[134:49] You can say crunch.
[134:52] Not sure we're not looking on just smart materials.
[134:56] Maybe crunched damas could be cool.
[135:04] It's probably not going to look as nice with the height that we have.
[135:09] Let's tone that way down.
[135:14] Maybe it's not the crunch that we should be using.
[135:20] Let's look for a metal one.
[135:26] Maybe this one.
[135:32] That's looking way way nice already.
[135:36] So you can see that we just need to experiment a little bit with different mattes and everything.
[135:56] I think this doesn't look pretty interesting.
[136:00] Then lastly I want to add a little filter on top of all this.
[136:09] Let's go filter.
[136:15] We can use a matte finish which is going to adjust the normals a little bit.
[136:20] Which is pretty nice when you're working with metals.
[136:23] I'm going to put this on top of the details.
[136:27] Let's look at the normal channel.
[136:30] You can see that it will add some stuff in there.
[136:34] We can adjust the intensity of that and the scale.
[136:44] That's going to make it look more worn out.
[136:49] I think we have a little bit too much break up now.
[136:52] It mostly comes from the details and the flakes I guess.
[136:57] Put the flakes down.
[136:59] Then the details.
[137:02] We can tone everything that we did down by adding a black mask.
[137:07] Then we do add fill.
[137:09] Now we can control the strength of the details.
[137:15] Let's just slide that in slowly until we get something nice.
[137:32] Let's also add a color contrast.
[137:36] Color correct on top.
[137:39] Again let's put this in a folder called adjustments.
[137:45] Pass through.
[137:46] Apply it to all channels.
[137:49] It's called roughness.
[137:53] Put this to rough.
[137:56] I'm going to be messing with luminosity.
[138:00] The midtones.
[138:02] Try to get a little bit more shiny.
[138:05] I think that works quite well.
[138:12] Now that we have that done, let's go ahead and call this.
[138:18] Worn.
[138:20] Let's start with metal.
[138:23] When we look for metal, I want to see all the metals that we have.
[138:31] It might also be a better idea to start off with a trigon.
[138:35] When you look for a trigon ladder.
[138:38] That won't just be showing the trigon ladders, but also the trigon base ladders.
[138:45] Now let's just keep on going with this naming convention.
[138:49] Let's call this metal.
[138:54] Worn.
[138:55] Trigon.
[138:57] Right click.
[138:59] Create smart material.
[139:02] Now you can see we have a metal wand trigon.
[139:05] Again next time I'm going to text you, I'm going to look for trigon.
[139:09] You'll see that I have three smart materials ready to go.
[139:17] That's going to be it for this section of creating smart materials and using them.


### Using Baked Maps to Refine Textures [139:25]
**Transcript (timestamped):**
[139:25] Now that we finished with all our material work, let's go ahead and talk a little bit about using our baked maps to add some detail and depth and extra push to the textures.
[139:42] I'm going to take this, group it together.
[139:47] Let's call this materials.
[139:58] Then we're going to be creating a new HSL.
[140:07] Let's group this and call this baked.
[140:11] Actually let's call this effects.
[140:16] Let's call this on AO.
[140:21] Now we're going to make this darker.
[140:26] And I've set this to pass through, applied to all channels.
[140:32] Now we can darken everything.
[140:35] Now I'm going to say add black mask, fill.
[140:40] Now if we go to project we can see our baked maps.
[140:44] We're going to take the ambient occlusion which stands for AO.
[140:48] Drop that in here.
[140:50] Let's check that out.
[140:52] And then lastly we want to go ahead and do a levels and invert that.
[141:00] Now everything that has a shadow of a high poly is going to be a little bit darker which can add some nice looking depth to the textures.
[141:12] For example take a look right here.
[141:19] How much more depth we're getting with the AO instead of not having that AO on top.
[141:28] Let's go ahead and up the saturation a little bit.
[141:32] A little bit darker.
[141:34] Take a look at the color.
[141:36] See what that's doing and that's looking pretty nice.
[141:44] So we're going to do the same with the curvature.
[141:47] Now add a fill layer.
[141:49] Let's call this curve short for curvature.
[141:53] Alt click color and roughness.
[141:56] I'm going to add the curvature in the fill.
[142:00] Let's get the color back.
[142:02] So I'm going to add this in the fill.
[142:06] Then we go to base color.
[142:08] Let's set this to overlay.
[142:12] Take a look at the base color.
[142:15] Now you can see that we're getting some of the details that we sculpted with in ZBrush into our base color.
[142:22] We want to keep this nice and subtle.
[142:24] We can put something like 27.
[142:27] You can see we'll just add a little bit of that depth into it.
[142:33] Which is very nice.
[142:36] Now if we go roughness let's say, apply to all channels.
[142:42] Now if we go to the roughness let's go ahead and adjust the length of that.
[142:48] Something like 29.
[142:51] This is just going to add a little bit of depth and sharpness to your edges.
[142:58] If we disable the group we can see what it's doing.
[143:04] And then lastly we're going to add a sharpen on top of this.
[143:12] So let's go filter.
[143:16] Sharpen.
[143:18] We're going to sharpen our texture a little bit.
[143:21] We want to keep this nice and subtle so it doesn't become just a big noise.
[143:25] Let's go with point 25.
[143:30] Take a look at the color.
[143:34] See how everything becomes a little bit sharper looking.
[143:39] Take a look at the roughness. Everything becomes a bit sharper.
[143:43] We'll do the same for the metal but we don't really need it in the metal.
[143:54] We can disable and enable it and you'll see it will just add a little bit of that extra nice effect to our textures.


### Wear and Tear [144:06]
**Transcript (timestamped):**
[144:07] Now that we have our materials and effect set up.
[144:11] We need to do one more thing to blend all the materials a little bit nicer together and give it some more realism.
[144:19] That's going to be adding some wear and tear and environmental storytelling.
[144:25] So what does that mean?
[144:28] We add a layer. Let's say this is a leather belt that's being used by a viking.
[144:35] This went through battle so you'd probably expect to see some blood on his clothes.
[144:42] Now we can just add some red.
[144:47] Adjust the roughness. Let's go with a dry blood. Let's go with a deeper darker red.
[144:56] Create a group. This should be under the effects layer.
[145:04] I like to call this group environmental wear.
[145:12] Let's group this fill layer. Let's call this blood.
[145:19] Add the black mask.
[145:25] Now let's talk a little bit. Actually before we do that let's just do fill.
[145:35] Let's go to textures. Let's look for a nice one.
[145:44] A pretty nice one for this would be the moisture.
[145:48] Add the moisture. Alt-click this. Try planar so it blends with the seams.
[145:55] Just dialing the contrast.
[146:03] Add some break up. Fill.
[146:06] We just add another moisture. Let's put this to multiply.
[146:21] We're going to add one more fill. Multiply so we can take away a little bit more.
[146:43] Now you can see that there's some blood on here. It's nice and subtle as it should be.
[146:56] Maybe we can add another blood. That's less subtle.
[147:00] At this point we can group the blood together. Let's call this blood.
[147:06] Call this one blood general. Let's make this one a little bit more general.
[147:20] Take down the contrast of all this.
[147:28] That's going to be our general blood. Duplicate this. Call this blood. Let it.
[147:47] Get rid of this mask. Do a fill. We can go with something like dirt too.
[147:56] Just want some blood splatters.
[148:03] Also make this one a little bit different in color. Maybe a little more shiny.
[148:22] Now we have some blood on our belt. Again you want to keep this pretty nice and subtle usually.
[148:32] I think we can pump this up a little bit. We can go ahead and put the levels on top of this.
[148:41] We can just push the whites.
[148:50] We can go with something like this.
[149:04] I think this looks pretty nice. This spots maybe a little bit too prominent.
[149:11] We can go blood general. We can do paint. We can start to paint away a little bit.
[149:19] We can go to paint. Dirt is a pretty nice one. Dirt one. It's nice and subtle.
[149:26] Hit X to switch the color to black. We're just going to be painting. Maybe that's too much.
[149:32] Let's go with a more gray value. Paint a little bit away. Paint a little bit with it.
[149:40] Go to black. Start painting that away a little bit.
[149:45] I can see we have a very subtle spot that we can just kind of get rid of.
[149:54] Now the blood is looking pretty nice. But everything is the same red.
[150:00] So what we can do, we can go filter. HSL on top.
[150:07] Up the lightness maybe. The saturation. Let me put that down a little bit.
[150:15] Black mask. Fill. And add the clouds.
[150:23] Just going to put that to try planar. Up the contrast. Just tiling.
[150:34] Let's go ahead and put that contrast down again. The balance down.
[150:40] Now we have some variation in the color of our blood.
[150:57] Quickly add more variation by just duplicating this. Let's call this a variation.
[151:05] 0.1. Duplicate it.
[151:18] Now all that we need to do is just rotate it a little bit.
[151:24] Now adjust the value.
[151:34] Group this together. As true. Let's call this a variation.
[151:42] You can see it's basically the same principles building up that smart material.
[151:48] Now we're doing it for blood. Go roughness.
[151:53] Add a filter. Contrast luminance, roughness.
[152:00] Adjust that a little bit. Then apply it to all channels.
[152:09] Make this a nice rough blood.
[152:27] Just like that. I'm sure you can already see it coming.
[152:32] We can take the blood. Let's add blood and score.
[152:36] Trigon. You can say create smart material.
[152:46] You see now that we have a Trigon blood smart material.
[152:54] This is what I was talking about earlier when you do have a mask.
[152:58] You can see that it will be black with just some spots on top where the mask is.
[153:04] Which in this case is a nice thing as it's supposed to be like blood splatters.
[153:12] So even when we're doing like environmental wear, I would still go like smart materials.
[153:20] I'd look for my materials, Trigon.
[153:23] Then I'd have here like dust, sand, blood and whatever.
[153:29] Anything that you can think about.
[153:32] By adding blood we're not only making the text look more interesting but we're also telling a story.
[153:40] Right now this leather belt is clearly being used by someone that went through a battle or whatever.
[153:47] It's something where people go to hurt which tells a story.
[153:54] Now let's add one more.
[153:56] Add a really quick and simple dust.
[154:01] Wear.
[154:05] So we have another way of creating masks.
[154:09] We don't need to do it manually every time with a black mask and fill and create blah blah blah.
[154:15] We can use smart masks.
[154:19] With these you can also make your own presets by the way.
[154:23] But for now let's just stick to the default ones.
[154:26] We're gonna look for dust.
[154:30] So over here we can see some masks.
[154:33] We can look for one that we like.
[154:35] Let's try dust double.
[154:38] Put that on, see how that looks.
[154:40] I don't like how that looks.
[154:41] Let's take it off.
[154:43] Maybe we can try sand dust.
[154:46] We're just gonna be looking for one that we like.
[154:49] I think this one looks pretty cool.
[154:51] Let's go with that.
[154:54] Let's give this like a bluish color to complement like the reddish tones that we have going on.
[155:00] Dust is very rough.
[155:02] Let's make it very rough.
[155:07] Definitely think it's too strong.
[155:10] We can go to mask editor.
[155:12] We can put global balance down to get a little bit less.
[155:18] Although I think this was looking more interesting so we can keep it like that.
[155:22] Then we can add a yellow on top.
[155:25] Put this to multiply.
[155:27] Then we can control the strength of that mask.
[155:32] Again we're multiplying black on top of the whites.
[155:38] Maybe something like this.
[155:44] We can do a second dust.
[155:55] Maybe one on the edges, that's pretty nice.
[156:08] That's not bad.
[156:10] A little bit lower perhaps.
[156:13] Maybe something like this.
[156:15] Although I think we need some break up.
[156:18] So on top of our smart mask we can go again fill.
[156:24] Let's get like a clouds.
[156:26] Just to multiply.
[156:29] Try playing a projection.
[156:32] Let's mess with the settings.
[156:35] I want to be taking stuff away.
[156:38] For a bigger tiling.
[156:50] Maybe this one can be a more like whiteish color.
[157:03] Go ahead and group all the dust together.
[157:07] Do our dust group.
[157:09] Add the black mask and fill.
[157:13] Now we can control the strength of our dust.
[157:18] Something subtle.
[157:20] Let's do the same for the blood.
[157:22] Add the black mask and fill.
[157:24] Now we can control the strength of our blood.
[157:30] Let's go with something like this.
[157:37] Now we're pretty much done with the environmental wear.
[157:45] I want to show you one more thing to add some more wear to this.
[157:49] Whenever we have a material that's composed out of multiple materials.
[157:55] For example our leather.
[157:57] We have the top layer and the bottom layer.
[158:01] We can go to the top layer.
[158:04] We can add some black to this.
[158:07] The easiest way to do that is to group it.
[158:11] Let's go to the top layer.
[158:16] Then control alt v to copy that mask.
[158:20] Control alt v to paste it.
[158:23] Now we're going to add a black mask.
[158:28] Now we don't see anything.
[158:30] Let's undo a little bit.
[158:32] Let's go to hide.
[158:34] We need to replace the new top layer.
[158:41] Now on top layer let's add wear mask.
[158:49] Let's add a black mask.
[158:54] What we can do now is we can use smart masks.
[158:57] We can for example say fabric edges.
[159:02] Drop that in here.
[159:05] Now you can see we get a pretty interesting mask.
[159:09] We need to invert this mask.
[159:14] Now if we adjust this.
[159:17] Let's up the global balance.
[159:19] You can see that it will start to show the layer underneath.
[159:25] Keep this nice and subtle.
[159:29] Let's contrast a little bit.
[159:36] Now for example you can see that we're starting to get some nice wear around the edges.
[159:41] We disable that mask.
[159:43] You can see this looks a little bit boring.
[159:46] Now we have some nice wear.
[159:49] Then some wear around the cracks.
[159:51] That's because of the curvature map.
[159:55] By blending your materials you can add some quick looking break up and damage.
[160:03] For example we could add a pill on top of this.
[160:07] Let's look for scratches.
[160:24] I think we need to set this subtract.
[160:30] Now we can have some scratches on our material.
[160:37] At any time we can adjust the balance of the scratches.
[160:42] Scratch tiling to get smaller scratches and whatever.
[160:48] The default settings work pretty well.
[160:51] Let's keep it like that.


### Final Adjustments [160:55]
**Transcript (timestamped):**
[160:56] Let's say we're all happy with our textures.
[160:59] We save the next day.
[161:01] We open it up.
[161:02] We think ok I like it.
[161:04] Maybe it's a little bit too saturated.
[161:08] What we can do is we can go.
[161:10] Let's say our leather is too saturated.
[161:13] Let's go to our leather and look in the leather.
[161:16] Ok leather blah blah blah blah.
[161:19] Top wear leather, trigon, adjustment.
[161:22] We can add a HSL.
[161:25] Or if we say ok I like it.
[161:28] But all the textures are a bit too saturated.
[161:33] On top of the effects.
[161:36] Just go.
[161:38] Adjustments, HSL.
[161:41] There's something that I use quite a lot.
[161:45] After I'm finished with my textures.
[161:48] Just add a quick HSL all the way on top.
[161:51] I just mess a little bit with the saturation of things.
[161:55] The lightness and see if I can get something that looks a little bit nice than what I had originally.
[162:06] This is just a quick way to try to push your textures.
[162:11] For example I do think I overdid the saturation a little bit.
[162:16] I like it a little bit better with a lower saturation.
[162:21] Group this.
[162:22] I call this Adjustments.
[162:26] We can do the same for the color.
[162:35] We can do the same for the roughness.
[162:39] Alt click that and let's mess around a little bit with that.
[162:47] Because we need to set this to best through.
[162:50] I like all channels.
[162:54] So on the roughness we can say ok let's try to make it look more shiny.
[162:59] Let's shine it.
[163:05] Now what maybe we make it a little bit more shiny.
[163:09] Something like this.
[163:12] So even if you finished all your texturing you can still try to kind of push it in whatever direction you want.
[163:20] It's done by adding some quick adjustments with filters.
[163:27] By just taking a second to do this you usually get a nice looking texture.
[163:36] So just kind of looking and I think we're pretty much ready.
[163:41] I think we can call this one done.


### Exporting Textures [163:45]
**Transcript (timestamped):**
[163:47] So now let's go ahead and save our project.
[163:50] Ctrl S as in save.
[163:53] Then to export we can say Ctrl Shift E as in export or we can go file export textures.
[164:05] Now we have a whole bunch of settings.
[164:08] Again if you're going to be working on a game you should probably be putting an Unreal Engine template.
[164:16] Just so everything gets packed nicely together for rendering.
[164:20] We can just keep it at metallic roughness.
[164:26] But my third one that I usually go with if I'm just going to do a render is document channels plus normal plus AO.
[164:36] No alpha with alpha depending if you have opacity let's just go with no alpha.
[164:41] PNG is pretty nice.
[164:43] Put it to 16 bits.
[164:46] This means that you get a bigger file size but more like information in your pixels like a further range.
[164:55] It's just going to make it look nice and again if we're texturing we want it to look as nice as possible.
[165:01] Now size even if you were texturing let's say 1k we can still export at 4k.
[165:08] Anytime we change the resolution the layer stack.
[165:12] We'll be calculating it again and it will be true for k.
[165:19] So lastly build MTL that's going to be the name of our textures.
[165:24] If you're not happy with that name we can say save settings.
[165:28] Text is at list let's change this to build.
[165:32] Let's go with letter.
[165:35] Bell.
[165:38] Ctrl Shift E is an export.
[165:43] Now we see letter.
[165:47] Now all that we have to set an output directory.
[165:55] Select this let's create a new folder all these textures.
[166:03] And select folder.
[166:05] Now we're going to export them.
[166:12] Save settings.
[166:14] Now you've officially finished your textures.
[166:17] You can use them in Marmoset or any other software to render.
[166:26] You can take a quick look at the textures.
[166:29] Also we can get rid of the letter belt normal.
[166:33] We don't need that.
[166:35] We need the letter belt normal open GL.
[166:39] Now as you can see now we have our textures all ready and done.
[166:52] So I hope you enjoyed this chapter.
[166:55] This is going to be the most important chapter in the course.
[166:59] Because this is going to be your base.
[167:02] Like your building blocks.
[167:04] This is the base that you need to work in Substance Painter.
[167:08] If you can master these techniques you can pretty much texture anything and everything that you want.
[167:16] From that point on you can start looking at more techniques and more stuff that you like.
[167:22] To keep adding to that workflow.
[167:25] But for me this is a very strong foundation that you can use to texture anything that you would like.
[167:35] And depending on the time that you see this course.
[167:38] This might be the final chapter.
[167:41] Or if we are a little bit further in the future this is going to be chapters with more advanced techniques.
[167:47] And ways to improve your workflow.
[167:50] And to accomplish more complicated materials and better textures.



---

## Captured Frames

- [6:10] tutorials/frames/substance-painter-beginner-to-pro---course/frame_000.jpg
- [11:20] tutorials/frames/substance-painter-beginner-to-pro---course/frame_001.jpg
- [14:14] tutorials/frames/substance-painter-beginner-to-pro---course/frame_002.jpg
- [24:25] tutorials/frames/substance-painter-beginner-to-pro---course/frame_003.jpg
- [39:05] tutorials/frames/substance-painter-beginner-to-pro---course/frame_004.jpg
- [53:00] tutorials/frames/substance-painter-beginner-to-pro---course/frame_005.jpg
- [60:53] tutorials/frames/substance-painter-beginner-to-pro---course/frame_006.jpg
- [66:33] tutorials/frames/substance-painter-beginner-to-pro---course/frame_007.jpg
- [73:50] tutorials/frames/substance-painter-beginner-to-pro---course/frame_008.jpg
- [77:03] tutorials/frames/substance-painter-beginner-to-pro---course/frame_009.jpg
- [84:08] tutorials/frames/substance-painter-beginner-to-pro---course/frame_010.jpg
- [100:58] tutorials/frames/substance-painter-beginner-to-pro---course/frame_011.jpg
- [119:15] tutorials/frames/substance-painter-beginner-to-pro---course/frame_012.jpg
- [120:50] tutorials/frames/substance-painter-beginner-to-pro---course/frame_013.jpg
- [140:48] tutorials/frames/substance-painter-beginner-to-pro---course/frame_014.jpg
- [155:00] tutorials/frames/substance-painter-beginner-to-pro---course/frame_015.jpg
- [164:25] tutorials/frames/substance-painter-beginner-to-pro---course/frame_016.jpg

---

## Structured Notes

### Core Technique
Complete zero-to-production foundations course (2h48m, 26 chapters) building up Painter's core mental model layer by layer — layers/fill-layers → channels → masking → smart materials → filters → baking → ID maps — then applying every piece to a single real asset (a leather belt with metal buckle) through blocking-out, a fully non-destructive filter-driven "primary/secondary/tertiary breakup" material-building method, baked-map-driven refinement (AO/curvature), environmental wear/storytelling, and export. The throughline technique taught across nearly every later chapter is **building materials entirely from Pass-Through filters (HSL / Contrast & Luminance / Color Balance / Levels) rather than editing base Fill-layer values directly**, so that any earlier decision (e.g. base leather color) can be changed once and propagate through every dependent layer automatically.

### Summary
**Fundamentals (0:00-44:39):** Establishes layers vs. fill layers (fill layers carry all base channel values at once), the channel model (BaseColor/Height/Roughness/Metallic/Normal — Metallic should almost always stay a pure 0 or 1, not an intermediate value), masking (right-click → Add White/Black Mask, Alt-click a mask thumbnail to preview it in isolation, paint mask values in grayscale — not just pure black/white — for partial-strength effects, hotkey X to swap paint color between black/white), Smart Materials (pre-built layer/effect stacks you drag onto a model or into the stack; a Smart Material's internal layers should always be clearly named — e.g. Base Metal / Dirt / Surface Details / Edges / Damage / Sharpen — so you know what to tweak), and Filters (a filter layer holds a filter — e.g. HSL, Contrast & Luminance — that can target one channel via Alt-click on that channel button, letting you re-grade a material's color or roughness in seconds instead of hunting through every base layer; filters should always be named for what they do). **Baking (46:27-65:06):** explains what each mesh map means (Normal and Ambient Occlusion are the two you'll always use directly; ID, Curvature, Position, Thickness mainly exist to build masks later); demonstrates baking a real high-to-low-poly asset (belt + buckle from ZBrush), the ID map needing its Color Source switched from Material Color to **Vertex Color** (since the ID color was authored as ZBrush PolyPaint), baking best-practice (bake test passes at low Anti-Aliasing/resolution first, final pass at 64x AA and double your final texture resolution — e.g. bake 4K for a 2K final export, except at 4K final where you bake at 4K to avoid an unwieldy 8K), fixing intersection/projection bake errors by splitting a mesh into separate objects (belt / buckle / buckle-clip) with matching `_low`/`_high` name suffixes and setting **Match by mesh name** in the Baking settings, and manually widening the **Cage** (inflated bake-ray-search mesh, visualized as green wireframe) as close to the high-poly as possible without it self-intersecting (shown in the red/green **matching-error heatmap**) — noting plainly that Painter's cage tools have real limits and the video's own residual bake artifact was left unfixed as an honest example (creator's own preference for hard cases: bake externally in Marmoset and import the maps). **ID Maps (65:06-69:18):** using **Add Mask with Color Selection** to pick a color from the baked ID map and instantly get a perfect mask for that mesh region, adjustable Hardness/Tolerance for near-identical ID colors, and an alternate "background white / output black" ID mode for isolating a single color as a hole-punch mask (used later for stitches). **Blocking Out Materials (69:18-75:35):** establishes flat base-color/roughness/metallic values and ID-map-driven masks for every material up front (leather base layers, a second "shiny top-coat" leather layer masked to just part of the ID region, a separate stitches layer) before any detail work — creating "all the masks you'll ever need" early so later chapters just swap folder contents. **The Power of Effects (75:35-80:24):** the pivotal non-destructive-workflow lesson — instead of hand-painting a fixed color onto stitches (which breaks the moment the base leather color changes), copy the base layer's mask onto an HSL filter layer (Ctrl+Alt+C / Ctrl+Alt+V) set to only lighten/tweak, so the stitches automatically track any future base-color change; filters can themselves be placed inside their own layer (magic-wand "Add Filter" icon) targeted to a single channel via Alt-click. **Adding Variation (80:24-98:58):** the core material-breakup recipe — duplicate a base Fill layer, mask it with a **Tri-Planar-projected** procedural noise (Clouds/Grunge from the Assets shelf, chosen specifically to avoid UV seams), add a second smaller-scale noise on **Multiply** to break up the first noise's own visible tiling, group multiple such passes (Lighten / Darken / Saturation-spots) under a **Pass Through**-blended folder, and organize them by scale into a **primary / secondary / tertiary breakup structure** (one big low-frequency pass, one medium pass, one small subtle pass) — the video's stated single most important realism principle. **Adding Details (98:58-119:51):** layering a tileable material texture (default Painter leather resource, deliberately over-scaled beyond real-world size so it "reads" at game distance) into Height only, inverting via Levels if needed, Blurring a noisy height mask to soften it, then feeding the same mask into a Pass-Through HSL (color) and Contrast & Luminance (roughness) so the detail affects every channel consistently; breaking up an obviously-tiling detail pass with a Tri-Planar Multiply noise, controlled via Opacity rather than deleting the effect; and a first introduction to **Anchor Points** (add on a mask, reference it from any layer above via "Fill → Anchor Points" or a filter's mask source) used here to re-inject a saved mask as an extra Roughness-only boost layer. **Smart Material save/reuse (119:51-139:25):** grouping a finished material (cannot have a mask on the group itself, or the resulting thumbnail breaks) and right-click → **Create Smart Material**, with a deliberate naming convention (`Material_YourName` / `Material_Trigon`) so personal libraries stay searchable and distinct from Painter's defaults; demonstrates rapidly re-skinning a blockout by dragging saved Smart Materials in, deleting the temporary blockout layer, then grading the whole result with one top HSL filter; and building a second (metal) Smart Material the same way. **Baked-Map Refinement (139:25-144:06):** an AO-driven darkening pass (HSL/Contrast layer set to Pass-Through-all-channels, masked by the baked **Ambient Occlusion** map inverted via Levels) and a Curvature-driven pass (Curvature map loaded directly into a Fill layer's BaseColor at low Overlay opacity and Roughness at a small amount) to push baked high-poly surface detail back into the final texture, finished with a subtle **Sharpen** filter. **Wear and Tear (144:06-160:55):** environmental storytelling — building a "blood" Smart Material from layered Moisture/Dirt-texture masks with Tri-Planar + Multiply breakup, HSL color variation, hand-painted cleanup with the Dirt brush, and Contrast & Luminance for rough blood, saved as another reusable Smart Material; a "dust" pass built from the built-in **Smart Masks** library (search "dust", e.g. Dust Double / Sand Dust) rather than hand-built masks, tinted and layered with a second dust pass and Tri-Planar breakup; and cross-material edge wear achieved by copying the top-coat leather layer's mask onto a new masked-with-a-Smart-Mask ("Fabric Edges", inverted) layer set to reveal the rough base-leather layer underneath at the edges/cracks, finished with a Subtract-mode Scratches Smart Mask. **Final Adjustments & Export (160:55-168:03):** a closing top-of-stack HSL/Color-Balance/Contrast pass (Pass-Through, all channels) purely for a final look-grade after "sleeping on it," then **Ctrl+Shift+E** to open Export Textures — choosing an output template (Unreal Engine template if game-bound, or "Document Channels + Normal + AO" for a straight render), No Alpha unless Opacity is used, PNG at 16-bit for extra dynamic range, exporting at full target resolution regardless of the texturing resolution (the layer stack recalculates at whatever export size is chosen), and a custom filename template via **Save Settings**.

### Key Steps
**Fundamentals**
1. Fill layers carry every channel's base value at once (vs. plain paint layers, which hold only paint strokes); delete the default layer and build from a blank stack to learn the primitives cleanly.
2. Channels = Base Color, Height, Roughness, Metallic, Normal; hit `C` repeatedly to cycle the 2D channel-preview view, `F2`/`F3` to toggle 3D/2D, `M` for the full shaded material view.
3. Metallic should almost always be a pure 0 or 1 (non-metal or metal), not an in-between value, with rare exceptions.
4. Add masks via right-click → Add White Mask / Add Black Mask; Alt-click the mask thumbnail to preview it in isolation; paint mask values can be any gray value (not just pure black/white) for partial-strength effects; `X` swaps the paint color between black and white.
5. Smart Materials are just grouped, well-named fill-layer + effect stacks; drag one onto the model or into the layer stack; open one up and inspect/rename its internal layers (Base / Dirt / Surface Details / Edges / Damage / Sharpen) to learn how professionally-built materials are organized.
6. Filters (HSL, Contrast & Luminance, etc.) placed above a material re-grade color/roughness/etc. in seconds without hunting through base layers; Alt-click a specific channel icon on the filter to restrict it to just that channel; always name filters for what they do (e.g. "Color Adjustment", "Roughness Adjustment").

**Baking**
7. Mesh maps to know: Normal and Ambient Occlusion are used directly; ID, Curvature, Position, Thickness mainly exist to build masks later; World Space Normal is mostly a masking helper too.
8. ID map's **Color Source** must be set to **Vertex Color** (not Material Color) when the ID data was authored as ZBrush PolyPaint.
9. Bake at low settings first for a fast test pass; final bake at 64x supersampling and roughly double your intended final export resolution (bake 4K for a 2K export; bake 4K, not 8K, if your final target is already 4K).
10. Fix bake intersection/projection errors by splitting the mesh into separate low/high objects with matching name suffixes (`_low` / `_high`) and setting the Baker's **Match** mode to **By mesh name** — verify with the Match-by-name check panel, which flags mismatched names in red.
11. The **Cage** (inflated search-mesh, shown as a colored wireframe) should be pushed as close to the high-poly as possible without self-intersecting; the **matching-error heatmap** (red = bad, green = good) is the direct feedback signal; acknowledges Painter's cage tools have real limits — some intersection artifacts may not be fixable purely in Painter's cage UI (creator's own workaround for hard cases: bake externally in Marmoset, import the resulting maps).
12. Preview any individual baked map at any time with the `B` hotkey to cycle through bakes.

**ID Maps → Blocking Out**
13. Right-click a mask → **Add Mask with Color Selection** → Pick Color from the baked ID map for an instant, perfectly-fitted regional mask; Hardness/Tolerance sliders help when two ID colors are close together.
14. An alternate ID-map mode ("background = white, output = black") turns any picked ID color into a hole-punch/cutout mask — used for isolating stitches.
15. Before any detail work, block out every material's base BaseColor/Roughness/Metallic values and every mask (including a separate "shiny top-coat" leather layer masked to a sub-region of the base leather's ID color, and a dedicated stitches layer) — this "quick representation of the final texture" front-loads all mask-building so later chapters only swap folder contents.

**Non-Destructive Workflow (Power of Effects)**
16. Instead of hand-painting a fixed detail color (e.g. stitches) that breaks when the base material color changes later, **copy the base layer's mask** (Ctrl+Alt+C) and **paste it onto a filter layer** (Ctrl+Alt+V, e.g. HSL set to only lighten) — the detail then automatically tracks any future base-color edit.
17. A filter can live inside its own dedicated layer (magic-wand "Add Filter" icon) so multiple filters can be organized, named, and toggled independently; Alt-click a channel icon to restrict a filter to just that channel.

**Adding Variation (primary/secondary/tertiary breakup)**
18. Duplicate a base Fill layer to create a "Lighten" (or "Darken") variant with slightly different Base Color/Roughness values.
19. Mask it with a **Tri-Planar**-projected procedural noise from Assets → Procedurals/Grunges (e.g. Clouds 3) — Tri-Planar avoids visible UV seams that plain UV projection would show.
20. Add a second, smaller-scale noise on top set to **Multiply** blend mode to break up the first noise's own repeating tiling pattern; adjust Balance/Contrast/Tiling/Rotation on both until the pattern reads as organic, not obviously repeating.
21. Duplicate this whole recipe for additional passes (a "Saturation" pass for small colorful spots, a "Big Breakup" pass on Roughness for large-scale variation) and group them all under one folder set to **Pass Through** blend mode (required — filters inside a group default to Normal and go invisible until switched) via right-click → Pass Through → **Apply to all channels**.
22. Organize breakup passes explicitly by scale — small, medium, and large ("primary, secondary, tertiary structure") — as the single stated most important realism principle in the whole course.

**Adding Details**
23. Load a tileable detail texture (Painter's built-in leather resource, or your own) into a Fill layer's Height channel only (Alt-click Height to isolate it); deliberately scale the tiling **larger** than real-world size so detail reads at typical viewing/game distance.
24. Invert the detail mask with a **Levels** filter if the source texture reads backwards (dark cracks vs. light cracks); **Blur** a noisy detail mask slightly (e.g. 0.6-0.9) to soften without losing the pattern.
25. Feed the same detail mask into a Pass-Through **HSL** (color) and **Contrast & Luminance** (roughness) layer so the detail consistently affects every channel, not just Height.
26. Break up an obviously-tiling detail pass with a small Tri-Planar Multiply noise layer, controlling its strength via **Opacity** rather than deleting the effect outright if it removes too much detail.
27. First introduction to **Anchor Points**: add one on a mask, then any layer positioned above it can reference that exact mask via "Fill → Anchor Points" (or as a filter's mask source) — demonstrated re-injecting a saved detail mask as a separate, independently-tunable Roughness-boost layer via added Levels.

**Smart Material Save/Reuse**
28. A group cannot have a mask directly on it when saved as a Smart Material (the resulting thumbnail breaks) — group the material's contents cleanly first, then right-click → **Create Smart Material**.
29. Use a deliberate naming convention (e.g. `Leather_Trigon`, prefixed with your name/studio) so your own Smart Material library stays searchable and distinct from Painter's built-in defaults, especially once you've built dozens of variants.
30. Rapidly re-skin a blocked-out mesh by dragging a saved Smart Material onto each masked base layer, deleting the temporary flat-color blockout layer once replaced, then applying one top-level grading filter (HSL: saturation/lightness) for quick large color changes (e.g. "the concept says this leather should be black").

**Baked-Map Refinement**
31. Add an AO-driven darkening pass: an HSL or Contrast layer set to **Pass Through + Apply to all channels**, masked by the baked **Ambient Occlusion** map (dropped from the Project/baked-maps panel) with **Levels → Invert** so occluded crevices read darker — adds real depth from the high-poly bake.
32. Add a Curvature-driven pass: load the baked **Curvature** map directly into a Fill layer's Base Color channel at a low **Overlay** opacity (~25-30%) and independently into Roughness (Apply to all channels first, then dial per-channel), pushing baked-in sculpt detail (edges/creases) back into the final texture.
33. Finish with a subtle **Sharpen** filter (~0.25) applied per-channel — kept deliberately mild to avoid a noisy/burnt look.

**Wear and Tear**
34. Build a "blood" Smart Material the same layered way as any other material: base red Fill layer, masked with **Moisture**/Dirt textures at Tri-Planar projection plus a Multiply breakup pass, hand-painted cleanup with the Dirt brush (`X` to toggle black/white paint), an HSL variation pass (masked by more Tri-Planar clouds) for non-uniform blood color, and a Contrast & Luminance pass for rough blood — saved as its own reusable Smart Material once finished.
35. Build a "dust" pass from Painter's built-in **Smart Masks** library (search "dust" — e.g. Dust Double, Sand Dust) instead of hand-building a mask from scratch; tint with color, layer a second dust pass, and break up with a Tri-Planar Multiply noise.
36. Cross-material edge wear: copy the top-coat leather layer's mask (Ctrl+Alt+C/V) onto a new layer, mask it with a built-in **Smart Mask** ("Fabric Edges", inverted) so the rough base-leather layer shows through at edges/cracks (curvature-driven), finish with a **Subtract**-mode Scratches Smart Mask for fine damage.

**Final Adjustments & Export**
37. Close with a top-of-stack HSL/Color-Balance/Contrast/Levels pass (grouped, Pass-Through, Apply to all channels) purely as a final look-grade — a habit worth doing even after "finishing," often after stepping away and returning with fresh eyes.
38. Export via `Ctrl+Shift+E` (or File → Export Textures): choose an output template (an Unreal Engine template for game work so maps pack correctly; "Document Channels + Normal + AO" for a straight external render), set Alpha to No Alpha unless Opacity is genuinely used, PNG at 16-bit for extra dynamic range, and export at your true target resolution regardless of what resolution you textured at (the layer stack recalculates fresh at export time) — customize the output filename template via **Save Settings**.

### Layers / Tools / Settings
- `Fill layer` (all-channel base values) vs. `Paint layer` (strokes only); `Ctrl+G` group, `Ctrl+D` duplicate
- Masks: right-click → Add White/Black Mask, **Add Mask with Color Selection** (ID-map-driven), Alt-click to preview in isolation, `X` to swap paint color
- `Smart Material` (drag-on preset) vs. `Smart Mask` (drag-on mask preset, e.g. Fabric Edges, Dust Double, Sand Dust, Scratches)
- `Filters`: HSL, Contrast and Luminance, Color Balance, Levels, Sharpen, Blur — Alt-click a channel to restrict; group blend mode must be **Pass Through** (+ "Apply to all channels") for filters inside a folder to take effect
- `Anchor Point` (add on a mask; reference via "Fill → Anchor Points" or as a filter's mask source)
- Projection: **Tri-Planar** (seam-free procedural noise placement) vs. plain UV
- Baking: **Match by mesh name**, **Cage** wireframe + matching-error red/green heatmap, ID map **Color Source = Vertex Color**, Anti-Aliasing (test low, final 64x), bake resolution ≈ 2x final export resolution
- Baked maps used directly in-material: **Ambient Occlusion** (Levels-inverted darkening mask), **Curvature** (Overlay BaseColor + Roughness push)
- Copy/paste mask: `Ctrl+Alt+C` / `Ctrl+Alt+V`
- Export: `Ctrl+Shift+E`, output template (Unreal Engine / Document Channels+Normal+AO), 16-bit PNG, No Alpha (unless Opacity used), custom filename via Save Settings

### Difficulty
Beginner through Intermediate — explicitly structured as a ground-up foundations course; the creator states this single chapter/asset ("if you can master these techniques you can pretty much texture anything") is the strongest single foundation in the whole series, with more advanced chapters continuing beyond it depending on when the course is viewed.

### App & Version
Not stated on screen. UI (Baking Mode common settings layout, cage wireframe visualization, matching-error heatmap) is consistent with a modern, post-8.3-era Painter build; no explicit numeric version or version-gated feature name appears in the transcript or captured frames.

### Tags
`layers` `fill-layer` `paint-layer` `masks` `smart-material` `smart-mask` `generator` `anchor-point` `blend-mode` `baking` `mesh-maps` `ambient-occlusion` `curvature` `high-to-low-poly` `cage` `id-map` `texture-set` `pbr` `metal-rough` `basecolor` `roughness` `metallic` `height` `normal-map` `alpha` `tri-planar` `procedural` `export` `export-preset` `channel-packing` `game-engine` `unreal-export` `beginner` `intermediate` `advanced`

---

## Related Tutorials
- [Substance Painter Tutorial - Beginner To Advanced](substance-painter-tutorial---beginner-to-advanced.md) — same creator (TriGon); companion course in the same beginner-to-pro learning arc. Cross-link both ways once ingested.
- [Substance Painter - Creating Professional Textures](substance-painter---creating-professional-textures.md) — same creator (TriGon); the most advanced of the three-part series, building further on this video's primary/secondary/tertiary breakup and non-destructive filter methodology. Cross-link both ways once ingested.
- [SUBSTANCE PAINTER: Building Masks Explained](substance-painter-building-masks-explained.md) — different creator (Jared Chavez); a deeper dive into every masking primitive this course only introduces at a beginner level (generators, tri-planar grunge, anchor points).
- [How to TEXTURE like a PRO with ANCHOR POINTS | Substance Painter Tutorial](how-to-texture-like-a-pro-with-anchor-points-substance-painter-tutorial.md) — different creator (Jared Chavez); a dedicated deep-dive on Anchor Points, which this course only briefly introduces in its "Refining Our Details" chapter.
- [Hand Painted Workflow in Substance 3D Painter](hand-painted-workflow-in-substance-3d-painter-adobe-substance-3d.md) — different creator (Adobe); shares the AO/Position-generator-driven value-first approach that complements this course's AO/Curvature baked-map refinement chapter.
