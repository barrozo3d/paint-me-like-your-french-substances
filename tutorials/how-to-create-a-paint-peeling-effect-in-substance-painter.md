---
title: How to create a paint peeling effect in Substance Painter
source: YouTube
url: https://www.youtube.com/watch?v=JnWvMys9xNk
author: Wes McDermott
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated on screen (title bar: \"Adobe Substance 3D Painter - PaintPeeling\"); creator explicitly notes filters gaining their own per-layer blending mode as a then-recent feature (previously required anchor points/multiple layers to combine a filter with underlying layers), tentative"
tags: [layers, fill-layer, paint-layer, masks, generator, anchor-point, blend-mode, ambient-occlusion, MatFX, height, roughness, basecolor, alpha, procedural, tri-planar, smart-material, texture-set, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/how-to-create-a-paint-peeling-effect-in-substance-painter/
frame_count: 12
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# How to create a paint peeling effect in Substance Painter

**Source:** [YouTube](https://www.youtube.com/watch?v=JnWvMys9xNk)
**Author:** Wes McDermott
**Duration:** 30m31s | 8 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Introduction [0:00]
**Transcript (timestamped):**
[0:00] A smart material is simply a collection of layers that you can reuse throughout your different Substance Painter projects.
[0:06] In this video, we're going to take a look at how we can create a paint peeling smart material.
[0:11] So let's jump in and take a look.
[0:13] Here you can see the final result that I created here in Substance Painter for this paint peeling material.
[0:19] Now, what we're going to do in this video is I'm going to show you step by step each layer,
[0:24] and I'm going to go over each process so that you can see that how I constructed this smart material here using Substance Painter.
[0:30] Now, I'm going to close out my texture sets and I'm just going to be looking at the head and you can see here that I have this single group.
[0:39] This is a folder and if I expand this, I have lots of layers in here.
[0:42] Like I said, we're going to go through each one of these layers.
[0:44] But once I have everything contained within a group, this is when I can just right click and choose to create a smart material from this.


### Creating a paint peeling smart material [0:50]
**Transcript (timestamped):**
[0:51] So now you can see that I have my paint peeling smart material and I can reuse this in any of my Substance Painter projects.
[0:56] All right, so let's jump in and take a look at this entire process.
[1:00] So first things first, what I'm going to do, I'm just going to start turning off some of these layers because I want to get down to just the original base layer here.
[1:08] And let's take a look at what we have.
[1:10] So if we look, you can see that I started with what is going to be the underlying material that we're going to see when the paint layer is peeled away.
[1:19] And so to start, I create a fill layer and the fill layer is, and I like to name this base because it represents kind of the overall base material of what this layer is going to be.
[1:31] And so with that, I'll use things like my color, metal, rough and so on and so forth.
[1:35] Now in this case, I have just a value that I set for my base color.
[1:39] I've set this to be a fairly rough material with no metallic and this becomes my base.
[1:43] Now what I want to do is start to vary the different color values within this base.
[1:49] And I do that again by a series of fill layers.
[1:51] So I start here with another fill layer that I call dirt on top.
[1:54] And here's what this guy looks like.
[1:56] So with this fill layer, you can see that this is just set to my color and height.
[2:02] And I have just a very, very small amount of height just to give that just a little bit of a bump to it.
[2:07] And so I'll increase that just a little bit more so we can see that.
[2:11] Now what I've done here is I take the fill layer and I apply a layer mask.
[2:16] Here's what the layer mask looks like.
[2:18] And if we go over here to the fill layer, you can see that the grunge map I'm using is just this concrete moss small and this ships with substance painter.
[2:27] Here I have controls like I balance my contrast.
[2:29] I can go in and kind of play with this.
[2:31] Now if I take a look here at the actual projection settings, it looks like I have this set to UV projection.
[2:38] Can't remember why I did that, but I probably should have set that to try planar again, because when I use this on different substance painter projects,
[2:46] I know that I don't have to worry about the seams or how the UVs are laid out.
[2:49] I can just rely on this tri-planar projection to kind of do a lot of the work for me.
[2:54] So if we hit M on the keyboard to go back to my material mode, this is the result that I'm getting so far.
[3:00] Now again, I like to constantly vary this material.
[3:03] So I'm going to add another fill layer on top of it just to add a little bit more detail here.
[3:08] Again, it's just a fill layer.
[3:10] You can see here that this time I'm only working with color information and I have this color swatch here that I can start to play with and make different,
[3:17] you know, values, different changes here to the color if I need to.
[3:20] I love working this way with a fill layer that's being masked because it gives me this kind of procedural workflow in the sense that I mean that I can easily go back and
[3:29] change the color by just changing the color here through the color properties window.
[3:33] Now I've masked the layer.
[3:36] So alt left click on the mask and this is what the mask looks like here.
[3:40] I'm using just a fill for my grunge concrete spots.
[3:44] Again, I have all my controls here.
[3:46] In this case, I think I left this to UV projection like I was saying before.
[3:49] I want to set that to tri-planar.
[3:51] That looks pretty good.
[3:52] Hit the M key to go back to my material mode and here's what that base layer looks like.
[3:57] So pretty good.
[3:58] I could keep playing with this if I wanted to, but overall this is this is looking okay.
[4:02] I think for what I want to do in this demo.
[4:04] All right.
[4:04] So let's close up the base and let's take a look at the paint layer.
[4:08] There's lots going on here.
[4:09] So first things first, you'll notice that I have a folder group and the reason why I use this folder group is because I was going to definitely want to create a mask that's going to represent the paint layer being peeled away.
[4:23] So that's why I set this in its own group and you can see that this mask has a lot of values set up here.
[4:29] So what I'm going to do in this particular case just so that we can kind of see this step by step, I'm going to right click on the mask, choose toggle mask, which essentially turns it off.
[4:38] And if I go back to my material mode, you can see that, okay, the mask is no longer working.
[4:43] All right.
[4:44] Let's take a look at the layers that build up this effect.
[4:47] So starting with the very first layer, you can see again, I probably should call this base using the same process that I did for my base material that's underneath of the paint layer.
[4:59] Like I said, I always use a fill layer.
[5:00] I call it base.
[5:01] And then I set a couple of channels here that represent kind of the basic surface attributes for that material layer.
[5:07] And so here I've set a color value.
[5:09] This is a lot more rough and that's pretty much it.
[5:12] So it's just this base layer.
[5:14] Now the next layer on top of it, if we just enable this guy, it's another fill layer again, following the same steps.
[5:20] Let's just call this color variation zero one.
[5:24] And if I look at the mask, you can see that I've masked the layer.
[5:27] It's using grunge concrete spots here.
[5:30] And I can, you know, I can play with all these values if I want.
[5:35] In this case, though, I can tell you that the projection was set to UV.
[5:38] So let's change that to try planar.
[5:41] Again, the reason I'm doing that is just so I don't have to worry about how the UVs were laid out.
[5:45] Essentially, it's going to, you know, re-project that grunge map across the X, Y and Z axes so that I basically don't get any seams.
[5:54] So it's not perfect.
[5:56] Sometimes you can see some blurs and things like that, but overall it's going to help quite a bit.
[6:01] So that's going to take care of my color variation one.
[6:04] And one other thing that I wanted to bring to your attention on this fill layer is you'll notice that I have for my base color
[6:11] channel, the opacity is set kind of low.
[6:14] And sometimes I like to go this route because I'm kind of relying more on just some kind of optical color blending by just blending color
[6:23] information just by varying its opacity.
[6:25] I find that to be a pretty good way to work to get some nice subtle color detail information.
[6:31] But then also it's just kind of visual process.
[6:34] So like I said, this is what it would look like without it.
[6:37] We do intense.
[6:38] So I just bring this value down just quite a bit.
[6:40] So I think I left it like 26.
[6:42] Now we're going to add another layer on top of it.
[6:45] This one here, I'm going to call this color variation zero two.
[6:51] And it's the same process.
[6:53] I'm just using the color value with the color.
[6:56] I have a layer mask that looks like this and I'm using grunge paint streak circular.
[7:02] Let's come over here to our projection settings and set that to try planar.
[7:07] Okay, so now I have these two layers in place.
[7:10] And just as I did before, I have for the base color channel, the opacity.
[7:15] I've just lowered that just again, just to play around with just some of that optical blending of the color values.
[7:21] Now the next layer that I have, if I enable this layer, this is bringing just a little bit of height information.
[7:27] So if I look at the fill layer and for the properties, you can see that I'm just using height information and it's negative information,
[7:35] but it's very, very low.
[7:36] Let's just increase it slightly so you can see what I'm talking about here and I'll zoom in and just move my light around.
[7:42] So you can see this is what I'm trying to create here.
[7:45] Just a little bit of this tactile feel to the material.
[7:48] And let's see, let's just, I think it's a little too intense now.
[7:51] Let me just crank it down very, very subtle, but this is kind of what I want to create here.
[7:56] And this is just using a layer mask.
[7:58] This is what the mask looks like.
[8:00] And here I'm using a grunge concrete moss medium.
[8:04] It looks like our concrete is misspelled on the grunge materials that chip inside of substance painter.
[8:10] So that's, that's kind of interesting.
[8:12] But this is the map that I'm using.
[8:14] Now, if we look, you can see again, I just made the mistake when I first created this, just kind of moving quickly.
[8:19] I did not set this to triplanar.
[8:22] Again, it's just kind of a habit I want to get into.
[8:24] Triplanar is going to be the way to go.
[8:25] And if I'm moving my light around, this is the overall effect that I get.
[8:29] So that takes care of the actual fill layer properties that are going to make up this layer.
[8:35] And the next big phase of this is to then mask this.
[8:40] So you can see I've created a black mask.
[8:42] It's turned off right now.
[8:43] So I'm going to toggle the mask to re-enable it.
[8:46] And now let's take a look at all these layers that I have.
[8:48] So with a black mask with no fill layers or no filters, you can see that, well, it just shows the raw layer underneath of it.
[8:57] So the first thing I did was I created a dirt generator.
[9:00] I thought this was pretty good because with the dirt generator, let me just set my UI up here.
[9:05] You can see that this gives me a kind of a neat effect where if I just play around with the level slider,
[9:10] this essentially is just kind of wearing or creating a mask where all the occluded areas are, which is totally what I want to do.
[9:17] Now, it looks pretty clean.
[9:18] So something else I could do.
[9:20] I didn't do it in this case, but let's just see what this does.
[9:22] I could increase this little grunge amount here if I wanted to.
[9:25] So you can see that just erodes a little bit into the surface.
[9:29] And with that case, I'm going to increase that contrast.
[9:33] So I think what the reason I didn't do it the first time is just because it's looking at it.
[9:39] I feel like it's a little bit too noisy here.
[9:41] So I'll tell you what, I could increase or decrease the grunge scale.
[9:46] So if I set that to one, that's a little bit better.
[9:49] I don't know.
[9:49] Let's just see what it does.
[9:50] That looks kind of interesting now.
[9:52] So now I just want to start layering effects.
[9:55] It's all about variation when you're creating smart materials like this.
[9:58] So I start with a jumping up here to my effects and adding a fill, which I've done here using grunge map
[10:05] 004 and let's enable this guy.
[10:07] And so you can see here that I have grunge map 04 and the blending mode is set to multiply.
[10:13] So by default, set to normal, it's basically just going to overwrite my dirt that's below it.
[10:19] So in this case, I want to combine the two.
[10:21] There's all kinds of different ways.
[10:22] We could add them.
[10:23] We could use lighten.
[10:24] In my case, though, I wanted to use a multiply and that essentially kind of combines these two layers together now.
[10:32] And this is really the core of creating masking inside of painter.
[10:36] We're building up what we call here a mask effect stack.
[10:40] And all of these layers, these fill layers, generators and filters are combining to create for me this overall mask.
[10:47] You can also create smart masks.
[10:48] So let's say I have all these effects.
[10:50] If I just right click on the mask, you can choose to create a smart mask.
[10:54] Really great way.
[10:55] If you save up a kind of a complex layering system that makes up your mask, you want to save that.
[11:00] You can always just right click and choose to create a smart mask from that.


### Blurring the mask [11:04]
**Transcript (timestamped):**
[11:04] All right.
[11:04] So let's continue on the process here.
[11:06] So the next thing I'm going to do is just blur this quite a bit.
[11:09] And so really I could play with this blur intensity, but I'm just kind of breaking this up a little bit more.
[11:16] And now that I've blurred this, I have a paint layer on top of it.
[11:19] We're going to come back to that in just a bit.
[11:21] So let's skip it and let's go to the next layer.
[11:23] So I blurred things.
[11:25] And the reason I did that is because it gives me some of this kind of great value, this kind of transitional gray value, which is like going to be like a slope here.
[11:33] And now I can run a levels on that to kind of crunch things together.
[11:38] So with the levels, you can see that I essentially just took the input black and just moved it all the way up so that I just, you know, really kind of get some nice harsh edge here.
[11:47] And then what I want to do is I created a warp on top of that.
[11:53] And so now you can see the difference here.
[11:56] It's really nice, the effect that it's creating along this edge.
[11:59] So here's what it looks like with no warp, very clean edge.
[12:03] And then we're just going to warp that edge quite a bit.
[12:05] So let's take a look at what that's doing here on the warp.
[12:07] Now, one of the things that it's doing that's actually new to Substance Painter is you'll notice that filters now have their own blending mode.
[12:16] And that's pretty powerful because what it does is it allows me to combine effects.
[12:21] Now, previously, and you know, I'll say in previous versions of Painter, it would be more work.
[12:26] I'd have to use maybe an anchor point or it'd have to use multiple layers to basically combine this warp in.
[12:33] But now I can essentially just use this multiply.
[12:36] So for example, here's what it would look like before.
[12:39] And it is working.
[12:40] It's warping everything, but it's not, it's not really, it's just warping everything on a whole.
[12:46] But if I take the values that I'm trying to warp and I multiply them by some of the layers underneath of it.
[12:52] So again, I'm taking this information from the layers and feeding that into the warp by just multiplying it.
[12:59] Now I get something that's a bit more kind of varied.
[13:03] And this is precisely what I want to do with this filter.
[13:06] So if I look at the warp, a couple of things I want to point out with this is the mode is set to warp.
[13:13] There's a couple of different modes and have this set to warp.
[13:16] And for the source parameters, the source mode, I have it set to a custom noise.
[13:22] And that custom noise in my case is going to be a purlin noise.
[13:25] And I will often use a purlin noise, especially when I want to create just some warping around edges like this.
[13:31] So purlin works really good for this.
[13:33] And you can see it's just helping me to get this kind of bumpy, wavy little line in here.
[13:37] So pretty good.
[13:38] And then I can play around here with this intensity value to increase or decrease that will say warpiness.
[13:44] All right, so next we're going to add a slope blur to this.
[13:48] And so this is going to be a subtle effect, but it's just kind of doing some I'm going to say non uniform erosion to some of these areas here.
[13:58] And really the goal of this is that I'm just trying to vary the amount of effects, you know, and the more that you kind of vary these things up, the better they're going to look.
[14:10] So for example, you'll notice again, we're using a filter slope blur, and it's using this multiply.
[14:15] If I set that to normal, it's just slope blurring everything again.
[14:19] But now, like I said, I can take into consideration all these layers underneath of it and combine them by using this multiplying mode.
[14:26] And you can get different effects.
[14:27] Like if I could do like a subtraction or you know, we'll subtraction is going to not it's not going to work in this case.
[14:33] Now let's take a look at that slope blur with that's doing.
[14:36] So we'll move this up and you can see that for my blending mode here, I'm using this min as the mode that I'm using qualities set to one source parameters, source type custom noise once again, and that Perlin noise.
[14:49] So using Perlin noise here to help create these little slight edges.
[14:53] Now, if we look all left click on the mask, you can see this is what I'm talking about here.
[14:58] This is what this blur is doing.
[14:59] So see, you have this kind of more of a beveled.
[15:02] It's a little bit harder and then that slope blur is just pushing because I'm using this minimum mode.
[15:08] If I set this to say maximum, it pushes kind of the other way.
[15:11] Basically the white values get blurred towards the dark.
[15:14] But if we set this to minimum, we can take the dark values and kind of push those inwards towards the white values and blur is going to be a combination of both.
[15:23] But in my case, like I said, I want to set this to min and then it's subtle.
[15:27] But I get this nice kind of little bit of a fall off or a slope here to that edge.
[15:32] And it's just that little bit of extra modeling that I did that I just want to have for the material itself.
[15:37] Now, the next part of this, let's go back to my material mode is I just run a levels on top of it and that really is just going to help kind of crunch things in together.
[15:46] And so here you can see what I'm going to do.
[15:48] I might play with this a little bit now that it's here and I'm seeing this, but I'm just kind of crunching these values up a little bit.
[15:53] So let's just play with these and it's just, you know, playing with the levels until I can get the value that I want.
[15:59] So here's what it looks like without a little bit too soft.
[16:03] And then I'm just tightening everything up with the levels effect here.


### Painting the peeling effect [16:06]
**Transcript (timestamped):**
[16:07] And so that is basically going to take care of this paint peeling effect.
[16:11] Now, let's go back to this paint.
[16:13] So I said, we'd come back to this if I enable this paint.
[16:16] What this is, is just a layer.
[16:18] And if I look at the value that I'm painting here is because I'm in a mask, if I paint black, it's going to, you know, basically remove our mask.
[16:28] And if I hit the X key to swap this to a white value and paint, it's going to add to the mask.
[16:33] And so this paint just gives me a control for just going in and just painting some of the peeling exactly where I want it to be.
[16:41] And here I'm just using a round brush.
[16:42] But if I go in and use like an actual grunge brush with with some dirt or something like that, I can get a lot more of an organic look.
[16:51] And then I can always just toggle the value back just to kind of, you know, bring some of the material back.


### Masking the material [16:56]
**Transcript (timestamped):**
[16:56] Okay, so we get something like that.
[16:57] Now, once this effect is in place, what I want to do is I want to anchor all of this information because I am going to need to use it again.
[17:04] Another layer.
[17:05] So I created an anchor point here and let's actually do some proper naming.
[17:10] So I'm going to call this paint layer mask.
[17:13] And there we go.
[17:14] So now we can close up this layer and that takes care of my base and my paint layer.
[17:19] Now the rest of the layers on top are going to be about creating just a little bit more information to the material as well as creating the actual peeling effect.
[17:28] Okay, so the next layer I have called cracks and it is a fill layer.
[17:34] Let's enable this guy and you can see that it is just a fill layer.
[17:37] I'm just using height information with some positive height value around, you know, 0.28.
[17:42] So this is a layer that's masked and so it's just using marble fine and I'm playing around with the overall balance and some of the noise parameters.
[17:51] If we look here though at the projection, I could go ahead and set that to try planar.
[17:55] Probably want to always make sure I set that.
[17:58] So this is just giving me some just some of this cracks information.
[18:03] So if we look, you can see that I can jump over to the material itself and I can increase or decrease this value.
[18:09] So if I want it to be just a little bit more subtle, I can just, you know, lower that height value still positive, almost 0.2.
[18:15] And so that looks pretty good.
[18:17] Just a little bit of like kind of wrinkling around the area.
[18:21] Now I have another layer called cracks inside.
[18:24] So if we click, you can see that that is just another variation.
[18:27] So it's just the cracks once again, except just on the inside.
[18:31] And so the way that I do that is I just create a layer mask and you can see here that I'm using marble fine again.
[18:39] So here it's using that marble fine.
[18:42] Let's make sure that that is set to try planar.
[18:45] Okay.
[18:45] Now, because I want this to be on the inside of the actual painted layer here is where I add a fill.
[18:52] So I come up and I add a fill.
[18:54] And if we look at the properties for the fill, you can see that this is going to be the first time that I reference my paint layer.
[19:01] So just to recap, if we come down to the paint layer, I'm going to just click to expand the layer group.
[19:08] You can see that I have all of these layers that create the mask effect.
[19:13] And at the very top, I've anchored that.
[19:15] So essentially what that means is it's going to take all of this, all of these layers and it wraps it into this paint layer mask.
[19:22] Another really great way to look at anchors is think of it like being able to merge layers.
[19:28] So we don't have like a layer merge inside of painter, but you can use layer anchor points to do that exact same thing.
[19:34] All of this layer information is now accessible or can be referenced through this anchor point.
[19:39] And that's exactly what I've done here for the cracks inside layer.
[19:43] So if you look at this, all I've done here is I have my marble fine, which is giving me the lines, these, these, these extra cracks here.
[19:53] And then I have my fill, which my anchor point.
[19:55] And then I subtract that from the marble.
[19:58] And what that does is it just removes this layer.
[20:02] So if we come over here to this layer and I push this negative look, if I go positive or negative, it's just affecting the base layer underneath of my paint layer.
[20:12] And so that's how that system works.


### Creating the peeling effect [20:14]
**Transcript (timestamped):**
[20:14] Now we're going to start working on the actual peeling effect.
[20:17] And it's a lot easier than you would think.
[20:19] So you can see here that I have a fill layer set to height channel only, and it's set to a positive value of one.
[20:25] Let's take a look at what that's doing.
[20:26] So I'll enable the layer here it is on and off.
[20:29] And already we're starting to get a huge effect here.
[20:32] So how are we doing this?
[20:34] Like I said, it's a lot easier than it looks.
[20:36] So what I'm essentially creating here is a layer mask that looks like this.
[20:40] And what I'm using is a couple of things.
[20:43] First off, the magic happens by using that paint layer mask.
[20:47] So I create a fill and I reference that paint layer mask from my paint layer.
[20:52] And then I'm adding a new filter called mask outline on top of it.
[20:57] And with mask outline, you can see here that we have a couple parameters.
[21:01] The most important parameter for me is this start from black.
[21:05] I think by here, let's if we restore defaults, you can see it set to true.
[21:09] This is what it would look like.
[21:10] So this is totally not what I want at all.
[21:12] But if I go ahead and set the mask position, let me look at the mask here.
[21:18] Go back into the peel.
[21:20] And I'm going to set this value to false.
[21:24] Now I get this nice kind of gradient, this slope, and you have this mask position.
[21:29] It's set to outside.
[21:31] Well, you could have inside.
[21:32] And this is a great way to create an edge mask.
[21:35] I love this filter.
[21:36] It's super, super helpful.
[21:37] However, what I want to do is I want to use this option called both.
[21:42] And so now you can see that I have this edge right where the peeling happens.
[21:47] And then this nice slope fall off on both the inside and outside of that edge.
[21:52] And that's pretty much it.
[21:53] So if I hit the M key to go back to my material mode, this is what I'm getting.
[21:57] All I have to do now is play around here with the blur of this so I can blur it.
[22:03] And I can play with the overall kind of width of that.
[22:06] So you can dial this effect up and down.
[22:09] So I'm just kind of playing with some of these values here to get what I want.
[22:12] Now we also have the curve shape.
[22:14] And this is pretty interesting.
[22:15] So you can see that I can kind of round this.
[22:17] So that could be interesting.
[22:18] But really what I want to do is set the curve shape to negative one.
[22:22] And this gives me that really nice kind of fall off that I want for that curve edge.
[22:26] And so I can increase or decrease the width.
[22:28] And this is looking pretty good here.
[22:30] Okay, so let's take a look at the next layer to this.


### Creating the peel edge [22:31]
**Transcript (timestamped):**
[22:33] And that's going to be the peel edge.
[22:35] So I'll enable this layer and this is really making things kind of stand out and pop.
[22:40] And let's see how that is working.
[22:42] So if we look at the fill layer itself, you can see that I am using a color value.
[22:46] So now I've set a color value.
[22:48] And what I did was I just went in and just sampled kind of this blue value and then just increased the value like this just to make it a lot brighter.
[22:57] So just something really simple like that.
[23:00] If we wanted to, we could also go in and start to play around with some of these blending modes, like maybe do like an overlay or subtract or something like that.
[23:07] But in my case or a lighten, but in my case, I'm just going to leave it to the color value.
[23:11] And I may want to just back off the opacity.
[23:13] So I could do that.
[23:14] And so it's not just super, super saturated.
[23:17] So I'll just back it off a little bit.
[23:19] Now let's take a look at the mass that's being created here.
[23:21] And this is what it looks like.
[23:23] So let's go through all the layers on this guy.
[23:25] First things first, what we do is I create a fill and I reference my paint layer mask once again.
[23:31] Now I'm going to use the same mask outline filter.
[23:34] So we'll enable mask outline.
[23:36] This time start from black is set to false.
[23:40] The mask position is on the inside.
[23:43] And now I'm just making a few adjustments here to my curve shape and my width.
[23:48] And so if I hit the M key on the keyboard to go back to my material, this is kind of what I'm getting here.
[23:52] Now the big trick to this though is we now have this nice kind of gray slope value.
[23:57] And it's, it's, this is giving me a nice masking effect, but it's very, very uniform.
[24:01] So what I want to do here is just add another fill layer with some type of grunge map.
[24:06] In my case, I use fractal sum four.
[24:08] And so we'll enable this grunge map.
[24:10] And you can see that the blending mode is set to subtract.
[24:13] And then I just dropped the opacity.
[24:15] So here's what I'm getting.
[24:17] And this is starting to really break up this edge.
[24:21] And I'm super happy with the result that this is giving me.
[24:24] Now the only problem is I can see that my gray values are, you know, it's just, they're kind of muddied a little bit.
[24:31] So here's where I'm just going to use a levels effect just to clamp everything down.
[24:35] And so with just these few tricks.
[24:38] So again, we use the, we reference the paint layer mask, run a mask outline, subtract a grunge map, and then run levels to process the ranges.
[24:48] And this is the mass that we get.
[24:50] So we go back to our material mode and there we go.
[24:52] Now looking at this, I feel like the, the opacity for that layer is too low.
[24:58] So let me just dial it back up.


### Adding ambient occlusion [25:00]
**Transcript (timestamped):**
[25:00] Okay, so there we go.
[25:01] So that pretty much takes care of the effect that I've been working on here.
[25:05] Now the next thing that we're going to do just so we can really see this work is I want to use this matte FX horizon based ambient inclusion effect.
[25:13] And so here, let me show you how this works from scratch.
[25:15] So we're going to delete that.
[25:16] And if I jump over here to my texture set settings, let's see when we find where that is right here, my texture set settings.
[25:24] So I'm going to come over here to my channels and I'm going to add an ambient occlusion channel.
[25:29] Now if I jump back here to my layers and let's come over here to the asset library and I'm going to do a search here in my filters.
[25:36] So HB AO.
[25:37] And here I have this horizon based ambient occlusion.
[25:40] So now I can just left click drag and drop and place this right here into my scene.
[25:45] So now I can play around with things like my height depth and I'm going to increase my radius here.
[25:51] And so what this is doing is just adding some ambient occlusion here and then I'll play around with things like my blur intensity.
[25:58] Just kind of dial this guy in to get this effect that I'm looking for.
[26:01] So now I'm starting to get just like a little bit of shading within the peeled paint layer and that just gives us a little bit more depth.
[26:07] So now that I have my core material set up, I want to add a little bit of color variation.
[26:12] And so I have this color variation layer that's just essentially a fill layer.
[26:16] So let's take a look at what this guy is going to turn off these effects and just turn this on.
[26:20] And so I have a fill layer that has my color value set.
[26:23] So just a color channel and I set a color and for the base color channel, you can see that the opacity is set pretty low.
[26:30] So like 33% live.
[26:32] We pull this all the way up overriding all of our color values.
[26:35] So let me show you a couple of things that I can do here that's kind of interesting.
[26:39] And so what I'm going to do with this color layer selected, I click and add a fill layer on top of it.
[26:45] So I have a fill layer here and this fill layer on its base color channel, I have a grunge concrete old set.
[26:54] And so it's just one of the grunge maps that ship and painter and you can see here that I'm just overlaying that here to the color channel.
[27:03] Overriding that or blending with it with this fill layer.
[27:06] Now, if I want to override it, if I set this all the way to 100, that's an overwrite, but now I'm just dropping the layer opacity.
[27:12] So I get this blend between the grunge map, which is black and white and the original base color, which is this color value here on the fill.
[27:21] So then on top of this, I am adding a gradient filter.
[27:25] And this is pretty powerful because what I can do here is I can then colorize the layer underneath of it.
[27:34] So in this case, the layer underneath of it is this grunge concrete old grunge map.
[27:40] So the gradient is on top.
[27:42] And here I can see that it's going to remap those black and white values to the color one, two and three values that I have now have four color values.
[27:50] So I have all these colors set.
[27:52] So it's really intense, super over saturated.
[27:55] And I kind of went that route on purpose because at the top, I'm then going to use this HSL perceptive filter to then kind of bring everything back down here.
[28:05] And now once everything's set up, I'm going to jump over here to the color variation, grab my opacity slider and then just bring this down.
[28:13] And I think I had a value of like say point, I'll just say 30%.
[28:16] So it's 30.
[28:17] And it's very subtle.
[28:19] If I zoom really close in and let's just toggle this on and off, you can see what it's doing.
[28:23] Just adding a little bit of color variation across the whole thing.
[28:26] Some of this color is kind of speckling value.
[28:29] And this really helped me to create this, this very subtle color variation.
[28:35] Like I said, like this is really what I was going for.
[28:37] And then at the very top of my layer stack, I just have a sharpen.
[28:40] So this is what it looks like.
[28:41] And then I just went over here to my filters.
[28:45] And in here we have a sharpen and just drag and drop that to the layer stack.
[28:50] Here's what it looks like.
[28:51] And then I can adjust the sharpen intensity by just moving this slider around, dialing this in to get exactly what I want.
[28:59] And so now this finishes up the paint peeling smart material that I wanted to create in this video.
[29:06] Now what's kind of interesting is I can jump down to my paint layer.
[29:10] And if I go to my paint here, like I said, I have my brush.
[29:13] I can now go in and I can just paint to fill in some of these areas.
[29:18] I also have my dirt as a control so I can move this up and down to kind of dial this effect up and down just by using dirt.
[29:26] And then like I said, I can jump over to this paint and then kind of paint this value in.
[29:30] So we can do some interesting stuff like this just to get different results here in this mass that's being generated here for the paint layer.
[29:38] So it's just a matter of just painting between the white value and the black value to kind of rip in or peel away this paint layer as you can see here.
[29:46] And then of course just using different brushes is going to is going to really make this a lot more realistic.
[29:52] So for example, if I jump over here, I have this dirt brush.
[29:55] Oh, where is it dirt to and I'll increase the contrast of it.
[29:58] And then if I come in and just kind of paint, you can see this kind of rips into the brush.
[30:02] You can just get different effects just depending on like, you know, the different kind of effects that you want here, but it's really powerful, pretty cool type of effect.
[30:11] And like I said, everything is still because it's all connected together through these different blending modes.
[30:15] I can always just use the dirt slider here to play around with this value as well and kind of tear into that.
[30:21] So that's going to close out this video on how to make a paint peeling smart material using Substance Painter.
[30:27] Thanks a lot for watching and I'll see you next time.



---

## Captured Frames

- [1:19] tutorials/frames/how-to-create-a-paint-peeling-effect-in-substance-painter/frame_000.jpg
- [2:11] tutorials/frames/how-to-create-a-paint-peeling-effect-in-substance-painter/frame_001.jpg
- [8:00] tutorials/frames/how-to-create-a-paint-peeling-effect-in-substance-painter/frame_002.jpg
- [10:05] tutorials/frames/how-to-create-a-paint-peeling-effect-in-substance-painter/frame_003.jpg
- [11:47] tutorials/frames/how-to-create-a-paint-peeling-effect-in-substance-painter/frame_004.jpg
- [13:44] tutorials/frames/how-to-create-a-paint-peeling-effect-in-substance-painter/frame_005.jpg
- [17:05] tutorials/frames/how-to-create-a-paint-peeling-effect-in-substance-painter/frame_006.jpg
- [19:01] tutorials/frames/how-to-create-a-paint-peeling-effect-in-substance-painter/frame_007.jpg
- [20:19] tutorials/frames/how-to-create-a-paint-peeling-effect-in-substance-painter/frame_008.jpg
- [22:42] tutorials/frames/how-to-create-a-paint-peeling-effect-in-substance-painter/frame_009.jpg
- [25:24] tutorials/frames/how-to-create-a-paint-peeling-effect-in-substance-painter/frame_010.jpg
- [28:40] tutorials/frames/how-to-create-a-paint-peeling-effect-in-substance-painter/frame_011.jpg

---

## Structured Notes

### Core Technique
A full, from-scratch build of a reusable **Paint Peeling Smart Material**: an underlying "base" material group sits beneath a "paint layer" group whose mask is sculpted through a long procedural chain (dirt generator -> grunge multiply -> blur -> levels -> a filter-native `Warp` and `Slope Blur` both set to `Multiply`/`Min` so they read the layers beneath them instead of applying uniformly), then that entire finished mask is captured once as an **Anchor Point** and reused by name across four separate downstream layers (cracks-inside subtraction, the peeling-edge height push via `Mask Outline`, a colored peel-edge accent via a second `Mask Outline` config, and manual paint control) — turning one sculpted mask into the single source of truth for the whole effect.

### Summary
Wes McDermott builds a paint-peeling Smart Material end-to-end on a sphere-topped prop, narrating every layer in the finished group. **Base layer:** a Fill layer (Color/Metal/Roughness) as the "revealed" material seen once paint peels away, built up with two more Fill layers for color variation (each masked by a built-in grunge map — `Concrete Moss Small`, `Grunge Concrete Spots` — with Projection corrected from the default UV to **Tri-Planar** to avoid seam/UV-layout dependence, a fix the creator flags as something he "should have done" originally). **Paint layer mask stack:** starting from a Dirt generator (Level slider for occlusion-based wear, optional Grunge Amount/Contrast/Scale tuning), combined with a `Grunge Map 04` Fill layer set to blend mode `Multiply` (chosen over Normal/Lighten so the two masks combine rather than overwrite) — explicitly named as "the core of creating masking inside of Painter," i.e. a **mask effect stack**. This combined mask is then Blurred (creates a soft gray transitional slope), tightened with a `Levels` filter, then passed through a `Warp` filter and a `Slope Blur` filter — both demonstrated as a **then-new capability: filters carry their own per-layer blend mode**, set here to `Multiply` (Warp) and `Min` (Slope Blur, meaning dark values erode toward white) so each filter reads and combines with the layers underneath rather than distorting/blurring the whole canvas uniformly; both filters use a custom **Perlin noise** source for organic, non-uniform edges. A final `Levels` pass crunches the result to a clean edge. **Manual paint control:** a Paint sub-layer sits directly in the mask stack — painting black removes paint (reveals base), `X` inverts to white to restore paint; a grunge-tipped brush (vs. a plain round brush) gives a more organic torn-paint look. **Anchor point capture:** once the mask stack is finished, it's wrapped in an Anchor Point (named "Paint Layer Mask") — described as Painter's equivalent of a non-destructive layer-merge, since there's no true merge command. That anchor is then referenced four separate times: (1) a "cracks inside" layer subtracts the anchor-referenced fill from a `Marble Fine` noise layer to confine interior crack detail to the base material only; (2) the actual peeling-height illusion is a Height-only Fill layer (value 1) masked by a Fill referencing the anchor, run through a **Mask Outline** filter (`Start From Black = false`, `Mask Position = Both`, curve shape set to -1) which turns the flat mask into a graduated inside+outside slope right at the peel boundary; (3) a "Peel Edge" colored accent layer (a sampled-and-brightened blue, low opacity) uses a second Mask Outline config (`Start From Black = false`, `Mask Position = Inside` only) further broken up by a `Fractal Sum 4` grunge map set to `Subtract` blend and cleaned with another `Levels`; (4) ambient occlusion depth is added via `Texture Set Settings` (add an Ambient Occlusion channel) and the **HBAO (Horizon-Based Ambient Occlusion)** MatFX effect dragged in from the asset library, tuned via Height Depth/Radius/Blur Intensity. Finishes with a subtle color-variation Fill layer (grunge map remapped through a `Gradient` filter's 4-color ramp, deliberately over-saturated then tamed with an `HSL Perceptive` filter, opacity dropped to ~30%) and a top-of-stack `Sharpen` filter, then a live demo of hand-painting the peel pattern with the dirt slider and a grunge brush for final artistic control.

### Key Steps
1. **Build the underlying base material** (what shows once paint peels away): Fill layer named "base" with Color/Metallic/Roughness values, then layer 1-2 more Fill layers for color variation, each masked by a built-in grunge map (Concrete Moss Small, Grunge Concrete Spots) with mask Projection set to **Tri-Planar** (not the default UV) to avoid UV-seam dependence when reusing the material elsewhere.
2. **Group the paint layer's contents in its own folder** specifically because its mask needs heavy, multi-step sculpting — keeping it isolated from the base material's own layers.
3. **Build the paint-layer's own base + color variation** the same way as step 1 (a "base" Fill layer plus 1-2 color-variation Fill layers masked by grunge maps), including a technique of setting a Fill layer's own channel **opacity low (e.g. ~26%)** to rely on optical color blending against the layer below rather than a hard override.
4. **Start the peeling mask with a Dirt generator on a black mask**, tuning the Level slider (this alone approximates occlusion-based wear), optionally raising Grunge Amount for surface erosion and Contrast/Scale to control noise character — used at fairly clean/subtle settings here.
5. **Combine a second grunge mask via Multiply:** add a Fill layer masked with `Grunge Map 04`, set its blend mode to `Multiply` (not the default Normal, which would just overwrite the dirt mask below, or Lighten/Add which combine differently) — this is the core "mask effect stack" principle: several generators/fills/filters compositing together into one final mask.
6. **Blur the combined mask** to create a soft gray transitional gradient at the wear boundary, then run a `Levels` filter pushing input-black up to crunch that gradient into a harder edge.
7. **Add a `Warp` filter set to blend mode `Multiply`** with Source Mode = Custom Noise = **Perlin noise** — using the filter's own blend mode (a then-new Painter capability, previously requiring anchor points or extra layers to combine a filter with underlying layers) means the warp distortion is driven by/combined with the mask data beneath it rather than distorting the whole canvas uniformly.
8. **Add a `Slope Blur` filter set to blend mode `Min`** (Perlin noise source again) for a subtle non-uniform edge erosion — `Min` pushes dark values inward toward white (vs. `Max`, which pushes white toward dark); run a final `Levels` pass afterward to re-crunch the result.
9. **Add manual paint control inside the mask stack:** a Paint sub-layer where painting black removes the paint effect (reveals the peel), pressing `X` inverts to paint white (restores paint); switching from a plain round brush to a grunge/dirt-textured brush produces a more organic torn-paint edge than a clean circular reveal.
10. **Capture the finished mask stack as an Anchor Point** (named e.g. "Paint Layer Mask") positioned at the top of that layer group — functions as Painter's substitute for a non-destructive layer merge, making the whole stack's result referenceable by any other layer's mask.
11. **Build "cracks" and "cracks inside" detail layers:** a Height-only Fill layer masked by `Marble Fine` noise (Tri-Planar projection) for surface cracking; a second "cracks inside" variant adds a Fill referencing the Anchor Point and **subtracts** it from the Marble Fine mask, confining that crack variant to just the base material's revealed area (positive/negative height value flips which direction the crack reads).
12. **Build the actual peeling-height illusion:** a Height-only Fill layer (value 1) whose mask starts from a Fill referencing the Anchor Point, then add a **Mask Outline** filter on top with `Start From Black = false` and `Mask Position = Both` (not the defaults) — this converts the flat referenced mask into a graduated slope on both the inside and outside of the peel boundary; further shape it with the filter's own Blur, Width, and **Curve Shape = -1** parameters for the desired fall-off profile.
13. **Build a colored "Peel Edge" accent layer:** new Fill layer using a sampled-and-brightened accent color (low opacity) whose mask again references the Anchor Point through a Mask Outline filter, this time `Start From Black = false` / `Mask Position = Inside` only; break up the resulting uniform gray slope by adding a Fill layer with a grunge map (`Fractal Sum 4`) set to blend mode `Subtract` at reduced opacity, then clean the result with another `Levels` filter.
14. **Add ambient-occlusion depth for readability:** open Texture Set Settings and add an Ambient Occlusion channel, then drag the **HBAO (Horizon-Based Ambient Occlusion)** MatFX effect from the asset library shelf (search "HBAO") into the layer stack; tune its Height Depth, Radius, and Blur Intensity to add contact shading within the peeled crevices.
15. **Add subtle overall color variation:** a Fill layer with a low-opacity (~33%) base color, topped by a second Fill layer using a grunge map (`Grunge Concrete Old`) on the base-color channel at reduced opacity for a black/white blend against the flat color, then a `Gradient` filter on top to remap that grunge map's black/white values through a deliberately over-saturated 3-4-color ramp, tamed afterward with an `HSL Perceptive` filter; drop the whole color-variation layer's opacity to ~30% for a subtle final effect.
16. **Finish with a top-of-stack `Sharpen` filter**, dialing its intensity to taste.
17. **Right-click the finished group and choose "Create Smart Material"** to package the entire layer stack as a single reusable, drag-and-drop asset for future projects.
18. **Live-paint the final result:** use the Paint sub-layer from step 9 with the Dirt slider (from step 4) and a grunge/dirt-textured brush to hand-place peeling exactly where wanted, toggling between black (peel) and white (restore, via `X`) as needed.

### Layers / Tools / Settings
- **Base material:** Fill layer(s) with Color/Metal/Roughness, masked by built-in grunge maps (Concrete Moss Small, Grunge Concrete Spots), Projection corrected to **Tri-Planar**
- **Paint mask stack:** `Dirt` generator (Level/Grunge Amount/Contrast/Scale) -> `Grunge Map 04` Fill blend mode `Multiply` -> `Blur` -> `Levels` -> `Warp` filter (blend mode `Multiply`, Source = custom Perlin noise) -> `Slope Blur` filter (blend mode `Min`, Perlin noise) -> `Levels`
- **Manual control:** Paint sub-layer (black = remove paint, white via `X` = restore), grunge-tipped brush for organic edges
- **Anchor Point:** captures the entire finished mask stack, referenced by 4 separate downstream layers/masks
- **Cracks:** Height-only Fill masked by `Marble Fine` (Tri-Planar); "cracks inside" variant subtracts an anchor-referenced Fill from the Marble Fine mask
- **Peel height:** Height-only Fill (value 1), mask = anchor-referenced Fill + `Mask Outline` filter (`Start From Black=false`, `Mask Position=Both`, `Curve Shape=-1`, tuned Blur/Width)
- **Peel Edge accent:** colored Fill (sampled/brightened, low opacity), mask = anchor-referenced Fill + `Mask Outline` (`Start From Black=false`, `Mask Position=Inside`) + `Fractal Sum 4` grunge Fill blend mode `Subtract` + `Levels`
- **Ambient occlusion:** Texture Set Settings AO channel + `MatFX HBAO` (Horizon-Based Ambient Occlusion) effect, tuned Height Depth/Radius/Blur Intensity
- **Color variation:** low-opacity base color Fill + `Grunge Concrete Old` Fill + `Gradient` filter (4-color remap) + `HSL Perceptive` filter, overall opacity ~30%
- **Finish:** top-of-stack `Sharpen` filter
- **Packaging:** right-click group -> Create Smart Material

### Difficulty
Advanced — this is a complete ground-up Smart Material construction assuming fluency with generators, multi-filter mask stacks, blend-mode math, and (critically) the anchor-point-as-single-source-of-truth pattern referenced across four different downstream layers; the Mask Outline filter's `Start From Black`/`Mask Position` parameters and the filter-native blend-mode feature are both explained but assumed to be genuinely new concepts to the viewer.

### App & Version
Not stated numerically on screen (title bar reads "Adobe Substance 3D Painter - PaintPeeling", the project file name). The creator explicitly calls out filters having their own per-layer blend mode as a **then-recent feature** ("previously... I'd have to use maybe an anchor point or... multiple layers to basically combine this warp in") — a useful relative-version marker even without a specific version number, and consistent with this skill's modern-era ingested tutorials.

### Tags
layers, fill-layer, paint-layer, masks, generator, anchor-point, blend-mode, ambient-occlusion, MatFX, height, roughness, basecolor, alpha, procedural, tri-planar, smart-material, texture-set, intermediate, advanced

---

## Related Tutorials
- [Advanced Peeling Paint Effect in Substance 3D Painter](advanced-peeling-paint-effect-in-substance-3d-painter.md) — different creator (Javad Rajabzade), same core subject (procedural paint peeling) and the same anchor-point-as-shared-mask-source pattern; that video leans on Voronoi-fractal noise and a Multiply-Light paint-reveal trick where this one leans on the Mask Outline filter and filter-native blend modes — strong side-by-side comparison for the same effect family.
- [How to TEXTURE like a PRO with ANCHOR POINTS | Substance Painter Tutorial](how-to-texture-like-a-pro-with-anchor-points-substance-painter-tutorial.md) — different creator (Jared Chavez); this video's core anchor-point-as-reusable-mask-source technique (one anchor referenced by 4 separate downstream layers) is a direct, exhaustive real-world application of that anchor-points tutorial's central lesson.
- [SUBSTANCE PAINTER: Building Masks Explained](substance-painter-building-masks-explained.md) — different creator (Jared Chavez); shares the "mask effect stack" philosophy (generators/fills/filters combined via specific blend modes to sculpt one final mask) at a similarly exhaustive level of detail.
