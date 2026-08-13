---
title: Optimizing Textures - How to Pack Masks Like a Pro
source: YouTube
url: https://www.youtube.com/watch?v=yZA_QMeZU0Q
author: Abe Leal 3D
ingested: 2026-08-13
app: "Substance 3D Painter (channel packing/export) + Unreal Engine 5 (material graph reconstruction)"
version: "not stated on screen"
tags: [texture-set, channel-packing, export, export-preset, basecolor, roughness, metallic, normal-map, ambient-occlusion, curvature, thickness, height, alpha, masks, generator, procedural, blend-mode, game-engine, unreal-export, color-management, advanced, expert]
extraction_status: complete
frames_dir: tutorials/frames/optimizing-textures---how-to-pack-masks-like-a-pro/
frame_count: 12
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Optimizing Textures - How to Pack Masks Like a Pro

**Source:** [YouTube](https://www.youtube.com/watch?v=yZA_QMeZU0Q)
**Author:** Abe Leal 3D
**Duration:** 23m14s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hello everyone and welcome to a very special video. Now, this video, I'm gonna warn you, it's a little bit technical, but trust me, if you spend the time learning what I'm about to show you, your knowledge and understanding about textures and engines is going to exponentially grow.
[0:14] What we're going to be doing today is I'm going to show you how to build this very simple network that's going to allow us to further optimize our textures. We're only going to be using two textures in our asset and not only that, but we're actually going to be building a very simple mask that we can
[0:27] parametrically control to add a blood to our shield. All of this, we're going to talk from substance into Unreal and all of the integration you need to get this very cool result right here. So let's go.
[0:39] Very well, my friends. So let's start with the technical side of things. And as I mentioned in the intro, it's a little bit technical, but it's easy. It's easy. You guys are going to be able to follow. So as you guys know, normally, when we export our maps, we're going to have four very important maps. We're going to have, of course, the base color, which is going to represent the color of the object. We're going to have our, in this case, roughness
[0:57] map, which tells us what parts shine a little bit more than others. We're going to have our metallic map very important to describe different types of surfaces. We're going to have our normal map right here. And finally, we're going to have sometimes the ambient occlusion, right? So usually when we export, let's say we go here, file export textures and we select a preset like, for instance, the traditional PBR metallic roughness on our list of experts, we're going to have all of this maps right here. Base color, emissive, height, metallic, normal roughness. Usually we're going to only need four of them, right? Base color, metallic, normal and roughness. If you have emissive, of course, you're going to have a lot of roughness.
[1:27] You're going to need it as well. If you have height and you want to use like displacement, you're also going to use it. But as you can see, it's a lot of maps and all of this maps are not our 4k maps. So you can imagine how this can exponentially increase. This is just one asset. Imagine a scene where we have, I don't know, 200 assets. Every single one of those 200 assets is going to have like massive amounts of data.
[1:43] So one of the things that we can do, and this is level one of optimization, is use the Unreal Engine 4 packed right here or Unreal Engine pack right here. If we take a look at the list of experts, something very interesting is happening. And this is again where the technical set of things starts to
[1:57] occur. So what is happening is we are removing a lot of the maps and we're mixing them in a single map right here, the occlusion roughness metallic map. Now, if you've already seen this, trust me, trust me, in just a couple of minutes, I'm going to show you something that blew my mind when I learned this. So if we go to the output templates and we go to the Unreal Engine pack right here, you're going to see what that what they're
[2:15] doing is they're utilizing or inputting all of these maps in specific slots of your image. Normally, an image that has an alpha channel such as Targus, which by the way, are the best maps that you can use for exporting textures to games are going to have four slots, right?
[2:27] RGB and a so when you have those four slots, we can decide where all of these elements are going to go and look at how many elements we can actually export as part of the substance precess, right? So in the normal Unreal Engine pack, we have the base color and we have the opacity on the alpha
[2:42] channel. We don't have any opacity right now. So we don't need that. We also have the metallic roughness occlusion right here. We have the normal map and we have the MS. This is where the magic starts. We can export this and I've talked about this before. You can check any of the other videos on how to connect this one's right here inside the front real. But this is where the magic starts.
[2:57] I'm actually going to duplicate this guy right here. And over here, I'm going to call this Unreal Engine packed, I don't know, min max, let's call it min max. And when we do this, if we go here, we can actually start removing some of these elements and further crunch the amount of maps that we're going to get. So if your assets not going to have a MISI and most of the time when doing fantasy stuff, you're not going to have a MISI, we can just remove that. That's one map gone. But we still have three, four K maps. Can we reduce this further? And the answer is yes. So the base color we're going to keep. So that one stays exactly there.
[3:27] The metallic roughness metallic gone. We don't need it anymore. And this normal map right here, we're actually going to delete it as well, because we're going to recreate it with a new R plus G plus B plus A. So what this does when I click on this button is it gives me a new map right there that allows me to plug individual channels to the elements. And this is where the little trick happens, the little magic, the normal map information inside the front real engine and also inside the father software.
[3:51] But more easily inside the front real engine doesn't actually need the blue channel. We can recreate that blue channel in engine without having to save it on a blue channel here inside of substance. So what I'm going to do is I'm just going to grab normal direct X, drop that into the R channel, hit R, grab normal direct X again, drop it into the green channel, hit G.
[4:10] And there we go. Now we have two new channels empty right here, B and A. So what can we input here on the blue and the alpha? Of course, we're going to go for roughness in this case on the blue channel, right? Make sure it's just like great channel right there. And we're going to grab metallic right here on the alpha channel. Again, just click on great channel. Do not click on alpha channel because it's going to do a separate thing. It's going to add transparency. You want to keep it as a great channel. So now we have this single texture that has the normal map information. It has the metallic information and the roughness information.
[4:40] Saving us one full extra texture that we are not going to need inside of the engine. Now here's where the fun begins or we can have a fun little thing. As you can see right now, we have the opacity on the grayscale channel, which is fine. Opacity is a good map, but in this case we don't need it. So what could we use instead of opacity? Of course, we can just grab ambient occlusion and do the exact same thing. Say that's a great channel. And now we're going to be exporting the ambient occlusion channel in case you want it.
[5:04] But keep in mind, the ambient occlusion is just a multiply to make things a little bit crunchier. Nowadays with things like a screen space ambient occlusion or the automatic ambient occlusion that we get inside of the engines, you don't really need it as much. So I want to use this channel with a custom channel, a custom texture that we can then utilize inside of the engine. So let's close this for just a second. And let's imagine that this shield is going to have a version of the texture where there's going to be a lot of blood in it, right? Like you fight for a couple of seconds with the enemy, you get hit like a couple of times, and now your whole armor is very bloody.
[5:34] We see this quite a bit in games like Expedition 33, right? Like the more you fight, the more you get damaged, the more blood starts like appearing on your skin. So one of the things that you can do here is very simple. First, we need a custom channel. Because remember, we're exporting the basic channels that we know here. Well, we need to create our own like blood mask or blood channel. And we're going to do that by going here to texture set settings, creating a new level, my right here, new channel and going all the way down to user channels. And I'm going to create this user zero. That's it. User zero is going to be my blood channel. If you want to change the name, you can. You can just call it blood, but it's not going to be a new channel.
[6:04] And that showed like this in the texture set list. Don't worry. And over here, we just need to create a new mask. Now I do recommend doing one thing. I'm going to go all the way to the bottom, create a fill layer. This fill layer is going to be the blood channel. As you can see right there, all the way to the bottom. And now I'm going to create the main mask on the top.
[6:19] So I'm going to create a new fill layer here. I am going to keep color on for just a second. I'm going to turn blood on as well, all the way to one. And on the blood, let's select, you know, like a dark red color, something like that. And what I can do is I can just add, let's say a black mask. There we go.
[6:31] Let's add, I don't know, like a feel layer. Let's look for an interesting grunge map, something like this right here. There you go. I look like blood splatters. Let's make them a little bit more big, something like that. And then, you know, to sort of like break it down a little bit, let's say we add a generator. Let's add.
[6:47] Yeah, let's do a third generator. And what I'm going to do is I'm going to flip it. And then I'm going to multiply this. As you can see, it's removing the blood from the crevices and it's keeping the blood on like the other parts. We can do other things. For instance, let's do another fill layer. And now let's do, for instance, say,
[7:01] grunge map like this one right here. And we're also going to multiply this one right there. Awesome. So as you can see now with those two masks right there, we're able to create a very, very interesting like blood approach. And if we press letter C, we can actually see what is going on over on the top side right here. You're going to go to, you're going to see that we can access the blood channel right there. So this right here is my blood mask. It's a procedural generated mask that shows with all of this blood right here. Does it look like the blood that we want to see in game? Not necessarily. This is something that we are going to have to do in engine to properly calibrate all of the blood.
[7:31] The colors, but the important thing is that we have this mask. And now the only thing I need to do is go back to the export textures, go back to my output template, my Unreal Engine, min max right here. And over here, instead of using this in P interlusion, I'm going to look for user zero and user zero now goes into my great channel.
[7:49] So that mask that we just created that blood mask is something that we can export. Now, let's say we want to use as many masks as possible inside of the engine.
[7:56] And we want to give our technical artists or the shader artists as much like a range to play with different things. We can always export a new one right here. Let's select all of this. I'm going to call this map something like masks.
[8:07] Okay. And let's give him, let's give our artists all of this information. Let's say we give them an ambient occlusion. We're going to give them the thickness map. Maybe they use that for something. We're going to give them the curvature map as well. There you go. Great channel.
[8:20] And whatever, let's say we're going to give them something like the height map as well. Right. So as you can see, I've now created a new costume texture that holds a lot of information that can be used for further look development inside a bunch of engines.
[8:33] This, by the way, is not only applicable to our real engine, you can use this masks inside of Maya inside of Blender inside of any element or software that allows you to do like crazy fancy stuff with shaders. Well, you can use this information.
[8:44] Now, for this particular example, I'm not going to use it. I'm going to just remove that map, but I'm just giving you the options guys, I'm giving you the tools so that if you are ever in the production where you need to have all of this available information, packing it this way is an excellent way to optimize your texture size.
[8:57] Now, let's go back here to settings. Let's select our real engine min max right here. Very important. What is the best textures type that we can use target? Why target because target is a lossless format. It's not going to lose any information.
[9:08] And very importantly, it's going to keep the alpha channel as a separate channel, right? So you're going to have four little slots are GB plus a to have that information. If you export in PNG, which is also very good. Just keep in mind that the alpha channel gets multiplied by the colors.
[9:21] So you get a different approach and it might not work exactly like you would expect. It's also not like you're not going to lose a lot of like quality under compression like PNG is really good. But if you're using alpha channels, I strongly recommend target.
[9:32] I'm going to create a folder called min max right here and let's select the folder and just export. And the beauty about this is look at this. Just two textures, just two. Yes, they're 4k. So they're going to be a little bit big, right? But we optimize the size by just having two textures right here with all of the necessary information that we need for the different channels.
[9:48] Keep in mind, again, yes, this are 128 megabytes. So eight, this are big, big textures because every single channel is being occupied. So there's a lot of information in them. But it's a very good way to optimize some of the processes later on.
[9:58] Now, of course, the big question is, well, how are we going to rebuild this material so that it works properly inside the front real? We're inside the scene. If you haven't seen it, we did a long little video about this a couple of weeks ago where I show how to do a quick presentation here inside the front real. And the only thing we're going to do is of course, bring in our elements. So I'm going to create a new folder here. It's called this shield, bring in the textures and of course bring in the shield. Let's get rid of our little demon guy right here for a second. Now that we have the shield here on the scene, we of course need to start building the element. Now I do want to mention something. This is a small little tidbit of information.
[10:28] It's not something that you're going to use all the time, but I learned this very recently during GDC actually, and it really surprised me. And that's the fact that by default, if we go here to the images, you're going to see that images are compressed using this thing called the default TXT one BC one compression method.
[10:42] And it's a really good compression method. It's going to keep things like very optimized, but there is going to be a little bit of like pixel artifacts happening even at a 4k like texture right here.
[10:51] So let me know if you can see the difference, but I'm going to switch this to BC seven and BC seven. As you can see, it's going to give us a clearer look, something that's a lot cleaner and a lot closer to what we had in substance painter.
[11:02] Now, is this something that you always need to do? Not really. But if you really want to have like the best possible quality, changing the compression setting to PC seven is it's a good option.
[11:10] Don't do this without asking your lead or your client to please you don't want to make the whole thing like bigger because this does increase the performance a little bit.
[11:17] But it's a good way, especially for presentation purposes to have that at BC seven.
[11:20] Now, of course, we're going to go and create a material. I'm going to call this material M underscore shield, and we're going to go here instead of shield drag this thing right here.
[11:27] I'm not sure if I mentioned this, but if I haven't make sure that this normal map information has no sRGB.
[11:32] That's very, very important because we don't want to have any sort of like color correction being applied to it.
[11:36] And we just drag and drop this one right here. As you can see, if I select this texture sample, you're going to see this is set to linear color.
[11:42] Very, very important.
[11:43] Now, quick little tip. If you select your mesh on your outliner or your content browser and you click on this little brick thing right here, it's going to import the model.
[11:50] So that you're going to be able to to see what's going on.
[11:53] And it's just a good way to better see our textures. Right.
[11:55] So there we go.
[11:57] Now, of course, color is going to go into color right here.
[12:00] And of course, we still have the blood information here on the alpha channel, but we're not going to use it yet.
[12:04] We're going to first rebuild our normal and this is where we do need to do a little bit of math.
[12:10] So the big question here is, why can we reconstruct the blue channel from the red and green channel?
[12:16] And the answer is again, math.
[12:18] The information that we need to get for the blue channel comes from this two channels using a little bit of math.
[12:23] And this is the formula right here.
[12:25] I know it looks fancy. It scares me.
[12:26] I'm not a math guy.
[12:27] So anytime I see this sort of like crazy little things, I know for some people it's like, oh, yeah, that's easy.
[12:32] But for me, it's always like, oh, my God, what is this?
[12:34] It's very simple.
[12:35] Almost any software is going to allow you to do this.
[12:37] And it's very, very simple here.
[12:39] Let me show you.
[12:39] First thing we need to do is we need to mix together these two vectors.
[12:43] So I'm going to append the red channel and the blue channel.
[12:46] OK, so we're going to combine red and green into this append element.
[12:50] With this append element, we are going to first subtract a specific amount from this one.
[12:55] And what we want to subtract is we want to subtract point five.
[12:59] So it's minus point five.
[13:00] We're subtracting point five in the value of these two elements.
[13:04] Then we're going to multiply all of this by two.
[13:07] And that pretty much prepares this two vectors, the R and G vector to be able to properly generate the C channel or the blue channel.
[13:15] And the thing we're going to use these days, very specific note that Unreal has, which is called the arrive normal C.
[13:20] So as you can see, it's expecting to receive the in of X and Y, right?
[13:25] Red and green.
[13:25] Remember, anytime you see RGV, that's X, Y, C.
[13:28] It's the exact same thing for most of the time.
[13:30] So what we're going to do here is we're going to plug this in.
[13:32] And if we were to plug this into the normal map information, boom, there we go, guys.
[13:36] As you can see, the normal map has successfully been rebuilt with all of the three channels that we need to get all of the bump information that we have inside of substance.
[13:46] This is almost magic to me.
[13:48] But at the end of the day, it's just math, right?
[13:51] So that's it.
[13:51] And some of you might be wondering, well, why can't we not just use that derive normal Z, that you just show me and just plug this to end and get that into the normal map?
[14:00] Because as you can see, it's not going to work.
[14:01] The data, the information, the channels are not properly calibrated because of this, like math things that we need to do, this subtraction and this multiplication in order to properly derive the information for the normal C.
[14:12] So you do need these two nodes right here.
[14:14] Now, I do want to give a huge shout out to Ponky, who helped us troubleshoot this during the last livestream.
[14:20] So the only piece that I was missing was this one right here.
[14:22] And he later shared privately on the DM that there's another node that we can use called constant bias scale.
[14:28] If we use a constant bias scale, we can do the exact same thing.
[14:31] We just set the bias to minus point five.
[14:34] This is the subtraction that we're doing.
[14:36] And we see the scale to two.
[14:37] If we do that stuff right there and we eliminate this guy's right here, we can simplify the amount of nodes that we need.
[14:43] And we can just get this in here with the exact same result.
[14:46] All of the information is going to be there.
[14:48] This, my friends, is the magic of just having R and G for our normal map, reconstructing this here inside of Unreal and then using these two next maps, right?
[14:57] B was roughness, if you remember, and Alpha was metallic.
[15:00] So by doing that, now we've successfully rebuilt the exact same textures that we have inside of Substance, but now, of course, here inside of Unreal.
[15:09] Let's save this real quick.
[15:10] Go here and just drag and drop this into our shield and look at that.
[15:14] Beautiful textures, beautiful shading.
[15:16] Everything is working exactly as intended.
[15:19] And this is going to run perfectly fine inside of our games.
[15:22] Now, I made a little mistake right here, as you can probably tell.
[15:24] I kept the blood on.
[15:26] So the blood splatters are on.
[15:27] Let me show you now the blood stuff.
[15:28] How can we add this blood stuff inside the material to quickly toggle it on and off?
[15:33] Now, before we continue, I know you guys are not subscribed.
[15:36] We have the information.
[15:38] So if you like this video and you're learning, which is the most important thing, please subscribe to the channel.
[15:42] It really helps us out.
[15:43] And let's continue.
[15:44] So first of all, of course, we need to go back here to Substance.
[15:46] I'm going to go to this channel and just turn off the color channel.
[15:49] So again, if I turn off the color channel, the blood splatters are no longer going to be there, but the blood channel is still there.
[15:54] If we go back to our export textures, we should be using our Unreal Engine Minimax.
[15:58] Same elements, same everything we can just export.
[16:00] Go back to Unreal, just like this guy right here and Reimport.
[16:03] And if we do that, the blood splatters should disappear.
[16:06] There you go.
[16:06] And we're back to having the exact same shield that we would expect.
[16:09] Now, how can we use that as a mask?
[16:11] Well, if we go to the material right here, we can create a three-vector.
[16:15] So I'm going to press three and click on the channel.
[16:17] This is going to be my blood element.
[16:19] So it's going to be like this dark blood right here, something like that.
[16:22] And what we can do is do something called a LERP, linear interpolation, which is literally going to be A over B.
[16:27] Like we're not blending, we're not doing any sort of like overlay or anything like that.
[16:30] It's just placing this thing on top of the existing texture.
[16:33] So this one right here is going to be my A and this one right here, the color is of course going to be my B.
[16:39] And the alpha, what we're going to be using to blend is of course going to be the alpha channel that we stored from that blood like mask that we created.
[16:46] If we now plug this into base color, we get this.
[16:48] We have a little bit of an issue.
[16:50] What's the issue?
[16:50] Well, this is actually inverted.
[16:51] No big deal.
[16:52] In this case, I can just use a one minus one minus is a way to just like flip a color here.
[16:57] So there we go.
[16:58] And that's that's it.
[16:59] As you can see, now we have the blood on top of the shield.
[17:02] If we want to darken this a little bit more, I can go over here and for instance, like just lower the value quite, quite a bit, something like that to make the blood look a lot more dark.
[17:11] There we go.
[17:11] Now a question that I'm sure we're going to get is, okay, cool.
[17:14] Yeah, we're adding that color on top, but it doesn't look like, you know, glossy like elements.
[17:17] How can we do that?
[17:18] Well, that's the beauty of this.
[17:19] If you know how to deal with shaders, you can get so much information out of them.
[17:23] And one of that information is understanding, well, if I have the roughness coming here from the blue channel, the only thing I need to do is I need to find a way to add this element right here and make it so that the new roughness of this blood splatter gets combined with the other roughness that we have.
[17:40] Let's do that.
[17:40] The solution here is very simple, but again, it requires math.
[17:44] Just very simple understanding of how this black and white values are affecting the way we can build our textures.
[17:49] Okay, so let's do a quick comparison here.
[17:52] If I right click this guy right here and I say, start previewing note.
[17:55] This is what we want.
[17:56] This is the mask that I need.
[17:57] I need the blood spots, as you can see, to be very dark because the darker they are, the more shiny they're going to be, the more glossy they're going to be.
[18:04] And I just want to keep those right.
[18:06] We cannot multiply because if we multiply, we get a different result.
[18:09] So we need to use a different note.
[18:10] And in this case, the note that we're going to be using is called a men note.
[18:13] What the men note does is he tries to keep the minimum information from one of the layers.
[18:18] So the blue channel, which remember is a roughness, is going to go into the A slot.
[18:22] And this max that we have right here is going to go into the B slot.
[18:25] If we now preview this thing, look at what we have right here.
[18:28] We have the exact same layer, the exact same roughness that we had before.
[18:32] And now we are only adding this black spots on top, right?
[18:36] Again, coming from the mask.
[18:37] Can you guys understand how important masks are now?
[18:39] Because we can control this thing in engine.
[18:42] We don't have to go back to the substance to change as an export.
[18:45] Another set, we are doing this all inside of the engine and almost, almost in real time.
[18:49] Now, if you don't believe me that this is doing what it's supposed to be doing,
[18:52] here's what we're going to do.
[18:53] I'm going to double click right here, right click this little note and say,
[18:56] start previewing note.
[18:57] And this is our normal roughness material.
[18:59] As you can see, it's all of the exact same values.
[19:01] If we go now to the men and start previewing this note, as you can see,
[19:04] the only thing that is changing is this black spots are being added on top of that texture.
[19:08] So now, of course, let's stop previewing this thing.
[19:11] If we take a look at the shield right now, everything looks like wrong.
[19:13] Actually, let me like plug this in just like the roughness.
[19:16] As you can see, this looks good.
[19:18] It's the way it's supposed to be looking, right?
[19:19] But we don't have the blood.
[19:20] Well, actually, we do have the blood, but it's not changing anything on the glossiness.
[19:23] If we now plug this into the roughness, boom.
[19:26] Now, the blood actually shines and we can see the reflection of the light
[19:30] as it passes through the blood, right?
[19:32] Making this little blood mass that we procedureally created
[19:35] instead of substance available to us inside of the engine.
[19:38] I'm going to go one step further.
[19:39] And I know this is, you know, a little bit too much for some of you.
[19:42] If this is the first time you're getting into shaders and stuff, but it's really,
[19:45] really cool. And this is the fact that we can now create something to blend this thing.
[19:49] Right. So now the question is, how can we blend it so that we have just one little guy
[19:53] that controls whether we see the blood or not? Can we do that?
[19:56] The answer, of course, is yes.
[19:57] Now, I'm going to preface this by saying there's multiple ways to do it.
[20:00] And this is just one way to do it.
[20:01] It might not be the most efficient or, you know, performance oriented,
[20:04] but it's going to work.
[20:05] I'm going to use another lerp right here.
[20:07] And what I want to learn or what I want to sort of like go from one point to
[20:10] another is of course the original color right here and the color plus the blood.
[20:14] And this is going to go into my base color.
[20:16] So if the alpha of this thing is set to zero, we're going to see no blood.
[20:20] If the alpha of this thing is set to one, we're going to see blood.
[20:23] And we can do the exact same thing with the roughness.
[20:25] I can create another lerp right here.
[20:27] The original roughness goes into a, the new roughness goes into B.
[20:31] And the result of the both of those goes into that guy right there.
[20:34] And the alpha again, if this alpha set to zero, there's no roughness.
[20:38] And if this alpha is set to one, we have the blood plus the roughness.
[20:41] So it's going to be glossy and nice, right?
[20:43] With the shader.
[20:43] So everything's going to be working fine.
[20:45] And finally, I'm going to press number one, and I'm going to create this little
[20:48] guy right here, right click and convert this to a parameter.
[20:51] I'm going to call this blood.
[20:52] So now this parameter is going to control the alpha of both of this little sliders.
[20:57] One of them is the color.
[20:58] One of them is a roughness.
[20:59] If this value changes, right?
[21:01] If this value changes, the blood is going to appear.
[21:04] So if I go here, the slider max is going to be one, the final value is going to be
[21:07] zero and I'm going to save this thing right here.
[21:10] Now, in order to actually be able to modify it, I'm actually going to have to go
[21:13] here to the material, right click and create a material instance.
[21:17] Go to the shield or the shield right here, drop the material instance.
[21:20] And if I double click the material instance, what you guys are going to see is
[21:23] that we're going to have some controllers over here.
[21:25] We have this global scalar parameter value that I can just activate.
[21:29] And anytime I push this up, blood is going to appear on the shield.
[21:33] Look at that beautiful thing right there.
[21:34] So as I push this parameter up, blood appears as I push this parameter down,
[21:39] blood disappears.
[21:40] So dynamically, because you can control this through blueprints later on, right?
[21:43] Like with gameplay, dynamically, we can add and remove this blood by using the
[21:47] power of masks and instant materials and layers and of course math.
[21:52] That's pretty much it, guys.
[21:53] If you want to learn a little bit more about this, like parametric values that we can
[21:56] control in order to build like custom materials and custom shaders.
[21:59] Let me know here in the comments and either we do a video here for the channel
[22:02] or we'll talk about this during one of our live streams.
[22:04] But this is sort of like the next level.
[22:06] If you're a character artist, if you're a textural artist, if you do props,
[22:09] if you do environments, this is one of those things that can really separate you
[22:13] from a lot of other people out there who don't know how to control all of the
[22:16] amazing things that they model and texture inside of the engine, which is where
[22:20] it matters the most, right?
[22:21] Because this is what the players are going to be experiencing.
[22:23] So yeah, that's pretty much it, my friends.
[22:25] This is the end of the road right here.
[22:28] And hopefully you like not only the optimizations things that we did in substance,
[22:31] but also the little math that we talked about here inside of Unreal to get this to work.
[22:36] I have nothing else to say for now, except thank you.
[22:38] Thank you very much, everyone, for your support.
[22:39] If you find this content useful, please don't forget to subscribe.
[22:43] It really helps the channel.
[22:43] We're really close to our next milestone.
[22:45] I never thought we're going to get as close to 100k as we are now.
[22:48] And now it feels like it's just within reach.
[22:50] I know it's just like a, you know, like an insignificant number.
[22:53] It really doesn't matter as much.
[22:54] But it's one of those like interesting things for a YouTube channel, right?
[22:57] So thank you, everyone, for your support.
[22:59] And hopefully all of this information is helping you in your 3D journey.
[23:02] That's it for me.
[23:03] Don't forget, always learning, always improving.
[23:06] I will see you back on the next one.



---

## Captured Frames

- [1:50] tutorials/frames/optimizing-textures---how-to-pack-masks-like-a-pro/frame_000.jpg
- [3:15] tutorials/frames/optimizing-textures---how-to-pack-masks-like-a-pro/frame_001.jpg
- [4:00] tutorials/frames/optimizing-textures---how-to-pack-masks-like-a-pro/frame_002.jpg
- [5:50] tutorials/frames/optimizing-textures---how-to-pack-masks-like-a-pro/frame_003.jpg
- [6:55] tutorials/frames/optimizing-textures---how-to-pack-masks-like-a-pro/frame_004.jpg
- [7:35] tutorials/frames/optimizing-textures---how-to-pack-masks-like-a-pro/frame_005.jpg
- [9:35] tutorials/frames/optimizing-textures---how-to-pack-masks-like-a-pro/frame_006.jpg
- [10:50] tutorials/frames/optimizing-textures---how-to-pack-masks-like-a-pro/frame_007.jpg
- [13:00] tutorials/frames/optimizing-textures---how-to-pack-masks-like-a-pro/frame_008.jpg
- [14:40] tutorials/frames/optimizing-textures---how-to-pack-masks-like-a-pro/frame_009.jpg
- [18:25] tutorials/frames/optimizing-textures---how-to-pack-masks-like-a-pro/frame_010.jpg
- [21:15] tutorials/frames/optimizing-textures---how-to-pack-masks-like-a-pro/frame_011.jpg

---

## Structured Notes

### Core Technique
Aggressive texture-channel packing beyond the standard "Unreal Engine 4 Packed" export preset — reconstructing a normal map's Blue channel mathematically inside Unreal Engine so it never needs to be stored, freeing that map's RGBA slots for Roughness + Metallic instead, plus a custom **User Channel** ("blood" mask) built entirely from procedural generators/grunges in Painter and exported as a fourth packed channel, then reconstructed and dynamically toggled as a runtime material parameter in Unreal.

### Summary
Starts from the problem: a full default PBR export (BaseColor, Roughness, Metallic, Normal, plus optional Emissive/Height/AO) can produce many separate 4K textures per asset — at scale (e.g. 200 assets in a scene) this becomes enormous. **Level 1 optimization** is the standard **Unreal Engine 4 (Packed)** output template, which already merges Occlusion/Roughness/Metallic into one RGB image and keeps BaseColor+Opacity and Normal separate (TGA/PNG images have 4 usable slots: R, G, B, Alpha). **Level 2 (this video's real content)**: duplicate that template (e.g. "Unreal Engine Packed - Min Max"), delete unneeded maps (Emissive if not used), and — the core trick — delete the standalone Normal map output entirely and rebuild it as a custom RGBA output: Normal DirectX's X data into the R channel, Y data into the G channel (both as Greyscale channel, not Alpha channel, to avoid triggering transparency), Roughness into B, Metallic into Alpha. This works because a tangent-space normal map's Blue (Z) channel is mathematically derivable from X and Y at render time — Unreal (and most modern engines) doesn't need it stored at all. The freed Alpha slot on the BaseColor+Opacity map (since this asset has no real opacity) is instead repurposed for a **custom mask**: a **User Channel** (Texture Set Settings → Channels → + → User Channels → User0, renamed e.g. "Blood") is added to the texture set, built as its own Fill-layer-based procedural mask entirely inside Painter (a red-tinted base color for visualization purposes, driven by a black mask stack: a Grunge fill for blood-splatter shape, a Curvature-or-similar generator flipped and set to Multiply to remove blood from crevices, and a second Grunge fill on Multiply to further break up the shape) — previewable via the `C` channel-cycle hotkey. This user channel is then mapped into the custom export template's spare Alpha slot in place of Opacity. A third, fully-loaded "masks" template variant is also demonstrated (AO + Thickness + Curvature + Height all packed into one RGBA texture) as a general technique for handing technical/shader artists a rich set of look-dev channels in a single custom texture, applicable to any DCC/engine (Maya, Blender, etc.), not just Unreal — though not used in this video's final asset. **Export settings**: TGA recommended over PNG specifically when using alpha channels (PNG's alpha gets pre-multiplied into the RGB colors, changing the result; TGA is lossless and keeps alpha as a fully separate channel) — the final result for this shield asset is just **two 4K textures** instead of five-plus. **Unreal-side reconstruction**: import both textures, set the packed-normal texture's compression to a setting that preserves quality (BC7 instead of the default BC1/DXT1, visibly reducing block-compression artifacts on a 4K texture — a quality/performance tradeoff worth confirming with a lead before using broadly) and set its sRGB flag off (linear color — critical for any normal/data map). In the Material Graph: **Append** the packed texture's R and G channels into a 2-component vector, **Subtract 0.5** and **Multiply by 2** to remap the 0-1 stored range back to a -1..1 signed vector, then feed that into Unreal's **DeriveNormalZ** node (expects X/Y input, reconstructs Z) to rebuild a complete usable normal vector from just 2 stored channels — an equivalent simpler alternative uses a single **Constant Bias Scale** node (Bias = -0.5, Scale = 2) in place of the separate Subtract+Multiply nodes. The same texture's B and Alpha channels are wired directly into Roughness and Metallic respectively. The BaseColor+blood-mask texture's Alpha (the custom blood channel) is used two ways: (1) a **Lerp** between the plain BaseColor and a hand-picked dark blood color, alpha-driven by the mask (inverted with `1-x` since the mask read backwards), gives the visual blood-splatter color layer; (2) a **Min** node combining the stored Roughness (blue channel) with the blood mask makes the blood read as glossier/shinier than the surrounding rough material — verified by right-click → "Start Previewing Node" on individual graph nodes to isolate and check each step's output. Both the color-Lerp and roughness-Min results are then blended a second time via two more **Lerp** nodes (original vs. blood-modified color, and original vs. blood-modified roughness) driven by one shared **Scalar Parameter** ("Blood", 0-1 range) — converted from a constant to a parameter, then exposed and controlled live via a **Material Instance**, letting an artist (or later, gameplay Blueprint logic) dynamically fade blood damage in and out on the shield in real time without ever re-exporting from Painter.

### Key Steps
1. Understand the baseline: a full PBR export can produce 5+ separate texture maps per asset (BaseColor, Roughness, Metallic, Normal, optionally Emissive/Height/AO) — this multiplies fast across many assets in a scene.
2. Start from **Unreal Engine 4 (Packed)** output template (already merges Occlusion/Roughness/Metallic into one RGB image); duplicate it to create a custom variant (e.g. "Min Max") for further reduction.
3. Delete unneeded maps from the custom template (e.g. Emissive, if the asset doesn't use it).
4. Delete the standalone Normal map output and rebuild it as a custom RGBA channel-pack: Normal DirectX **X → R** (Greyscale channel), Normal DirectX **Y → G** (Greyscale channel), **Roughness → B**, **Metallic → Alpha** — freeing a whole separate texture, since the normal map's Blue/Z channel is mathematically re-derivable from X/Y at render time and doesn't need to be stored.
5. Repurpose the BaseColor map's now-unused Alpha slot (if the asset has no real Opacity) for a custom mask instead.
6. Add a **User Channel** (Texture Set Settings → Channels → + → User Channels → User0, rename as desired e.g. "Blood") to hold that custom mask data inside the Painter project.
7. Build the custom mask entirely with Painter's standard toolkit — Fill layer + black mask + Grunge fills for shape, a generator (e.g. curvature-based) flipped and set to **Multiply** to exclude crevices, a second Grunge on **Multiply** for further breakup — verified via the `C` channel-cycle hotkey to preview the raw mask channel.
8. Map that custom User Channel into the export template's freed Alpha slot (replacing Opacity).
9. (Optional, shown as a general technique) Build a fully-loaded secondary "masks" export template packing AO + Thickness + Curvature + Height into one RGBA texture, for handing technical/shader artists a rich look-dev toolkit in a single custom map — works in any DCC/engine, not Unreal-specific.
10. Export as **TGA** (not PNG) whenever using alpha channels — TGA is lossless and keeps alpha fully separate; PNG's alpha gets pre-multiplied into RGB, changing the stored color data.
11. In Unreal: import both packed textures; set the reconstructed-normal texture's compression to **BC7** (instead of default BC1/DXT1) for less block-compression artifacting at high resolution — a deliberate quality/file-size tradeoff, confirm with a lead before using broadly; set its **sRGB flag off** (linear color, essential for any normal/data map).
12. Rebuild the normal map in the Material Graph: **Append** the packed texture's R+G channels into a 2-component vector → **Subtract 0.5** → **Multiply by 2** (remaps 0-1 stored data back to a -1..1 signed vector) → Unreal's **DeriveNormalZ** node (reconstructs the missing Z/Blue component from X/Y) → plug into the Normal input.
13. Simplify steps 12's Subtract+Multiply pair into a single **Constant Bias Scale** node (Bias = -0.5, Scale = 2) for the same result with fewer nodes.
14. Wire the same packed texture's Blue channel into Roughness and Alpha channel into Metallic.
15. Build the blood color layer: a **Lerp** between plain BaseColor and a hand-picked dark blood color, alpha-driven by the imported blood-mask channel (invert with `1 - x` if the mask reads backwards) — plug into BaseColor.
16. Build the blood roughness layer: a **Min** node combining stored Roughness with the blood mask so blood-covered areas read glossier/shinier than the surrounding material — verify each graph node's isolated output via right-click → **Start Previewing Node**.
17. Add a second layer of Lerps (original color vs. blood-modified color; original roughness vs. blood-modified roughness), both driven by one shared **Scalar Parameter** ("Blood," range 0-1) converted from a constant — wire into final BaseColor/Roughness material inputs.
18. Create a **Material Instance** from the material to expose the Blood parameter as a live, artist- (or Blueprint-gameplay-) controllable slider that fades blood damage in/out in real time with zero re-export from Painter.

### Layers / Tools / Settings
- Painter: custom duplicated **Output Template** (Export Textures → Output Templates), per-channel RGBA remapping (drag an input map onto R/G/B/A, Greyscale vs. Alpha channel mode)
- **User Channel** (Texture Set Settings → Channels → + → User Channels)
- Custom mask built from standard Fill/mask/Grunge/generator toolkit, previewed via `C` hotkey
- Export format: **TGA** (lossless, alpha kept separate) preferred over PNG (alpha pre-multiplied into RGB) whenever alpha channels are used
- Unreal texture import: **sRGB off** for normal/data maps, **BC7** compression (vs. default BC1/DXT1) for higher quality at a size/perf cost
- Unreal Material Graph nodes: `Append`, `Subtract`, `Multiply` (or the combined `Constant Bias Scale`, Bias -0.5/Scale 2), `DeriveNormalZ`, `Lerp`, `Min`, `Component Mask`, `Scalar Parameter` (converted from constant), right-click → **Start Previewing Node** for graph debugging
- `Material Instance` (exposes a parameterized, live-editable slider from a base Material)

### Difficulty
Expert — combines advanced Painter export/channel-packing knowledge with genuine shader-graph math (tangent-space normal reconstruction, Lerp/Min-based mask compositing) inside Unreal Engine; explicitly flagged by the creator as more technical than typical texturing content.

### App & Version
Not stated on screen for either Substance Painter or Unreal Engine.

### Tags
`texture-set` `channel-packing` `export` `export-preset` `basecolor` `roughness` `metallic` `normal-map` `ambient-occlusion` `curvature` `thickness` `height` `alpha` `masks` `generator` `procedural` `blend-mode` `game-engine` `unreal-export` `color-management` `advanced` `expert`

---

## Related Tutorials
- [Zbrush to Substance Painter Bridge! NEW TOOL!](zbrush-to-substance-painter-bridge-new-tool.md) — same creator (Abe Leal 3D); a ZBrush-PolyPaint-to-ID-map workflow that shares this video's "custom Texture Set channel used for an unconventional masking purpose" spirit, applied to per-part masking instead of channel-packed export.
- [Substance Painter Tutorial: Texturing the Coin](substance-painter-tutorial-texturing-the-coin.md) — same creator; shares this creator's export-to-game-engine focus and small-prop production pipeline mindset.
- [Complex Wooden Medieval Door Tutorial in Substance 3D Painter](complex-wooden-medieval-door-tutorial-in-substance-3d-painter.md) — same creator; a larger production project sharing the same procedural-mask-building toolkit (generators, grunges, Multiply breakup) this video uses to build its custom blood channel.
