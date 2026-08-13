---
title: Shading & Lighting a Character - Blender and Substance 3D Painter Workflow
source: YouTube
url: https://www.youtube.com/watch?v=2lHAio4DoWw
author: FlippedNormals
ingested: 2026-08-13
app: "Substance 3D Painter (paired with Blender)"
version: "not stated numerically; UDIM/UV Tiles workflow visible (same project as the companion texturing video); Blender-side uses AgX color management (a then-newer alternative to Filmic) and Cycles"
tags: [texture-set, uv, udim, basecolor, roughness, color-management, export, export-preset, pbr, advanced]
extraction_status: complete
frames_dir: tutorials/frames/shading-lighting-a-character---blender-and-substance-3d-painter-workflow/
frame_count: 2
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Shading & Lighting a Character - Blender and Substance 3D Painter Workflow

**Source:** [YouTube](https://www.youtube.com/watch?v=2lHAio4DoWw)
**Author:** FlippedNormals
**Duration:** 27m11s | 9 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hi, I'm Henning from FlipNomals.com and let's get into my approach for shading and lighting
[0:08] my clicker project from the last of us using Substance Painter and Blender.
[0:12] Now, if you prefer an article instead of just a video, we have a written tutorial on this
[0:18] exact topic over at blog.flipnomals.com, which covers the whole thing as well, step by step.
[0:24] This is very similar to this video.
[0:27] Using Substance Painter, this is where we ended in the texturing video of this project.


### Final Substance 3D Painter maps [0:28]
**Transcript (timestamped):**
[0:33] As you can see, all the maps are now done.
[0:35] And if you break this down, you can see that we essentially only have two maps.
[0:39] We have the base color, then we have the roughness maps.
[0:43] If you spend a lot of time on the actual scope, you really don't need a whole lot more than
[0:48] that.
[0:49] In this case, the high frequency, like all the pores and all that is just done in decimation
[0:55] and we brought the decimator model into Painter and then we brought an even higher decimator
[0:59] version into Blender.
[1:01] So we're straight up rendering the decimator version.
[1:03] And this keeps it really simple.
[1:05] Once the textur maps are done, I've simply exported them out as this separate texture
[1:10] set with only the base color and roughness, which we are going to pick up in Blender.


### Using AgX to replace Filmic [1:15]
**Transcript (timestamped):**
[1:16] In Blender, the very first thing I recommended you do is that you change the LUT from Filmic
[1:21] to AGX.
[1:22] AGX is a new LUT, which is honestly just better than Filmic.
[1:27] There's a link to where you can download AGX in the description, but you can also simply
[1:30] just Google AGX and you're going to find this on GitHub.
[1:36] Once you've installed AGX, you simply go down all the way down under your render settings
[1:40] to color management.
[1:41] You make sure display device is set to sRGB, view transform is AGX and the look is punchy.
[1:48] Even if you aren't using AGX, I highly recommend that you use Filmic, simple because the render
[1:53] will be much more balanced.
[1:55] So once we have this installed and all set up, then it's important to just clean up the
[2:01] scene just a little bit.
[2:02] In this case here, we have all the pieces in and these are imported directly from Seabrush
[2:09] and these are decimated.
[2:11] And that means that this is simply the highest model that has been optimized to retain its
[2:16] shape and details.
[2:17] So keeping the poll account low.
[2:19] In this case, each model has a different poll account, depending on how important it is.
[2:23] For instance, the head has a much higher poll account than these little mushrooms here on
[2:27] this side.
[2:28] And the poll account that's good is really the one that fits your system.
[2:32] I tend to make this as high as possible while still being able to render and not crash in
[2:38] Blender.
[2:39] So with this said, now we have all the objects and I'm going to start making collections


### Organizing the scene with Collections [2:45]
**Transcript (timestamped):**
[2:45] for them.
[2:46] The collections I have here would really be the same models from Seabrush.
[2:49] I haven't really changed them a whole lot.
[2:50] I should have probably renamed these a little bit nicer.
[2:53] But here we go.
[2:55] One thing I've added as well that we haven't spoken about is the fact that I've added a
[2:58] quick wet line.
[2:59] This is simply a model that's right here.
[3:02] And this is a very, very simple model.
[3:04] This is basically just a cube that's been extruded out here and just has a wet material
[3:10] on it.
[3:11] Basically, there's a glass material as that makes a lot more realistic.
[3:14] Because it integrates the gums a lot more and makes it seem like you have a bit of like
[3:19] saliva here.
[3:20] But apart from that, all these are just the same models we've already had in previous
[3:25] videos.
[3:27] And then we have a simple environment.
[3:28] And the environment is very, very, very simple.
[3:30] This is simply just a cube that has been extruded out on the side here, rather a plain that's
[3:35] been extruded.
[3:36] And this just has a very simple material, like a really black material.
[3:39] And this is simply just to block off any lights from like environments or anything like that
[3:45] if we were to use an HDRI, which we're ultimately not using, but it's still kind of nice to
[3:49] have it here because then we can control it quite nicely.
[3:51] And this is just put in an environmental backdrop.
[3:55] Then we have a camera group.
[3:56] And here we have two main cameras.
[3:58] One is the more of a medium shot and one is a proper close up shot.
[4:02] And so we had to have two because we can try out different camera angles really quickly.


### Lighting in Blender using Three Point Lighting [4:07]
**Transcript (timestamped):**
[4:08] Then we have a light group that contains all the lights.
[4:11] And that's where we are going to be starting off right now.
[4:13] So we're starting off with the key light.
[4:15] And this is simply an area light in a pretty high up position, but also pretty frontal
[4:21] lit.
[4:22] When I'm lighting, I tend to keep either 20, 30% in light or 20, 30% in shadow.
[4:30] I try to avoid it being like 50, 50.
[4:32] In this case, you can see that the vast majority is in light.
[4:36] And this is just a general good rule for lighting.
[4:39] It just makes the lighting more comfortable.
[4:41] What I'm doing here as well as I'm trying to establish more of a focal point, I want
[4:44] people to be looking at around this area here.
[4:47] So I'm making this area here a bit brighter, but also you don't have too much control with
[4:51] just a single light.
[4:52] In this case here, you can go under the light settings and I've just added a little bit
[4:56] of color to it.
[4:57] I tend to add a little bit of color to all my lights as it just makes it just a bit
[5:01] more vibrant, even in a case like this where this is quite a neutral light.
[5:06] As a tip, whenever I'm lighting, instead of dragging the slider, I tend to just multiply
[5:10] by two to make it twice as bright or divide by two to make it half the brightness.
[5:16] This is just a quick way to change the brightness.
[5:19] Instead of finding the exact values, it's never about exact values.
[5:22] It's always just about the rough feeling of it.
[5:25] And then you can, of course, tweak this later on if you want to have like highly precise
[5:30] values.
[5:31] But find this to be a good way of doing it.
[5:32] Basically make it twice as bright or half as bright.
[5:35] And then we have the fill light.
[5:36] The fill light is here to simply brighten up the darker parts because without the fill
[5:42] light, you can see it's really dark and we don't want this to be perfectly black.
[5:46] So I'm just using a fill light in this case.
[5:48] I'm not using an HDRI for this project at all.
[5:52] I want to control the lighting fully.
[5:54] And I found that this worked really well.
[5:56] Really what I'm doing here is I'm just using a three point light setup which has a key
[5:59] light, a fill light, and a rim light.
[6:02] What I was missing at this point though was separating the character out a little bit
[6:06] more from the background.
[6:07] It was getting a little dark here and it was blending in a little too much.
[6:10] So I added a rim light as well.
[6:12] And this just separates him out a little bit from the background.
[6:16] As you can see down here and it just adds a bit more.
[6:20] This is more prominent once you're adding subsurface as well.
[6:23] And this is one of the ones you can go really crazy with.
[6:25] You can really like amp this up.
[6:27] But I found that this was just a little bit too crazy.
[6:29] And speaking of subsurface, it's really hard to light and shade.
[6:35] Like do the look of independently of each other.
[6:37] These are highly interconnected processes.
[6:40] For instance, when we're adding subsurface on the character, we're getting feedback as
[6:44] to the light intensity.
[6:45] If it works or not, the specularity is changing drastically based on the lighting.
[6:50] So you really have to be more holistic about it instead of simply just putting up lights
[6:55] and then doing your shading and then doing rendering.
[6:58] You need to constantly be changing the lighting based on the feedback from the materials.
[7:06] As a little heads up in disclaimer, this is not really how you would do it in a professional
[7:09] VFX workflow.
[7:10] What we're doing now is we're setting up a camera.
[7:12] We're basically locking the camera to it.
[7:14] And then we're lighting based on this.
[7:17] And that works really well for our purposes.
[7:20] But if you're doing a character for a full shot or a full sequence, that character would
[7:25] need to work from all angles.
[7:27] So in that case, you would set up a neutral lighting and look at environment, which is
[7:31] more generic than this, where you don't really have too many colors in the lights where you
[7:37] know if it works in that setup, it's going to work in all other setups.
[7:41] So this works well for this case, but don't confuse this with a full on professional lighting
[7:46] and look at that setup.
[7:48] And then it was getting a bit too bright up here.
[7:50] So what I'm doing is I'm simply just adding a light blocker.
[7:53] This is the simplest thing in the world.
[7:55] This is literally just a polygonal plane.
[7:56] I've just placed up here.
[7:58] This is how you can change lighting a lot, where if you just start to think about how
[8:02] you would do this in a physical world, instead of going into like fancy shader techniques
[8:07] or something like that, if you were to be lighting this on set in the real world and
[8:11] you want to have more shadows on the back, how do you do it?
[8:14] Well, you just put some cardboard or something in front of the light and then you will block
[8:19] out that light.
[8:20] So you can see this does quite a lot actually.
[8:21] This one right now, you can see this is real bright and then we add this and it just focuses
[8:27] it just a little bit.
[8:28] It's not like a crazy amount, but it's it just just helps to focus this in terms of
[8:33] the cameras as well.
[8:34] I always tend to lock the cameras so you can do that very easily just by going under the
[8:38] object properties and then just dragging on here.
[8:41] You can see now these are unlocked and just by doing this, you're now locking them.
[8:44] This is really, really handy because you are accidentally going to do this a lot where
[8:49] you you tend to like if you have locked camera to view enabled that you're going to accidentally
[8:56] keep changing the camera and Blinder does not have viewport undoes or camera undoes,
[9:01] which means that if you have a perfect camera set up like this and you move it around, you
[9:07] actually can't go back to it.
[9:09] You have to literally go back to an older file.
[9:12] So definitely make sure to lock the camera like this.
[9:15] This is going to be really beneficial.
[9:17] I do also recommend adding what I'm doing here, adding lock camera to view as well in
[9:21] the quick favorites.
[9:22] You can do this easily just by going to hitting the N key and then going to view and then
[9:27] you have this one here, camera to view and just right click and then add to quick favorites.
[9:31] This is really handy because you often want to do this whenever you are rotating around
[9:36] in the camera or setting up lights and the funny camera angle and such.


### Shading the 3D Character in Cycles for Blender [9:39]
**Transcript (timestamped):**
[9:40] So let's get into the actual shading part of this.
[9:43] What you have to do is select each part of the model and assigning a material based on
[9:48] the texture sets you have in Painter.
[9:51] In this case, the tongue and the rest of the head is going to be one texture set.
[9:57] The top mushrooms are going to be one.
[9:59] The neck mushrooms is going to be one and the teeth is going to be one material.
[10:03] This is something that you will define essentially when you are UV mapping your character.
[10:07] All this is very interconnected.
[10:10] The UV mapping of the character is determining essentially your materials at this point.
[10:15] So really think about the whole process early on.
[10:20] So I've simply just assigned very simple materials to this, just generic materials.
[10:24] And I've just made the base color just like a more of a neutral gray so it will fit the
[10:29] lighting a bit better.
[10:30] And then we are going to go into the various materials.
[10:34] We're going to go into the head, just select the head and then we are going to just assign
[10:39] the various texture maps.
[10:41] One of my core principles, whatever I'm texturing is, I try to keep my texture maps as final
[10:46] as I can, meaning that they don't rely on color corrections and masking and all that
[10:53] in a look at a solution like Blender.
[10:55] The reason is if you have a texture map that's more brownish, exported from Painter, you
[10:59] take it into Blender, you start to color correct it, you make it a bit more greenish, you start
[11:04] to modify the roughness using nodes, and then you want to change it later on.
[11:10] You want to make it a bit more red.
[11:11] It's really tricky to actually do that because now would you change the maps from Painter
[11:15] or you change the hue and saturation, the whole shader network?
[11:19] This is really tricky.
[11:20] So I tend to bring my texture maps into Blender, then I do my color corrections to them, seeing
[11:26] what actually needs to happen.
[11:27] For instance, a hue and saturation can work really well.
[11:30] Then I do the exact same hue and saturation in Painter.
[11:33] I actually export the maps out again from Painter into Blender.
[11:38] I delete all my shader networks and now it should look exactly the same.
[11:41] It just means that I keep the texturing software as the master and I just import the maps here.
[11:47] This means that the shader setup is dead simple.
[11:50] So we are going to start just by hitting Shift and A and then we're going to type image.
[11:56] And we're just going to have an image texture.
[11:57] And now we are just opening this up.
[12:00] And then just select in the head base color.
[12:01] You can see we're using Udems for this, but in this case, we just have a few Udems.
[12:05] So very easy.
[12:06] So just bring this in here.
[12:07] And now you're going to see on the bottom, this has Udems here and this is at sRGB, which
[12:11] is correct.
[12:12] And then I'm just going to duplicate this one, Shift and D. And then we do the same thing
[12:16] here.
[12:17] We are setting this to Roughness as well.
[12:19] And now we have the two maps I need for this.
[12:22] And then I'm going to be setting the subsurface to one.
[12:25] And this is essentially a balance between subsurface and base color.
[12:28] So in this case, if the subsurface is going to be like red or pink or whatever, currently
[12:34] there is no subsurface.
[12:35] And this is set to like 50.
[12:36] Now it's going to be 50%.
[12:37] And now it's set to one.
[12:38] It's going to be 100%, meaning that it's just basically just a blend between the base color
[12:43] and the subsurface.
[12:46] Then we're going to be changing the subsurface amount to random walk, fixed radius.
[12:50] I find this to be a much better way of working compared to the default random walks is to
[12:56] have more control with this one.
[12:58] And then we are going to be plugging the base color into the subsurface color.
[13:03] And now you're going to be able to see we have subsurface.
[13:05] But the problem is that the subsurface is far, far too strong.
[13:09] The way we are fixing this is not by reducing the subsurface here or going in and tweaking
[13:14] the radius, because this is a mess.
[13:16] It's really hard to know what's actually going on here.
[13:18] You could of course visualize it like the red, green and blue, and you can just adjust these
[13:22] values.
[13:23] So instead, we are going to be using a Mix RGB, Shift A, type Mix RGB.
[13:28] And then we are going to be using this color as the radius.
[13:32] And this means we can actually choose the colors using like our eyes instead of using
[13:36] math.
[13:37] So set the fact all the way to zero.
[13:39] And this means that the color one is going to be the slot we're using.
[13:42] And the color we're choosing now is essentially going to be both the value, meaning how strong
[13:47] is the subsurface, but also the actual hue of the subsurface.
[13:51] In this case, you can see it's red, but we can change this as well to something else.
[13:55] So the first thing we'll do, we are simply just going to plug this into the subsurface
[13:58] radius.
[13:59] And now you're going to see that the color indeed changed to this.
[14:02] If we change the color now to pink, you're going to see that this is going to be scattering
[14:05] pink.
[14:06] And now if you just leave this to a neutral way, if you go here and just go and remove
[14:11] the saturation, you can see it's now, we can make it all the way white.
[14:14] So it's really extreme.
[14:15] But if you now were to just change the value of this all the way down, you can see what
[14:19] happens.
[14:20] The subsurface really disappears.
[14:22] So the value controls the amount of subsurface and the color controls a hue.
[14:29] So this is a pretty intuitive way of working.
[14:31] And then what I tend to do is I tend to use a pretty low value with this.
[14:35] And like something like this depends on the scale, but something like 0.03 tends to work
[14:40] really well for me.
[14:41] But again, this does depend on your scale and it depends very much on which model you
[14:45] are using with the fixed radius.
[14:47] This is these values are completely different from if you're using this to random, the default
[14:53] random walk.
[14:54] So now we are just going to be changing this to something like, let's choose here, the
[14:58] value something 0.042.
[15:01] That's fine.
[15:02] And then we're going to pick a color and the color was going to be like this dark ish
[15:05] red color, dark ish red or dark ish, like brown ish color.
[15:11] And this is going to be subtle and you want this to be kind of subtle because if you're
[15:16] exigering this too much, the character is going to seem like it's made of wax.
[15:19] So something like this is actually quite nice.
[15:21] And I can see that the roughness is set to one, which we definitely don't want.
[15:25] We want to use the roughness map.
[15:27] But before that, we have to change the color space to generic data.
[15:31] This is different if you are using Filmic or Not Filmic or AGX.
[15:36] If you are using AGX, your scalar maps, meaning black and white maps or data maps should be
[15:41] set to generic data.
[15:43] And then you simply just plug the roughness into the roughness.
[15:47] And this should just work out of the box.
[15:51] And the reason this should work out of the box is that I've tested this back and forth
[15:54] in a texturing phase.
[15:56] So at this point, when it comes to adding the materials, doing the materials, I'm more
[16:01] thinking about what is the actual material made out of?
[16:04] What is the surface made out of?
[16:06] Not so much what specifically is the color and the roughness because I should have really
[16:10] defined that before.
[16:12] And now you can see we have some nice roughness on our character.
[16:16] We have some nice SSS as well.
[16:17] And this is the same approach for all of the other maps.
[16:21] So we are just going to be choosing this one here.
[16:24] And then we are simply just doing the same thing.
[16:25] This is for Shift A, Image, Duplicate this guy, Shift and D.
[16:33] This is going to be our roughness.
[16:34] So just plug this into roughness.
[16:36] And this is going to be our subsurface.
[16:37] So plug this into subsurface color.
[16:40] And then we're just going to be assigning these textures and changing this to Generic
[16:44] Data.
[16:45] And now the headroom should be working.
[16:48] And now just changing this to Generic Data.
[16:51] And then just changing the SSS to Random Walk Fixed Radius and then setting the subsurface
[16:55] all the way up.
[16:57] And then same thing as before, Mix RGB node.
[17:00] Just moving this up here.
[17:03] You can also just straight up just copy from this one here.
[17:06] That's what I'm going to be doing.
[17:08] So you can see the subsurface is way too strong now.
[17:10] So just plug this in.
[17:11] And then it's the subsurface radius.
[17:16] And there we go.
[17:17] Now we have the headrooms.
[17:18] Now we need the teeth and the neckrooms.
[17:20] And you guessed it, same approach for that.
[17:22] So we are just going to be time-lapsing our head just a little bit.
[17:35] And that's really it for the materials.
[17:45] Like I said before, it's really simple once you've done a good job in Painter and once
[17:49] you've already iterated a bit back and forth between this, then assigning it and the actual
[17:53] final material becomes quite simple.
[17:55] The key to skin shading in Blender or in Arnold or wherever you're doing, like I developed
[18:01] this first in Arnold.
[18:02] So this should definitely work there as well.
[18:04] Because don't use a base color.
[18:06] Use a full subsurface.
[18:08] Plug the diffuse into the subsurface color and use a color for the radius.
[18:12] In this case, we're using a Mix RGB node of FAC set to zero and then a dark and saturated
[18:18] color for the actual value.
[18:23] And this is a simple and powerful system.
[18:25] For roughness, keep it simple and just plug it straight into the roughness slot.
[18:30] If you need to modulate this later on, like if you need to change the value of this, the
[18:33] best way to do this is to use a map range node.
[18:37] And then you can plug this in.
[18:38] You can adjust these values here.
[18:39] Then if you do that, I recommend control shift clicking on the map radius.
[18:44] And now you can see what's happening here.
[18:45] So now you can adjust the values up and down where brighter means is more rough and darker
[18:50] means is smoother.
[18:52] So this is like a good way of doing it.
[18:53] So now, for instance, if we were to change this, a control shift clicking on the material
[18:58] again, we should be able to see that the next mushrooms are much more specky than before.
[19:03] And then use control X to remove it from your shadow network.
[19:06] And now really the last thing we need to do in terms of the look is we need to set up
[19:11] depth of field.
[19:12] And first select the camera you want.
[19:14] And then here's a little tip.
[19:16] If you see the little icon here, this is the active camera icon.
[19:19] So if you click on this one, this is going to change the active camera to a different
[19:22] one.
[19:23] And clicking on this is going to change the active camera here.
[19:26] This is the same as going under your scene properties and changing the active camera here.
[19:30] This is a lot easier since it's just a single click like so.


### Setting up Depth of Field (DOF) for the camera [19:33]
**Transcript (timestamped):**
[19:33] So the way we set up depth of field is very simple.
[19:37] Select the correct camera, the render camera, then go to your camera properties all the
[19:41] way in the bottom here under the data object properties.
[19:43] Then we go all the way down.
[19:44] And here we have a button called or checkbox called depth of field.
[19:48] If you enable this, you now get depth of field and by default, you just get a distance.
[19:53] The problem is, distances kind of suck.
[19:55] You don't really know exactly what it's like.
[19:57] You have to use a ruler and all that.
[19:58] A much better way of doing it is use a depth of field object.
[20:01] And this is very simple to do.
[20:03] You simply just make a new empty or can be any object really, but just an empty.
[20:09] And then you place this where you want the object to be sharp.
[20:12] So in this case, we want it to be around here because this is the area you want to be sharp.
[20:16] And you can see I've already done this.
[20:17] So this is this guy here.
[20:19] And this is the one that's actually under the camera.
[20:21] It's called depth of field or doff and then empty.
[20:24] And you don't have to do anything else with this.
[20:26] The only thing that matters in this case is that this is in the correct position.
[20:32] And then you go all the way down again to your, to your properties.
[20:36] And then this, what you have to change is the F stop.
[20:38] This is similar to a real world camera.
[20:41] So a lower value means more blur.
[20:44] So if you set this to like 0.01, this is going to be blurry as crazy now.
[20:48] But if you set this to 10, then it's going to be really sharp.
[20:51] Now this depends on your scene scale.
[20:54] So if this is like 10 meters, you probably won't really get depth of field.
[20:57] So that's actually why you see up here in the character, I had to have a scale group
[21:01] because the scale was wrong on my actual character.
[21:04] Because honestly, this was just a super stoodle that turned into something larger.
[21:07] So I didn't really consider the scale because so much is dependent on the actual scale.
[21:12] So by setting the scale correctly, even stuff like depth of field is going to be easier.
[21:16] So in this case here, we're using a pretty low value, something like 0.3.
[21:20] And this is like a nice value.
[21:21] We don't want this to be like crazy blurry because then it looks like this guy is tiny.
[21:25] And but making something really blurry, you're also making it more beautiful.
[21:30] And we don't really want this guy to be beautiful.
[21:32] If you want something to look really appealing, like look really cute, then you can add a lot
[21:36] of depth of field.
[21:37] It just means that everything is softer.
[21:39] And if you want something to be like scary and all that, then you can make it really sharp.
[21:43] You can see all the details.
[21:44] Something like 0.3 is a good value for me, but this depends entirely on your character.
[21:50] And then for the blades, this is basically what the depth of field is going to look like.
[21:56] This is also like based on real world cameras.
[21:58] I'm just setting this to five because that makes it nice and just squareish.


### Cycles Blender Settings [22:03]
**Transcript (timestamped):**
[22:03] And that's really for the final look of the character.
[22:05] Now we just have to talk briefly about render settings.
[22:08] And we can do that if we go all the way up to the render settings.
[22:10] And then in terms of my device, I'm using GPU.
[22:14] The only reason I'm using CPU is because this video will crash if I use GPU.
[22:18] So I need to set this to GPU.
[22:20] So I need to set this to CPU for video purposes only, but I'm using a GPU for normal rendering.
[22:26] And GPU rendering is stupidly fast.
[22:28] This whole character in full HD will take around a minute and a half to render.
[22:34] And I have a four year old mid-sized GPU.
[22:37] So if you have a new beasted GPU, this is done in like 30 seconds or so.
[22:42] In terms of the sample sort of viewport, this is usually set quite a lot higher.
[22:46] Again, this is to make sure that my video doesn't crash.
[22:49] But setting this to something like 500 is going to look quite nice.
[22:51] You don't want it to go all the way because then it's just going to keep on computing all the time.
[22:55] But you want this to look similar to what the final render is going to be like.
[22:59] I don't use denoising for the viewport rendering.
[23:04] And the reason is that there's so much texture in this character.
[23:09] And the denoising, if you just enable this one, is just going to remove a lot of that texture.
[23:13] It has to keep going for a while to see that.
[23:15] So in this case, I actually far prefer having more noise in my render,
[23:20] but seeing the texture instead of having something that's super clean but without texture.
[23:24] So if you look at like, for instance, this area here now, it looks really bland.
[23:28] It looks perfect in terms of noise, but it looks way too stylized.
[23:31] So if I disable denoising, you can see that, yes, it's noisier,
[23:36] but it's more true to what it's actually going to look like.
[23:40] And then for the final render settings, I set the noise threshold to 0.01.
[23:45] And max samples to a high number.
[23:49] Specifically what this number is, it doesn't matter a whole lot.
[23:52] I found that around 1500 to 2000 is a good number for me.
[23:56] The reason this number is so high is first, you have subsurface, which requires a lot of samples.
[24:02] Subsurface is very heavy sample.
[24:04] The second reason is that we are using area lights that are also very hungry for samples
[24:08] because the shadows are so soft.
[24:10] And the third and most important reason is simply that we're using depth of field.
[24:14] And depth of field is very hungry for samples.
[24:16] You don't want noise in your depth of field.
[24:19] I guess technically, depth of field will be the sharp part, but colloquially,
[24:23] depth of field would just be the blurry part.
[24:26] So essentially, my approach to this is just set it to a number where you don't have noise.
[24:31] Honestly, you can't really optimize this scene too much when it comes to this.
[24:35] Like the render settings off today are really simple.
[24:38] It's basically what are your samples?
[24:40] So essentially, you're just talking about what is the acceptable noise amount you want.
[24:44] And my acceptable noise is none.
[24:46] So my approach is set it to a high number, let it render until there is no more noise.
[24:50] I just go have a cup of tea or something and then I just come back.
[24:53] For this, I do actually denoise it, but I denoise just the final, final pixels,
[24:59] meaning that it will just do its thing and remove as much noise as it can.
[25:04] And then I'm using a denoise just at the very end.
[25:06] I've also found it to be important to use the optics denoiser.
[25:09] I found this to be the most stable and far the fastest.
[25:11] And then once you're done, you simply render.
[25:14] So I'm just going to do a render of this.
[25:15] I'm just going to set this to GPU, pulse the video and get back to that.
[25:20] And that's it for this whole video.
[25:22] This is the final result of the character, which we just shaded and lit in this video.
[25:28] The important part is that you have a really good scope before you really start texturing.
[25:32] And once you are texturing, you need to go back and forth constantly between your shading
[25:38] software, in this case, Blender, and then your texturing software.
[25:41] If not, you're flying entirely blind and you really have no idea what you're actually doing.
[25:46] So go back and forth constantly between the two software and adjust the values.
[25:51] I also tend to take these kind of renders into Photoshop and doing like global changes to it.
[25:56] And that's one of the reasons why these edges now are nice and orange.
[25:59] They used to be more red, but I did a huge shift in Photoshop on them and thought that
[26:02] it would cool. And then I did those changes back in painter.
[26:05] And it means that the setup is really nice and simple in terms of the shaders.
[26:10] In terms of skin shading in Blender, make sure to use the random walk fixed
[26:14] radius and use a mixed RGB node for the radius as well.
[26:19] If you're interested in more content like this as well, I highly recommend our


### Realistic Character Portrait Masterclass [26:20]
**Transcript (timestamped):**
[26:22] realistic character Port for Masterclass.
[26:24] This is where we're making this character here from scratch.
[26:27] It's using the exact same workflow from these videos, the three videos we have
[26:31] on the clicker where we are sculpting a sea brush, where we're apologizing in Blender,
[26:36] UV mapping in Blender and going back and forth between painter and Blender to develop
[26:42] the look and finally rendering the whole thing in Blender.
[26:45] Where we also doing hair and fur as well for the eyebrows.
[26:50] So I highly recommend this full course as well.
[26:53] It's about 21 hours long and we go through all the steps in real time.
[26:57] So if you enjoyed this series of YouTube videos, I'm sure you're going to enjoy
[27:00] this course as well.
[27:01] It's taught by myself and the style is very similar to that.
[27:04] So yeah, that's it for this video.
[27:06] So make sure to like, comment and subscribe and we'll see you in the next video.



---

## Captured Frames

- [0:35] tutorials/frames/shading-lighting-a-character---blender-and-substance-3d-painter-workflow/frame_000.jpg
- [1:05] tutorials/frames/shading-lighting-a-character---blender-and-substance-3d-painter-workflow/frame_001.jpg

---

## Structured Notes

### Core Technique
Note: this is a cross-platform (Blender + Substance 3D Painter) shading/lighting/rendering video, the direct sequel to this creator's "Texturing a Clicker" video. The vast majority of runtime (Cycles shader-node setup, three-point lighting, depth-of-field, render settings) is Blender-side and outside this skill's stated scope; per this ingest's instructions, Painter-side content is kept primary below and the Blender portion is summarized only briefly for pipeline context. **The one Painter-specific principle worth extracting in depth is the "texture maps as final / texturing software as master" workflow rule:** any color/roughness correction discovered while look-developing in the shading/rendering software must be reproduced back in Painter on the actual Fill-layer/map data and re-exported, never left as a permanent non-destructive adjustment inside the shading network — keeping the render setup simple and keeping one single, portable source of truth for the character's look.

### Summary
Picks up exactly where the companion texturing video left off: the finished Painter project exports down to just **two texture maps per texture set — Base Color and Roughness** — deliberately minimal because high-frequency surface detail (pores, fine wrinkles) was already baked in from a well-developed ZBrush sculpt rather than painted as height/normal detail, and because the render uses an even-higher-decimation mesh brought directly into Blender rather than relying on Painter-side normal maps for extra detail. UV Tiles/UDIMs are used (multiple tiles per texture set, visible in the Texture Set List), reflecting the same multi-part organization (head, mushrooms, teeth, tongue) from the companion texturing video. Once in Blender, the core Painter-relevant discipline is: bring the exported Base Color and Roughness maps in as Image Texture nodes (Roughness map's color space explicitly changed to **Generic Data**, i.e. non-color, appropriate for AgX color management — the setting differs depending on whether the project uses Filmic, AgX, or no LUT at all), wire Base Color into both the shader's Base Color and (via a Mix RGB node used purely as a color-picker convenience, Fac=0) the Subsurface Radius input, and treat any further Roughness remapping through a **Map Range** node rather than editing the source map. Critically, whenever a color-correction need is discovered during Blender look-dev (the video's own example: pushing edge colors from red toward a "cooler"/orange shift after seeing a Photoshop-graded test render), that correction is **reproduced directly on the Fill-layer colors back in Substance Painter**, the maps re-exported, and any temporary Blender-side color-correction nodes deleted — explicitly to avoid the "which one do I edit now" ambiguity of having color decisions split across two pieces of software. The video closes reiterating the same iterative-feedback loop theme as the companion texturing video: texture and shading/lighting decisions are "highly interconnected" (subsurface intensity changes what the correct light intensity looks like, and vice versa) and must be developed by constantly cycling between the texturing software and the shading/rendering software rather than finishing one in isolation before starting the other.

### Key Steps
1. **Keep the final Painter export minimal and purposeful:** for a well-sculpted character, export only what's actually needed downstream — here just Base Color and Roughness per texture set — rather than exporting every possible channel by default; fine surface detail sourced from sculpt/decimation quality doesn't need a redundant normal/height map if the render mesh itself already carries that resolution.
2. **Treat the texturing software as the single master for any color/value data.** When a shading-software look-dev session (Blender, Arnold, or any renderer) reveals that a color needs to shift, do NOT leave that as a permanent hue/saturation or color-correction node in the shader graph — reproduce the exact same adjustment on the actual Fill-layer colors back in Painter, re-export the maps, and delete the temporary shader-side correction nodes. This keeps exactly one place to look for "what color is this material" and avoids the shader network becoming an undocumented second source of truth.
3. **Set scalar/data maps (Roughness, and similarly any mask/utility map) to a non-color/"Generic Data" color-space setting** in the shading software when importing Painter's exported maps — required when using AgX (or any view-transform LUT) so the renderer doesn't apply display gamma/LUT transforms to numeric data that isn't meant to be viewed as a color.
4. **For subsurface scattering setups, prefer feeding the shader's Base Color output into the Subsurface Radius input through a Mix RGB node (Fac locked to 0) used purely as a manual color/value picker**, rather than tuning per-channel RGB subsurface radius numbers directly — makes the subsurface hue and intensity adjustable by eye instead of by math, with the Mix node's color controlling hue and its value/brightness controlling the overall SSS strength.
5. **Iterate constantly between texturing and shading/lighting software rather than finishing one before starting the other** — SSS intensity, roughness values, and light intensity are described as "highly interconnected": a change in one invalidates assumptions baked into the other, so texture-then-shade-then-light as strictly sequential phases will fly blind.

### Layers / Tools / Settings (Painter-relevant only)
- **Final export:** Base Color + Roughness only, per texture set, UV Tiles/UDIMs
- **Cross-software color discipline:** any color correction discovered downstream gets reproduced on Painter's actual Fill-layer color values and re-exported — never left as a permanent shader-graph adjustment
- **Color space on import (Blender side, for context):** Roughness/scalar maps set to Generic Data (non-color) when using AgX or Filmic view transforms
- *(Out of this skill's scope, summarized only: Blender Cycles shader-node SSS setup via Mix RGB + Random Walk Fixed Radius, three-point lighting with a light-blocker card, camera-locking, depth-of-field via an Empty + F-stop, and Cycles render/denoise settings.)*

### Difficulty
Advanced — the Painter-relevant portion is conceptually simple (a discipline/workflow rule, not a specific tool sequence), but assumes the reader already has a finished, well-organized Painter project (per the companion texturing video) and is comfortable working across a texturing-to-rendering pipeline rather than treating Painter as a standalone destination.

### App & Version
Not stated numerically on screen for Painter. UV Tiles/UDIMs visible in the Texture Set List (same project as the companion texturing video). Blender-side uses the AgX color-management LUT (described as then-newer than Filmic) and Cycles — useful pipeline context but not a Painter version marker.

### Tags
texture-set, uv, udim, basecolor, roughness, color-management, export, export-preset, pbr, advanced

---

## Related Tutorials
- [Texturing a Clicker - FULL Substance 3D Painter Workflow](texturing-a-clicker---full-substance-3d-painter-workflow.md) — same creator (FlippedNormals), same character/project, direct prequel — that video covers the full Painter-side texturing build (channel-separated groups, procedural+hand-painted hybrid materials, AO-hand-correction-then-Curvature-then-Levels mask chain) that this video's Base-Color+Roughness export is the output of; the "reproduce color corrections back in the source software" principle here directly extends that video's live Fill-layer color-editing workflow.
