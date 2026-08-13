---
title: SUBSTANCE PAINTER: Building Masks Explained
source: YouTube
url: https://www.youtube.com/watch?v=um3YRzqwYU4
author: Jared Chavez
ingested: 2026-08-12
app: "Substance 3D Painter"
version: "not specified (UI consistent with pre-12.1 era, approximate)"
tags: [masks, layers, paint-layer, fill-layer, generator, smart-mask, curvature, ambient-occlusion, mesh-maps, tri-planar, procedural, alpha, blend-mode, anchor-point, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/substance-painter-building-masks-explained/
frame_count: 12
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# SUBSTANCE PAINTER: Building Masks Explained

**Source:** [YouTube](https://www.youtube.com/watch?v=um3YRzqwYU4)
**Author:** Jared Chavez
**Duration:** 23m13s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hey, how's it going guys? So today I wanted to talk about feature inside of Substance Painter that I think is commonly overlooked in how powerful it is. That's going to be masking. So if you are at all familiar with using Substance Painter, you're probably familiar with masking to some extent, but it's very imperative in creating complex, good looking textures for any of your characters. So I just wanted to dive a little bit deeper into that today. So let's go ahead and dive right in. The first thing that we're going to talk about is just simple masking.
[0:30] Right? So if you have your character, one of the most common processes that you're going to use is just creating a simple mask. So let's apply this white to one specific area. So we would use a mask essentially to do that. What we would do is we would come over here to the material and we're going to right click. And this is going to give us access to the add white mask, add black mask, add bitmap mask, and a couple of other selections.
[0:54] The first one that I'm going to do is going to be add black mask. What that's going to do is it's going to create this black fill layer across the entire character. This is now going to allow so that when I am selecting this icon over here, I can come in here and just paint on top of the character.
[1:12] So now wherever that white color is going to be seen is going to be enabled on our textures. So if you come over to this mask and you hold Alt and tap on it, that will bring up this view so that you can independently view your mask. Or if you want to, you can come over here to this drop down and you can scroll down to mask. Or if you hit C on the keyboard and shift C, you can scroll forward and backwards in all of your channels.
[1:38] So now you can see this is kind of the first, you know, manual way of going about creating masks, which may be good, maybe bad, you know, it just really depends on what it is that you're trying to create, but it is one of the tools that you would use and pause.
[1:54] So my editing team, I'm my editing team, I'm looking at the analytics here told me that 56% of you guys don't subscribe to the channel. That's a lot. That's, that's more than 50%. That's 6% more than 50%. Not only are 56% of you not subscribed, there's also only 9% of you that have the notifications turned on.
[2:13] So if you want to see all of my content, make sure to hit that bell to turn that on as well. So if you guys could go ahead and do me a favor, make sure to subscribe to the channel so that you can watch more cool content about 3D character.
[2:24] And if you did it, well, well, thanks. If you haven't yet, go click the button. Now back to what we were talking about. Some of the other ones that are a little bit more complex is something like adding a mask with a color select.
[2:36] For this character in particular, I don't think I have. Yeah, I don't have an ID mask on here. So I'm not able to go in and color pick specific parts of the mask.
[2:45] But if I had a character with armor, you know, leathers, metals, things like that, I would have built out an ID mask in order for me to be able to come in and, you know, color pick specific elements to create a mask relatively quickly.
[2:59] In this case, I don't have that, which not a big deal. But the next thing that I wanted to add on top of here, you can add on top of this mask. You can add layers on top of this mask, right?
[3:11] So we talked a little bit about painting. If you want to add layers on top of your mask, a good way to go about doing that is coming down to this bottom section and adding something like a paint layer.
[3:23] So if we really wanted to, we could come in and, you know, we could draw our design on here and then it's like, okay, well, I really like what I have in this section of the layer.
[3:33] What I'm going to do is I'm going to add another paint layer on top of it, and I'm going to either draw some more, maybe subtract some until we get something like this.
[3:43] But it's like, oh, well, I don't really like what I added. So what would I do? Well, I can come back here and I can turn this paint layer off so that I'm back to my original design.
[3:52] So that I'm back to my original starting point. So it's a great way to create and work in a non-destructive fashion by creating multiple layers in order to build up something more complex, right?
[4:03] So that is going to lead us into some of our next masks that we're going to take a look at. So we're going to add a red layer.
[4:13] So this will be our red layer. And what we're going to want to do is we're going to want to pump some of this color into maybe like our ambient occluded areas.
[4:22] So like maybe some of these cracks and crevices and things like that, right?
[4:26] So most people, this is probably the process that they're most familiar with, which is using generators and generators are great.
[4:34] If you come down here in your assets menu, you have access to all of these smart material masks that you can use to essentially generate a mask for you relatively quickly.
[4:46] When making characters, most of the time I rely on probably like five or six of these and they kind of get me either a good working place or just a general starting point that I will modify after the fact.
[5:00] If you don't want to use one of these, you can always build your own by coming here to add generator.
[5:05] And in the generator, you have another list of ways you can go about it.
[5:10] Some of the really nice ones that you have in here is things like curvature.
[5:14] So this will just generate a curvature mask off of your curvature map that is baked inside of substance painter.
[5:21] So you can come in here and you can kind of just modify that.
[5:24] Although it's a little bit limited, you do have a little bit more control once you expand the curvature map where you can start to independently control certain levels of detail, whether it be the sharp details or the big details.
[5:38] So you can see if I start to kind of pull some of this down.
[5:42] Now I'm only masking the curvature on the larger forms that it's finding inside of the curvature map.
[5:48] So that's another way to go about using a generator.
[5:53] But what we're going to do instead is we're going to go and we're going to select this occlusion strong and we're just going to drop this on here.
[6:00] Right. So now you look at this and go, oh, wow.
[6:02] Well, you know, it's in all the cavities, which is what I expected and what I was looking for, which is a great place to essentially start from.
[6:11] But, you know, we might decide, OK, well, some of these areas, they're a little bit too strong.
[6:18] I don't really love what I'm getting in some of these areas.
[6:21] Well, you do have the ability to also modify this down here in your properties palette.
[6:26] You have a lot of controls that you can play with.
[6:28] The first is going to be your global opacity, which is obviously turning up or down the effect, your global contrast, which controls essentially the contrast of the opacity mask.
[6:41] So if I turn this all the way down, you can see we're starting to get a lot more gray values in there, right?
[6:46] But you also have the ability to tile some textures on top of the mask.
[6:53] So you also have the ability to enable a couple of different textures that will tile across this generator so that you can start to modify what they're doing, whether they're adding or subtracting detail to the mask.
[7:06] So that's a really great functionality and control that you do have from the generators as well.
[7:11] Now, where generators really become powerful is you have all of your bake maps that you baked out, you know, on your initial start of the project, your world space, your position, thickness, curvature, ambient occlusion, all of those.
[7:24] And you're given independent control over all of those textures to add influence to what the mask is deciding to do.
[7:32] So for example, if I came in here, you can see the ambient occlusion right here.
[7:37] So I was to take this and pull this down.
[7:40] It's pulling all of the information out from my cavities because I'm no longer getting an influence from the ambient occlusion, right?
[7:47] We also have the dropdowns where we can modify those independently, which is really nice and really powerful.
[7:54] So sometimes when I apply a generator, I get a result that may look good as a starting point, but there's certain aspects or elements to it that I may not love.
[8:04] Some of them might be like quite how much dust is getting collected.
[8:07] So I might come in here and potentially just start to like play with the contrast or even maybe bring down the balance.
[8:15] Or maybe I really want a lot of this stuff cranked into the cavities.
[8:19] So I will just modify my balance, play with that a little bit more.
[8:24] And then now I can come up here and play with my global balance and I can bring that up as I see fit.
[8:30] So this is another really powerful way to create a mask, which is definitely probably the most common method that most people use.
[8:38] Now, this isn't where I stop.
[8:41] I like to, you know, expand and really build complex masks with using all of these methods.
[8:48] But one other one that I also like to use, which is kind of dabbled in here is the use of texture maps.
[8:54] So this one's relatively straightforward and easy.
[8:57] So what I'm going to do is over here on my mask, I'm going to add a fill layer and I'm going to come to my textures.
[9:03] So in here, we have a bunch of grunge textures that are already natively inside of substance painter.
[9:11] So all of these are there and available to use again, like anything, I use a handful of them.
[9:17] I just have found a couple that I really like that get the results that I'm after, you know, pick and choose what work for you.
[9:25] But I have kind of my handful that I like to use.
[9:28] So, for example, let's look at maybe like grunge 13 is one that I usually use or actually even this like grunge dirt thin, but that one's that one's a little less crunchy than I think I want.
[9:42] So what we're going to do is we're just going to search grunge and let's look for grunge map 13.
[9:50] So we have 12.
[9:53] Yeah, we'll use 13.
[9:54] And what we're going to do is we're just going to drag and drop this into the grayscale.
[9:58] And you can see here that now we have this tile to cross the character.
[10:02] One thing that you'll notice right off the bat is there's a lot of seams, which can be fine.
[10:06] It depends on how you're building your masks and stuff.
[10:08] So this may not be a huge issue, but in this case, they're very obvious seams because I, you know, cut down the neck.
[10:16] I cut across the neck right here, cut up across the top.
[10:19] So that might not be the look that I'm necessarily after.
[10:22] There is a way to alleviate that, which is going to be the projection method.
[10:25] So we're going to come here and we're going to set this to tri-planar instead.
[10:28] And what this is going to do is it's going to project that map from different angles in order to alleviate that seam.
[10:34] You might notice there's a little bit of like funkiness happening.
[10:37] That's just from the projection.
[10:38] And, you know, it's not a huge deal.
[10:40] But what I will do next is I will just tile this a couple of times.
[10:45] And now you can see we have a result that feels pretty much seamless across our character.
[10:51] Now, if we switch into here, you can see all of the red is being revealed in those white areas.
[10:57] Maybe I want to make it a little bit more crunchy.
[10:59] So now I have the ability to come down to my grayscale map and I can play with the parameters down here.
[11:06] So I can lower my balance.
[11:08] I can increase my contrast, even the brush pattern I can play with.
[11:12] So there are procedural elements in a lot of these textures, which is really nice and useful to use when building your textures.
[11:19] So we drag and drop a different one on here.
[11:22] We have some of those same controls you can see.
[11:26] I can play with the contrast and the balance.
[11:29] There are some different texture maps that let's see scratches.
[11:39] You also have a little bit more procedural control over the final result.
[11:44] I think it's this one.
[11:45] Yeah.
[11:46] So you can see here we have a balance slider, but we also have a scratch quantity.
[11:51] So you can play with the number of scratches.
[11:53] You can play with the tiling of the scratches.
[11:55] You can blur the scratches.
[11:57] You can make them longer or thicker.
[12:00] You have a lot more control over some of these procedural textures, which is great.
[12:05] Scratches is one that I have a tendency of using pretty frequently and getting a pretty good result from it.
[12:12] So these are a couple of the methods that I like to use.
[12:15] Now, where things get really complicated with masking and what I like to do is I don't use usually any one of these specific things on their own and not take into consideration the other tools that I have.
[12:29] So like I mentioned, sometimes you maybe just want to make a simple map.
[12:34] So simple map.
[12:35] We decide, okay, I want to paint this.
[12:37] That's good.
[12:38] But there are sometimes where you want to make things a little bit more complicated.
[12:41] So let's go ahead and take a look at some of the masks that I made on this character that hopefully can kind of illustrate that.
[12:49] So the last and final method is taking all of those masking processes and techniques that I showed and combining them in one in order to create things a little bit more complex and unique and interesting.
[13:02] That kind of sell different sort of details that I need on my character.
[13:06] So we'll take a look at this one.
[13:08] This is a mask that I built for some of like the flaked skin on my character.
[13:13] So if you come in here, you can see which the texture is a little bit low res right now.
[13:19] So let me bump that up real quick.
[13:23] Okay, so now that that has finished thinking, you can see down here, I have like a couple of these spots which are like, like,
[13:31] skin or like build up on top of the scales that I wanted to add, right?
[13:36] So in order to do that, you know, you probably don't want it on the entirety of the character.
[13:41] I wanted it more localized to certain bigger scales and edges and just very specific areas, right?
[13:47] That was the initial intent behind it.
[13:49] So if we click on the mask, you can see this is what the mask looks like.
[13:53] There's a lot of like blacked out spots.
[13:55] There's areas located close to like the jawline a little bit around the eye.
[14:00] But point being the mask overall, this does not look like something that you're going to get just standard with a generator or a tile texture.
[14:09] So how do I go about building something this complex?
[14:12] Well, like I mentioned, I take all of those processes that I showed and I kind of package them together and build something with all of those techniques at once.
[14:22] So let's go ahead and just turn all of this stuff off.
[14:25] And you can see this is the initial mask that I started with, right?
[14:29] Now, once I have an initial mask, it doesn't always have to be perfect, but it's something that I feel like I can work off of.
[14:36] So I'm going to turn this back on and I'm going to make this a very obnoxious color so that we can really start to see what it's doing on top of the surface.
[14:48] So maybe that's not the best color and I'm going to turn up my opacity.
[14:54] So again, it is more obnoxious.
[14:58] So we'll do...
[15:02] Yeah, we'll do something like this. This works.
[15:04] So you can see the initial mask really doesn't look good.
[15:09] It's not delivering at all what I expect out of this mask.
[15:12] It's kind of just hitting the edges, hitting a couple of the top surfaces.
[15:16] Overall, doesn't look very good.
[15:18] So what I would do is I would start to layer on different things on top of this mask in order to get a final result.
[15:27] Now, with Substance, one of the powerful things comes from the fact that you can layer on top of layer on top of layer and you can really build something procedurally really quickly.
[15:37] Kind of how I showed stacking paint layers on top of themselves.
[15:40] That's essentially what I'm going to do is I'm going to create a generator or a mask and I'm going to continue to stack them on top of themselves so that I get something a little bit different.
[15:50] So you can see I added another mask on here, which this is brightening some stuff up.
[15:56] But what is really important once you start to deal with building your mask is you have to worry about the blending modes.
[16:03] Blending modes is something that I plan on talking about in the next video, hopefully.
[16:08] But what essentially is happening if I left this on normal, it's just taking the mask and replacing what's there.
[16:14] But I have it set to linear dodge, so that's combining the two masks.
[16:19] And you can see that I get the best of this mask and I get some of the values from this mask.
[16:26] So that's kind of what they look like independent of each other, but I'm combining them.
[16:30] Now, what I continue to do from here is I'm like, okay, there's definitely some stuff in here that I like, you know, I like some of these bigger shapes.
[16:38] I like some of this like medium gray value stuff and some of the cavities and crevices.
[16:43] But it's still not where I want to take it as a jumping off point.
[16:47] So what I'm going to do from here is I'm going to add another mask and I'm going to degrade a lot of the edges around what the mask has.
[16:56] So you can see this this has a lot of impact on what's actually happening.
[17:00] It's removing a lot of those edges.
[17:02] So if we were to turn both of these masks off and turn this one back to normal, you can see this is what the mask looks like.
[17:09] So I'm taking I'm creating a mask with a black and white edge so that I'm kind of hitting those edges or areas where I don't want the masking information to be.
[17:19] And I am taking that and I'm subtracting it from the information that's below it.
[17:24] So that's removing areas of white around edges and leaving me with some of this like kind of build up and things like that.
[17:32] So now you can see even just with those three smart materials, we're getting something that feels a little bit more complex.
[17:38] One thing that people tend to do when it comes to masking in substance painter is they leave the procedural texture without touching it after the fact this is good, but it's probably not where I would leave it.
[17:53] So I'm going to continue to break it up and refine it a little bit further.
[17:56] The first thing is just adding a sharpen on here.
[17:59] So this is just because I know that this is going to be kind of flaky and sharp edged, adding the sharpen sort of crunches the detail a little bit more.
[18:07] And then from here, adding a another mask on top of it, which is starting to remove bigger chunks.
[18:14] So I want something that's going to remove kind of big clumps of areas.
[18:17] You can see this area and down here starting to remove some of that.
[18:21] But from here, now we start to take those tileables into effect because I'm like, OK, I have a good starting point.
[18:28] Now let's add tileables over the top to start removing more information.
[18:33] So what I'm doing here is I'm just dragging a tileable on top of this and then I'm adding I'm subtracting from what's underneath it and playing with the values in order to get something that feels not procedural, more unique, more interesting, more varied over the overall surface.
[18:52] Now at this point, I would say that this mask feels very unique.
[18:56] It doesn't feel like it needs too much more in order to make it feel organic and natural.
[19:01] Whereas, you know, when I have something like this, this is hitting the entire surface doesn't feel very organic or natural.
[19:08] Just kind of feels like it's like a splat on top of the surface.
[19:12] But with all of these layers, we have something that looks more like this.
[19:15] And from here, adding another one, which is just removing more information, adding some value range with some of these grays while leaving some of the peaks of white.
[19:25] Now, where I usually finish things off is in a lot of cases, a mask like this just looks pretty good.
[19:32] But sometimes I want to have a little bit more control.
[19:35] And usually that's where the paint layer comes into play.
[19:38] So you can see here, what I'm doing is felt like there was a little bit too much kind of flaky skin in some of this area and maybe like some down here.
[19:48] So I just add a paint layer and take a little bit more control over where I have this stuff being applied.
[19:55] That's kind of me taking the ownership of the art direction of it deciding, OK, what makes sense?
[20:00] What does it make sense?
[20:01] Where do I want people to see this detail?
[20:04] Do I want it to be too overpowering or not overpowering?
[20:07] And usually it's more of less is more, you know, this is flaky skin.
[20:11] I want it to be a subtle detail that's kind of in the cracks and crevices and things like that.
[20:16] So then from here, the last thing that I do is just add a slope, a blur slope, which is just adding some irregularity to the edges.
[20:25] That's another thing that I want to talk about in a future video is just some of the use of filters that I use and kind of how I take them into account with my texturing process.
[20:34] Now, the last thing is just adding an anchor point on here because I know at some point, which in this case, right above it, I'm going to want to have another layer that's going to control some kind of functionality.
[20:44] I'm going to need to use this mask as a starting point.
[20:47] So we talked a little bit about this before, but here I'm taking the scale, the flaked information, this mask, and I am coming here using it as a starting point, playing with some levels, adding a fill to kind of degrade it.
[21:03] So it's only on the edges playing with a level.
[21:06] And you can see that I'm getting kind of some of those high points on the edges, and then I'm taking this mask as a another anchor point so that I can use that later down the line.
[21:16] So if I was to come here and really kind of crank that up, you can see what it's doing to displace the surface.
[21:23] So that's one of the examples of kind of creating a complex mask.
[21:27] I have another one here that is kind of doing the same thing.
[21:30] So we'll just step through this real quick.
[21:32] But initially, I'm starting with a curvature map.
[21:34] So you can see here, I plugged in my own curvature map.
[21:37] I started to modify the levels of it, use a dirt generator to really kind of amp some of those colors up, blur it, start layering on procedurals, breaking it down, running a levels on top of it, and then painting out areas that I don't want, and then adding an anchor on top because I know I'm going to reference it later.
[22:00] So then you get really, really complex masks like this, or like this, or any of these other masks that are on here, or sometimes you might just have a mask as simple as this.
[22:13] You know, I painted a couple of black dots.
[22:16] I added an anchor point, I blurred them, and then I referenced them later.
[22:20] So there's a lot of flexibility in masking, and it's something that you definitely want to get familiar with, and you don't want to just let the software do its thing.
[22:28] Usually, most of the time, you need to have some kind of hand authoring in the process of creating your maps.
[22:34] But overall, this is kind of the process that I take every character kind of requires something different.
[22:41] But hopefully you guys found this helpful.
[22:43] And if you guys haven't already, make sure to like and subscribe to the channel.
[22:47] I would greatly appreciate it.
[22:48] And I hope to keep presenting more cool stuff like this in the future.
[22:52] Hopefully you guys found this useful.
[22:54] Maybe you did.
[22:55] Maybe you didn't.
[22:56] It's a rather simple topic of masking, but I think it's something that's very overlooked by a lot of people in terms of how complex you can make it if you really choose to.
[23:03] So make sure to leave a comment below if there's anything you guys want to see in the future, and I will see you guys in the next one.
[23:09] Bye.



---

## Captured Frames

- [0:54] tutorials/frames/substance-painter-building-masks-explained/frame_000.jpg
- [1:12] tutorials/frames/substance-painter-building-masks-explained/frame_001.jpg
- [5:10] tutorials/frames/substance-painter-building-masks-explained/frame_002.jpg
- [5:53] tutorials/frames/substance-painter-building-masks-explained/frame_003.jpg
- [6:26] tutorials/frames/substance-painter-building-masks-explained/frame_004.jpg
- [9:54] tutorials/frames/substance-painter-building-masks-explained/frame_005.jpg
- [10:25] tutorials/frames/substance-painter-building-masks-explained/frame_006.jpg
- [11:39] tutorials/frames/substance-painter-building-masks-explained/frame_007.jpg
- [13:53] tutorials/frames/substance-painter-building-masks-explained/frame_008.jpg
- [15:50] tutorials/frames/substance-painter-building-masks-explained/frame_009.jpg
- [17:02] tutorials/frames/substance-painter-building-masks-explained/frame_010.jpg
- [20:44] tutorials/frames/substance-painter-building-masks-explained/frame_011.jpg

---

## Structured Notes

### Core Technique
Building complex, "hand-authored-feeling" masks in Substance Painter by layering multiple masking methods on top of each other (manual paint, generators, tileable/procedural grunge textures, blend modes, filters, and anchor points) instead of relying on any single one alone.

### Summary
Jared Chavez walks through every masking primitive in Substance Painter, from simplest to most complex, then shows how his own production masks (on a reptilian/creature head) are actually built by stacking all of them together. He starts with manual black/white mask painting, moves through generators (curvature, dirt/occlusion presets, and the full bake-map-driven generator: AO, curvature, position, thickness, world-space normal), then tileable/procedural grunge and scratch textures with tri-planar projection to kill seams, then shows how blending modes (e.g. Linear Dodge) combine multiple stacked masks, how paint layers add manual "art direction" on top of procedural results, and finally how anchor points let a finished mask be referenced as a driver for a later layer/effect. The end result is a "flaked skin" buildup mask on the creature's face that would be unachievable from any single generator or texture alone.

### Key Steps
1. **Simple manual mask:** right-click a fill/material layer -> context menu offers `Add black mask`, `Add white mask`, `Add bitmap mask`, etc. `Add black mask` creates a fully black mask (nothing visible); select the mask, pick the paint tool, and paint white directly onto the mesh in the 3D viewport to reveal texture only where painted.
2. **Isolate/view a mask channel independently:** Alt+click the mask thumbnail in the layer stack, OR use the channel dropdown next to the viewport and select `Mask`, OR tap `C` / `Shift+C` on the keyboard to cycle forward/backward through all channels (color, mask, individual PBR channels) — essential for judging a mask's actual grayscale values without the color layer in the way.
3. **ID-mask color-select masking (mentioned, not demonstrated on this mesh):** if a texture set has a baked ID map, you can color-pick specific IDs (e.g. "leather," "metal") directly from the ID map to build a mask instantly — this creature had no ID map baked so it wasn't shown live, but flagged as a fast method for hard-surface/multi-material characters.
4. **Stack paint layers on a mask non-destructively:** add multiple `Paint Layer`s on top of a mask (via the `+` at the bottom of the mask's sub-stack) so each pass of manual painting stays isolated and can be toggled off individually to revert without erasing work — described as "non-destructive" layered mask authoring.
5. **Generators — smart-material-style presets:** the Shelf/Assets panel has many pre-built generator mask presets (Chavez says he typically only relies on 5-6 of these) that drop on as a fast starting point/base, meant to be refined afterward rather than used raw.
6. **Generators — build your own via `Add Generator`:** opens a list including `Curvature` (drives off the baked curvature map; expandable to independently control small-detail vs. large-detail curvature response) and `Dirt`/occlusion-style presets (e.g. "Occlusion Strong," driven by the baked Ambient Occlusion map, collects in cavities).
7. **Generator properties palette controls (bottom-left panel when generator/mask selected):** `Global Opacity` (overall strength), `Global Contrast` (contrast of the resulting grayscale mask — pulling it down flattens toward more mid-gray values), `Balance` (shifts where in the range detail collects), plus independent sliders for every baked mesh map feeding the generator (World Space Normal, Position, Thickness, Curvature, Ambient Occlusion) — each can be dialed up/down or disabled to change what drives the mask. Optional tileable texture inputs can also be layered onto a generator to add/subtract extra procedural detail.
8. **Tileable/procedural grunge & scratch textures as a mask layer:** on the mask's sub-stack, add a `Fill Layer`, then drag a texture from the built-in Textures/Grunge shelf (e.g. `Grunge Map 13`, `Grunge Dirt Thin`) into the fill layer's Grayscale slot — this tiles the pattern across the whole mesh via UVs.
9. **Fix UV-seam artifacts from tiled textures:** change the fill layer's `Projection` mode from the default UV-based projection to `Tri-planar` — this projects the texture from three world-space axes instead of following UV seams, eliminating the visible seam break (e.g. across the neck cut) at the cost of some minor per-axis blending "funkiness"; increasing the `Tiling` count tightens the pattern until it reads as seamless.
10. **Procedural texture parameter control:** grunge/scratch textures expose their own grayscale-map parameters in the properties panel — `Balance` and `Contrast` on grunge maps; on more procedural ones like the "Scratches" texture: `Balance`, scratch `Quantity`, `Tiling`, `Blur`, and scratch length/thickness — Chavez calls Scratches one of his most-used, reliable procedural picks.
11. **Blending modes combine stacked masks:** stacking a second generator/mask directly on top of a first (both inside the same mask's sub-stack) and changing the top one's blend mode from `Normal` (replaces) to `Linear Dodge` (adds/combines) merges the grayscale information of both rather than one overwriting the other — described as the key mechanic (with a "next video" teaser) for combining multiple generator passes into one richer mask.
12. **Edge-degrade pass:** add another mask/generator specifically tuned to hit edges (a black-and-white edge mask), set to subtract from what's below it — removes white detail specifically at edges/rims, cleaning up over-strong generator results.
13. **Refinement filters:** add a `Sharpen` filter on the mask stack to crunch/tighten detail (used here because the target look — flaked/cracked skin — needed harder edges); add further generator/tileable subtract passes to break up large uniform clumps into smaller, more organic, non-repeating clusters.
14. **Final manual art-direction pass:** add one more `Paint Layer` on top of the whole procedural mask stack to manually erase/reduce the effect in specific areas where the procedural result reads as "too much" — Chavez frames this as reclaiming art-directorial control ("less is more") rather than trusting the procedural stack blindly. Finish with a `Blur Slope` filter to add irregularity to the remaining hard edges.
15. **Anchor point as a mask-reuse mechanism:** once a complex mask is finished, add an `Anchor Point` on that layer so a later layer/effect elsewhere in the stack can reference this exact mask as an input (e.g. feeding it into a `Levels`-adjusted fill to drive edge-only detail, or into a height/displacement-driving effect) — lets one hand-built mask be reused as a mask *source* multiple times downstream without rebuilding it.
16. **General philosophy stated repeatedly:** don't rely on any single masking method (paint-only, generator-only, or texture-only) in isolation — production-quality complex masks come from combining manual painting + generators (bake-map-driven) + tileable procedural textures + blend-mode stacking + filters + anchor-point reuse, refined iteratively, with the artist always making a final manual pass for art direction.

### Layers / Tools / Settings
- **Mask creation:** right-click layer -> `Add black mask` / `Add white mask` / `Add bitmap mask`
- **Mask sub-stack additions:** `Paint Layer`, `Fill Layer`, `Add Generator`, `Add Effect`/filters (`Sharpen`, `Blur Slope`), `Anchor Point`
- **Generators used/shown:** `Curvature` (with small-detail/large-detail split control), `Occlusion Strong` (AO-driven preset), a custom edge-detecting generator for edge-degrade
- **Generator/mask properties palette fields:** `Global Opacity`, `Global Contrast`, `Balance`, per-bake-map influence sliders (`World Space Normal`, `Position`, `Thickness`, `Curvature`, `Ambient Occlusion`), optional tileable-texture add-ins
- **Fill-layer texture inputs:** built-in Grunge shelf textures (`Grunge Map 13`, `Grunge Dirt Thin`, `Scratches`), dropped into the Grayscale slot
- **Fill-layer `Projection` dropdown:** default (UV-based) vs `Tri-planar` (seam-free world-space projection), plus `Tiling` count
- **Scratches texture parameters:** `Balance`, scratch `Quantity`, `Tiling`, `Blur`, length/thickness
- **Blend modes:** `Normal` (replace) vs `Linear Dodge` (additive combine) demonstrated for stacking two masks
- **Channel isolation:** Alt+click mask thumbnail, viewport channel dropdown -> `Mask`, or `C`/`Shift+C` hotkeys to cycle channels
- **Filters:** `Sharpen`, `Blur Slope`
- **Anchor Point:** added on a finished mask layer so downstream layers/effects can pull it as a mask source

### Difficulty
Intermediate to Advanced — the individual tools (paint mask, generator, fill layer with grunge texture) are beginner-accessible, but the video's real content is the *combination strategy* (stacking generators with blend modes, tri-planar seam fixes, anchor-point reuse) which assumes the viewer already knows the layer-stack basics.

### App & Version
Not stated explicitly in the video or visible in any captured frame (no version string shown in title bar or About dialog). The UI matches the classic Substance Painter layer-stack + generator-properties layout (right-click context mask menu, generator `Projection`/`Tiling` fields, no Skew-specific baking/painting controls, no OpenPBR-labeled shader) — consistent with the Painter 8.x-11.x era per `references/version-tracker.md`, but this is an inference from UI layout only, not a confirmed version. Treat "App & Version" as **not specified — approximate pre-12.1 UI era**.

### Tags
masks, layers, paint-layer, fill-layer, generator, smart-mask, curvature, ambient-occlusion, mesh-maps, tri-planar, procedural, alpha, blend-mode, anchor-point, intermediate, advanced

---

## Related Tutorials
- [REALISTIC CREATURES: HAND PAINTED TEXTURES in SUSTANCE PAINTER](realistic-creatures-hand-painted-textures-in-sustance-painter.md) — same creator; that video's edge-detect peeling-skin mask (step 13) and repurposed-material rash detail (step 10) apply this video's generator/blend-mode masking toolset in a production context.
- [How to TEXTURE in SUBSTANCE PAINTER | Creature TEXTURING](how-to-texture-in-substance-painter-creature-texturing.md) — same creator; the gradient-mask and blend-mode-stacking fundamentals covered here (Key Steps 7, 11) underlie the gradient-mask hand/arm work and layered discoloration patches in that video's Key Steps 13 and 15.
- [How to TEXTURE EVERYTHING in Substance Painter](how-to-texture-everything-in-substance-painter.md) — different creator (J Hill); a much longer (3h19m), full-project demonstration of the same anchor-point-as-mask-source technique introduced here at [20:44] — that video uses one paintable "control" anchor to simultaneously drive color, primer-reveal, and edge layers across an entire helmet's paint/leather/decal passes (Key Steps 21-28, 35-37, 48), and adds the `Bevel Smooth` filter (not covered in this video) as a way to turn a hard anchor-driven mask into a soft, physically-offset edge.
- [TEXTURING METAL from Scratch in SUBSTANCE PAINTER](texturing-metal-from-scratch-in-substance-painter.md) — same creator; a live production application of this video's generator-then-manual-breakup principle (edge wear generator, then a paint layer to break contiguous lines) and its anchor-point-as-mask-source technique (used there for the final rust-edge flake/peel pass).
- [How to TEXTURE like a PRO with ANCHOR POINTS | Substance Painter Tutorial](how-to-texture-like-a-pro-with-anchor-points-substance-painter-tutorial.md) — same creator; a dedicated deep-dive expanding the single anchor-point-as-mask-source use case shown here at [20:44] into three full production use cases (pattern-variant reuse, utility-map forward-planning, modular library materials).
- Additional cross-links to other Jared Chavez tutorials in this knowledge base that build on the same masking primitives shown here (hand-painted texture videos reference this video's generator/blend-mode/anchor-point stack; the anchor-point-focused videos reference this video's anchor-point-as-mask-source technique introduced at [20:44]) will be added as those sibling tutorials are ingested. See `tutorials/INDEX.md` for the full current list.
- [Texturing a Cyberpunk Building in Substance 3D Painter – Project Breakdown](texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s.md) — different creator (Adobe Substance 3D); a fast-paced production application of this video's generator/tri-planar/anchor-point masking toolkit across a whole building's brick, concrete, fabric, and tile materials.
- [Creating & Reusing Smart Materials in Substance 3D Painter | Stylized Crab](creating-reusing-smart-materials-in-substance-3d-painter-stylized-crab-adobe-sub.md) — different creator (Adobe Substance 3D); assumes this video's tri-planar/anchor-point masking fundamentals are already in place, then shows how to package a finished layer stack built from them into a portable, reusable Smart Material.
