---
title: Speeding Up Character Texturing with Smart Masks - Substance Painter
source: YouTube
url: https://www.youtube.com/watch?v=qkRJjA5rTcY
author: FlippedNormals
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated numerically; scattering (subsurface) channel added manually via Texture Set Settings > Channels > \"support by shader,\" consistent with a modern shader-driven channel model, tentative"
tags: [layers, fill-layer, paint-layer, masks, smart-mask, blend-mode, basecolor, roughness, height, alpha, texture-set, pbr, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/speeding-up-character-texturing-with-smart-masks---substance-painter/
frame_count: 10
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Speeding Up Character Texturing with Smart Masks - Substance Painter

**Source:** [YouTube](https://www.youtube.com/watch?v=qkRJjA5rTcY)
**Author:** FlippedNormals
**Duration:** 17m2s | 5 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hi, this is Henning from FlipNormals and in today's video we are going to show you a
[0:06] really cool tip for speeding up your work when it comes to texturing characters.
[0:11] We are going to be using smart masks, which is a very powerful tool when it comes to quickly
[0:17] changing things in your model, quickly blocking out your model and quickly making additional
[0:22] maps like the spec R and subsurface amount.
[0:26] Before we get into the tutorial, I want to talk to you about character face texturing
[0:29] in Substance Painter.
[0:30] This is a course where you learn how to make this character from scratch in terms of the
[0:34] textures, from exporting out the mesh from Seabrush to creating every single map in Painter,
[0:41] to exporting all the maps into Arnold for Maya, which you can also do in Blender and
[0:46] all of our software and then we have a nice final result at the end.
[0:51] Also the model we use in this video and same for the course as well is made by Niazi, there's
[0:56] a link to his portfolio in the video description, his work is fantastic so highly recommend
[1:00] you check that out.
[1:01] Now in Painter, I'll show you how to set up a smart mask.


### Smart Masks [1:02]
**Transcript (timestamped):**
[1:04] Now if you already know how to set up smart masks, don't skip out on video yet because
[1:07] I'm going to show you how to use the smart masks, which is much more than just how to
[1:11] technically set them up.
[1:13] So the way we are going to be making a smart mask is we are going to be making a new filler,
[1:17] we are going to be grouping this and we are just going to call this smart masks and then
[1:21] we are going to put this in here and we are going to call this base.
[1:25] And then we are going to make another layer, just duplicate this one and the only thing
[1:29] we really want here is color so we can just all click on the color and we are going to
[1:32] make this nice and red.
[1:34] Basically we just want a nice saturated color, then we just click this way so that's fine
[1:39] and then we are going to call this red.
[1:41] I prefer to name my things very early on.
[1:44] Then we are going to right click on this red layer and then we are going to go to add black
[1:48] mask and now this is where you can paint and whatever you paint is now going to be red.
[1:53] So we are going to be adding a paint layer and then this is where you can just paint
[1:57] in the red.
[1:58] And the gist of this is that we are going to be creating a lot of these ones, a lot of
[2:01] these masks, we are going to be saving them out as smart masks and now we can keep reusing
[2:07] these masks over and over again.
[2:09] So we are going to be starting off by just making a mask for the general eye area.
[2:15] This is going to be quite soft and nice and it's really important that you have something
[2:20] like a saturated color whenever you make this mask because honestly it's going to be hard
[2:25] to see them otherwise.
[2:28] Like you want to be sure that it's a completely clean mask.
[2:30] The brush I'm using is just a standard soft brush but then I set the pen pressure to be
[2:35] on the flow and not on the size because I have more control this way.
[2:39] So meaning I have more control over the softness this way.
[2:43] And then we just go down here all the way to the bottom and here you can see if we were
[2:46] to change this from black to white by hitting the X key we can now just paint in and we
[2:52] can remove stuff as well.
[2:54] So that's the gist of this.
[2:55] Once you paint to your mask you want to hit the alt key, hold the alt key and click on
[2:59] the mask so now you can see exactly what's actually going on because this way you can
[3:03] ensure that you get nice and clean masks.
[3:05] It's really hard to see this properly whenever you are working with just a material view.
[3:11] It can also be easy to miss certain areas.
[3:14] In this case it's inside the eye so this is not a huge concern but yeah this is how I
[3:18] do it.
[3:19] So then I'm going to rename this paint layer to eye soft and then we are going to right
[3:27] click on the layer and then we're going to go to create smart mask and then you can see
[3:33] this is going to pop up here.
[3:34] Now it's important you have to be under the smart mask tab here, filtered by that, right
[3:41] click and then we're just going to call this, I'm going to call this CHR first just so we
[3:45] can search for character and then we're going to call this eye soft.
[3:50] And what's cool about this now is that now if we were to delete this, now we can very
[3:54] easily get this back just by searching CHR and just drag this in here and now you can
[3:58] see we have the same mask.
[4:00] So we are just going to create a few of these which is going to really really speed up your
[4:06] texturing.
[4:07] So we are just going to use this one as a base so just make sure you are on the actual
[4:15] layer and you're not on like in the like on the mask itself.
[4:20] So we can just create one for the eyelids.
[4:25] So I think it's important to reuse as much as you can.
[4:29] So like this, we're going to keep this a bit quicker for now but just make sure here you
[4:35] go you can see that there is an issue with this.
[4:37] So we just want to make sure that this is nice and soft, cool.
[4:42] And then we're going to call this eye, eyelids.
[4:44] They're the same thing as before.
[4:47] So now we just go in and we just do actually there's a little bit of discrepancy here so
[4:51] we just go in, make sure this is set.
[4:54] Then we right click on the layer and then we do create smart masks.
[5:00] Do the same thing as before and we just do CHR.
[5:05] We do eyelids.
[5:06] Then we do the same again.
[5:08] And I'm just going to create like one more for the mouth and then you can make your own
[5:12] one or I'm just going to be doing it behind the scenes because this is just the same thing
[5:17] over and over and over again.
[5:19] There's really nothing fancy about this.
[5:24] It's very simple once you get this workflow.
[5:27] And the reason this works particularly well for characters versus hard surface.
[5:31] Now it does work well for hard surface as well but particularly reason this works for
[5:35] characters is that for characters you basically work within like this region here most of
[5:40] the time, right?
[5:41] You usually work within the eyes, nose, mouth, ears and you know the surrounding area.
[5:48] And that's what you do most of the time while on props you work a bit more all over the
[5:53] place and you don't just keep repainting the same areas as much as you do with characters.
[5:58] So it's really powerful to use this with characters but of course you're more welcome to use this
[6:03] for props as well or hard surface.
[6:06] So we're going to call this mouth.
[6:08] Then we're going to right click.
[6:10] We're going to set this to, you guessed it, create smart mask.
[6:14] And then same thing, CHR.
[6:20] So the advantage we have with this is that we can very easily start to block in the characters.
[6:24] I'm going to show you the procedure for this in a second.
[6:28] But now I'm just going to skip a little bit ahead.
[6:30] I'm going to make a few smart masks myself.
[6:32] All right, cool.


### Block In [6:33]
**Transcript (timestamped):**
[6:33] So I've now deleted the overall smart mask group and I've made a few of these.
[6:38] So we have the eyelids, the eyelids, the eyes sharp, the eyes soft.
[6:43] We have horns, ears, mouth, nose.
[6:47] So essentially we have things for this region.
[6:53] So we have for this, we have for this, we have for the lips, we have for the ears, we
[6:58] have for the horns.
[7:00] And what you might want to do is also for characters like this is like for the scars
[7:03] as well.
[7:04] We haven't done that.
[7:05] And you also sometimes want for like the overall T zone here as well.
[7:07] So you have a bit more control of the spec there as well.
[7:10] And you probably also want these things.
[7:12] We haven't done that for now.
[7:13] So I'm going to show you how you can use these masks to quickly block in first, just a color
[7:19] map of your character.
[7:20] So under color, we have a few different fill layers already.
[7:23] We have the red, which is just, there's nothing in here because the mask isn't there.
[7:27] So if we just were to kill the mask, then it's going to look like this.
[7:31] So what we can do for this is make a eye soft and we can just put this under here.
[7:35] And now you can see we instantly have the color for this.
[7:40] We can do the same thing for the mouth as well.
[7:42] Now we're going to have instant lips as well.
[7:45] Do the same thing for the nose.
[7:48] And you can just see how quick this is to block this in.
[7:51] And of course we can change the opacity of these as well.
[7:54] So really useful stuff.
[7:58] So if you want, for instance, to have horns that are darker, you can easily do that.
[8:01] You can go over here and you can just drag the horns in and I can see that we have horns
[8:05] that are darker right away.
[8:08] If you want, for whatever reason, you want ears that are like more towards green, a bit
[8:15] desaturated, darker because it's more of a fantasy character.
[8:20] We can go in here, we can do the same thing with the ears as well.
[8:25] Just drag this in and there we go.
[8:27] And the cool thing about this approach is that you can very easily change this up.
[8:30] So oh, you don't want green, that doesn't work super well.
[8:32] Well, we can just color pick something else and then we can easily just change this up.
[8:38] And then we have it.
[8:39] So again, another advantage of this is that these masks are not actually live.
[8:45] So if we want to change, for instance, where the nose goes or let's say we want the eyes.
[8:54] So currently we have a mask for the eyes.
[8:57] But if we update this one, it's not going to update here, which is great because this
[9:01] means we can use the starting point.
[9:03] We can blend this in, for instance, or we can extend this up like so.
[9:07] So it's a very quick way of blocking things in like so.
[9:11] And I use this for all my characters essentially.
[9:14] So that's it.


### Roughness [9:15]
**Transcript (timestamped):**
[9:15] How we can use this for the color map.
[9:17] Now where this is really useful as well is for if we want to do something for the specular
[9:21] map, for instance, so let's go into our roughness.
[9:25] So now we can just make a roughness or new filler and we can call this mouth.
[9:31] And then we can just all click on roughness and we can make this quite a smooth.
[9:37] Roughness value.
[9:38] And then we just go in here and we just go in and we go boom.
[9:41] And I can see we have instant roughness map or a mask for the mouth.
[9:46] We can do the same thing or you can just like duplicate this one.
[9:48] We can call this eyes.
[9:50] We can just delete what we have.
[9:52] And then we can just set this to be even an even lower value.
[9:55] We want the eyes to be super sharp, for instance, or maybe a little bit higher up.
[9:59] Then we can do eyes soft.
[10:01] And we just drag this in and boom, we now have this.
[10:04] Then we want the eyes, the actual like shelf here to be even, to be even harsher.
[10:11] Then we can go in here and we can make this be even darker like so.
[10:15] So we can go in and we can do eye sharp, drag this in and there you go.
[10:19] You can see that now if we were to go in and check our spec map, you can see that
[10:23] we can now go in and we can really just play around with this.
[10:28] Maybe the specular value for this is, is too sharp.
[10:32] So we can just go in and we can just quickly change this up.


### Subsurface [10:35]
**Transcript (timestamped):**
[10:35] And you can see how fast this actually is.
[10:37] Obviously, you still have to work on the color map and on the spec map and such.
[10:40] But it just means that you can very quickly get a base.
[10:43] Another one you can use is the subsurface amount as well.
[10:47] Because we keep seeing that we're going to use the same things over and over again.
[10:50] So just hit the C key a few times until we get to the scattering channel.
[10:53] If you don't have a scattering channel, you just have to go to the texture sets
[10:56] and then go to channels.
[10:57] And then we just have to go to a channel on support by shader.
[11:00] And then we just have to get scattering in here.
[11:03] So then we have scattering.
[11:05] So we have a base value for the scattering, but what if we want this to be a different
[11:09] value? What if we want the eyes to be, uh, let's say we take this down.
[11:13] So we want this to be like kind of nice and neutral, but we want the ears to be
[11:17] really, really shiny or sorry, really, really absorbing a lot of, um, of subsurface.
[11:23] Then we go in here and we just go, boom.
[11:25] And then we have this for the ears.
[11:27] Do the same thing.
[11:28] We can just duplicate this one and delete layer we have and we can, let's say we
[11:33] want the mouth to be, to be a subsurface, but not that much.
[11:38] We just go in and go, boom.
[11:41] Do the same thing for the, um, for the eyes as well, cause you want them to be a
[11:46] little bit specky or sorry, a little bit, um, uh, subsurface.
[11:53] And there you go.
[11:53] You can just see how you can very quickly create this.
[11:55] Now this is not connected to anything, but at least the point is here.
[11:59] And then of course we want the, uh, the horns to not have any scattering
[12:02] whatsoever cause the horns, then we just go in and we just go, boom.
[12:05] And now we have horns that are basically anything on it.
[12:09] So this is a bit of a different approach to how, how you might normally do it.
[12:13] A normal approach might be to just go, well, I want horns to be darker.
[12:18] So I'm just going to go in.
[12:19] I'm just going to paint this kind of stuff in.
[12:21] So, you know, just going to start to straight up paint that was in color.
[12:24] We need to make sure this is a scattering.
[12:26] So you just go in and you just paint this.
[12:27] The problem is you can't really change the value of this.
[12:29] You can't really quickly block it out either.
[12:32] You can't really, you can't erase it with the eraser brush, but it's much,
[12:35] much better to do these kind of maps with fill layers and, um, using the smart mask.
[12:44] So this has so much potential.
[12:46] So before you start any character, I highly recommend that you go in and you
[12:50] spend like half an hour or so.
[12:53] That's about how much time it takes to create these masks from scratch.
[12:56] Cause I've timed that for more tutorials.
[12:58] So just spend a lot of time doing that.
[13:00] And if you find yourself painting something, let's say you, we are in the color and we
[13:05] realize that, um, we keep doing the same thing over and over again.
[13:10] Let's just put it here and we, we keep doing the same thing.
[13:13] So let's say we want to have some darkness and the scars and we just make a black mask
[13:19] and we do this.
[13:20] We had a paint layer and we keep doing this over and over again, because we just
[13:23] don't want some values in this.
[13:25] Well, what you should then do is you just do the same thing.
[13:28] You just take what you keep painting all the time, then right click on it and
[13:32] then just turn this into a smart mask and you can find her all here.
[13:36] If you want to delete the smart mask, you simply as right click on it and then
[13:39] you delete.
[13:40] Now, if you for whatever reason, you can't find this like you, you don't, you
[13:43] can't delete it through here.
[13:45] You can just search through your windows machine to smart mask or to the name of
[13:49] this and you're going to find the file and it's going to be under your assets
[13:53] and smart masks under your painter directory.
[13:56] So then you can just delete it from there as well.
[13:58] Another thing you can do with this as well is if you want to grade the, um,
[14:03] the textures for whatever reason, let's see, you have a height map and, um,
[14:07] we have a height map that looks like so, but we want to reduce the intensity of
[14:11] this is actually what I'm doing with the height balance here.
[14:13] So let's make another layer and we just set this to height, click the, um,
[14:17] just click the alt key or clicking on it.
[14:20] Then we change the blending mode to height.
[14:22] So we can actually adjust this.
[14:23] Then we just set this to normal and I can see there's nothing here.
[14:26] So if we go to the material view, there's nothing.
[14:29] So, uh, this is a good way to do it, to balance things out.
[14:32] So now what we can do, let's say we want the, um, the eyes to be, um, to be less
[14:38] intense when it comes to the amount of bump there is, we can just set this to
[14:43] be like balance eyes.
[14:46] And then we can just drag in the eyes soft for this.
[14:49] And I can see this is now excluding everything, but the eyes.
[14:53] The important thing is that you do set this to normal.
[14:55] And then you can just set the opacity just a little bit down.
[14:58] So this is a great way to balance things out.
[15:01] Can do the same thing with the, uh, the nose as well.
[15:05] If you want this to be a little bit less intense, what you can also do,
[15:09] you can set this to max and then we can just change the amount here as well.
[15:13] This we have finer control over this.
[15:16] So yeah, that's, this is a good way of doing it.
[15:18] Uh, you can do this exactly the same thing.
[15:20] If we were to use, go to color as well, and we want to change, uh, something
[15:26] like an adjustment layer, or we want to change the amount of something.
[15:29] We want to change the saturation in certain area.
[15:32] Then we can just make a, um, a regular paint layer.
[15:35] And then in here, we can add levels to this.
[15:38] And then we just set this to, uh, to pass through this in color.
[15:42] And we just go under here and we just set this to pass through.
[15:45] Now you should be able to change the, the grading of this.
[15:48] So we want a whole thing to, well, now we make the whole thing darker.
[15:53] And then we just go in, call this grade, and then we can go in and we can just
[15:57] change this to be eyes soft.
[15:59] And now you guessed it, this is only going to grade down this one.
[16:03] So tremendously powerful when it comes to, um, to doing, well, particularly
[16:10] characters, it's useful for all sorts of texture, but particularly for characters.
[16:13] This is really, really handy.
[16:15] So that's it for this video.
[16:17] If you did enjoy this video, I really recommend our course face
[16:21] texturing in substance painter, which covers a lot of the same concepts where
[16:25] we also cover how to do the whole thing, including how to do the, the, the normal
[16:30] map you can see are doing all the pores.
[16:32] And then we take all the maps into, into Arnold and we rendered them out there.
[16:36] But again, if you are using another software than, than Maya and Arnold,
[16:40] these maps are going to work perfectly fine.
[16:43] So yeah, thank you so much for watching.
[16:44] If you did enjoy this, let us know in the comments and make sure to like,
[16:49] comment and subscribe and hit the little notification bell to get updated every
[16:53] single time we come out with a new video.



---

## Captured Frames

- [1:44] tutorials/frames/speeding-up-character-texturing-with-smart-masks---substance-painter/frame_000.jpg
- [3:19] tutorials/frames/speeding-up-character-texturing-with-smart-masks---substance-painter/frame_001.jpg
- [3:41] tutorials/frames/speeding-up-character-texturing-with-smart-masks---substance-painter/frame_002.jpg
- [7:20] tutorials/frames/speeding-up-character-texturing-with-smart-masks---substance-painter/frame_003.jpg
- [8:05] tutorials/frames/speeding-up-character-texturing-with-smart-masks---substance-painter/frame_004.jpg
- [9:25] tutorials/frames/speeding-up-character-texturing-with-smart-masks---substance-painter/frame_005.jpg
- [10:19] tutorials/frames/speeding-up-character-texturing-with-smart-masks---substance-painter/frame_006.jpg
- [11:00] tutorials/frames/speeding-up-character-texturing-with-smart-masks---substance-painter/frame_007.jpg
- [14:17] tutorials/frames/speeding-up-character-texturing-with-smart-masks---substance-painter/frame_008.jpg
- [15:35] tutorials/frames/speeding-up-character-texturing-with-smart-masks---substance-painter/frame_009.jpg

---

## Structured Notes

### Core Technique
Pre-build a one-time library of hand-painted, character-region **Smart Masks** (eye soft, eyelids, eye sharp, mouth, nose, ears, horns, etc.) saved once, then reuse each mask across every channel — Color, Roughness, Height, and Scattering/Subsurface — of a new character by simply dragging it into each new Fill layer's mask slot. Because each drag-in creates an independent, non-live copy of the mask data (not a linked reference), the same regional shape can carry completely different values per channel and be locally fine-tuned afterward without disturbing the original saved mask.

### Summary
Demonstrated on a horned fantasy-character bust (model credited to artist Niazi). **Building the mask library:** create a Fill layer inside a temporary "smart masks" group, give it a strongly saturated flat color (important for visibility — muted colors make mask edges hard to judge) and only enable the Color channel via Alt-click, add a black mask, add a Paint sub-layer, and hand-paint the target region (e.g. a soft eye-socket falloff) using a soft round brush with **pen pressure mapped to Flow rather than Size** for finer control over softness/opacity buildup; press `X` to swap between painting black (remove) and white (add). Alt+click the mask thumbnail to preview it in isolation (essential for verifying clean edges — hard to judge accurately in material/shaded view, and easy to miss small gaps like inside the eye opening). Rename the finished paint layer descriptively (e.g. "eye soft"), then right-click it and choose **Create Smart Mask** — save under the Smart Mask tab specifically (not Smart Material) with a consistent naming prefix (the video uses `CHR_` for "character") so the whole reusable set stays groupable and searchable later. Repeat for each recurring facial/character region: eyelids, eye sharp (a harder-edged variant of eye soft for crease/shelf definition), mouth, nose, ears, horns — the video argues this workflow suits **characters specifically** more than hard-surface props, because character texturing repeatedly revisits the same handful of anatomical regions (eyes/nose/mouth/ears and immediate surroundings), whereas prop texturing tends to spread work more evenly across the whole surface. **Reusing the library:** once saved, search the asset browser by the naming prefix and drag any smart mask directly into a new Fill layer's mask slot — Color-channel blocking becomes near-instant (drag "eye soft" under a skin-tone Fill layer, "mouth" under a lip-color layer, "horns" under a darker horn-color layer, etc.), and because copies are independent, adjusting one channel's color/coverage never disturbs another channel's use of the same region, and even editing the *original* saved smart mask afterward does not retroactively change any already-placed copy (useful for it to serve purely as a reusable starting point that gets blended/extended per-use). The exact same drag-in-a-smart-mask pattern is repeated for **Roughness** (distinct roughness values per region: soft/matte lips vs. sharp/shiny eye-shelf highlights) and for **Scattering/Subsurface** (added as a channel first via Texture Set Settings > Channels > "support by shader" if not already present, then per-region SSS intensity set directly rather than painted — full for skin-toned areas, zero for horns) — argued as strictly better than hand-painting these auxiliary maps directly, since a painted-in value can't be cleanly re-scaled, block-adjusted, or erased with the same control a Fill-layer-plus-mask setup gives. **Bonus grading technique:** to locally dampen an existing effect (e.g. reduce Height-channel bump intensity, or grade down Base Color saturation/darkness) only within one of the already-established regions, add a new Paint layer scoped to the relevant channel, add a `Levels` filter on it, set the layer's blend mode to **Pass Through** (so the Levels adjustment reads/affects the layers beneath it rather than compositing as its own new value), then mask that grading layer with one of the same reusable smart masks (e.g. "eyes soft") to confine the correction to just that region — described as "tremendously powerful" for fine local balancing after the initial block-in.

### Key Steps
1. **Build each reusable region mask from a saturated, single-channel Fill layer:** new Fill layer inside a temporary group, Alt-click to isolate the Color channel only, set a strongly saturated flat color (critical for visibility while painting/verifying), add a black mask, add a Paint sub-layer.
2. **Hand-paint the region with a soft brush set to Flow-based pen pressure** (not Size-based) for finer control over edge softness; use `X` to toggle between painting black (remove from mask) and white (add to mask).
3. **Verify the mask is clean by Alt+clicking its thumbnail** to preview it in isolation — material/shaded view alone makes it too easy to miss small gaps or leave a messy edge.
4. **Rename the finished paint layer descriptively before saving** (naming discipline done early, e.g. "eye soft") — right-click the layer and choose **Create Smart Mask** (confirm you're saving under the Smart Mask tab, not Smart Material), using a consistent searchable prefix (`CHR_` in this video) across the whole set.
5. **Repeat for every character region reused across a typical face/character build:** eye soft, eyelids, eye sharp, mouth, nose, ears, horns (or equivalent regions for a different character type) — budget roughly half an hour to build a first complete library from scratch (timed by the creator across multiple projects).
6. **Reuse the library for fast color block-in:** search the asset browser by the naming prefix, drag a saved smart mask directly into a new Fill layer's mask slot, and adjust that Fill layer's own color — repeat per region to block in a full base color pass in minutes; each drag-in is an independent, non-live copy, so later edits to the original saved smart mask (or to one placed copy) never propagate to other already-placed copies.
7. **Blend/extend a dropped-in smart mask locally when needed** (e.g. push a nose-mask's coverage further up the bridge) rather than treating it as fixed — the point of the library is a fast, editable starting point, not a rigid final shape.
8. **Reuse the exact same masks for Roughness:** new Fill layer scoped to Roughness only, drag in the relevant region mask (e.g. "mouth" for smooth/matte lips, "eye sharp" for a harder specular shelf around the eye), and set distinct roughness values per region.
9. **Reuse the same masks for Scattering/Subsurface:** if the Scattering channel isn't already present, add it via Texture Set Settings > Channels > add a channel supported by the active shader ("support by shader"), then for each region drag in the matching smart mask and set a direct subsurface-intensity value (not hand-painted) — full SSS for skin, none for horns, etc.
10. **Use a Pass-Through Levels layer + a reused smart mask for local grading corrections:** add a new Paint layer on the target channel (e.g. Height, to reduce bump intensity in one area, or Base Color, to darken/desaturate one area), add a `Levels` filter to it, set the layer's blend mode to **Pass Through** so the Levels adjustment reads from the layers beneath rather than replacing them, then mask that grading layer with a saved smart mask (e.g. "eyes soft") to confine the correction to exactly that region.
11. **Promote any frequently-repainted pattern into a new smart mask as you notice it** — if you catch yourself hand-painting the same kind of detail (e.g. scar darkening) repeatedly across a project, right-click that paint layer and save it as a smart mask immediately rather than continuing to repaint it by hand.
12. **Manage the saved library directly on disk if needed:** smart masks not deletable from within Painter's asset browser for any reason can be found and removed manually under the Painter install's `assets/smart masks` directory (or the equivalent custom-assets path), searchable by the same naming prefix used when saving.

### Layers / Tools / Settings
- **Mask-building layer:** Fill layer (Color-only via Alt-click), saturated flat color, black mask + Paint sub-layer, soft brush with pen pressure mapped to Flow
- **Save/reuse:** right-click > Create Smart Mask (Smart Mask tab, not Smart Material), consistent naming prefix (e.g. `CHR_`) for searchability
- **Verification:** Alt+click mask thumbnail to preview the mask in isolation
- **Reused across channels:** Color, Roughness, Height, Scattering/Subsurface — each channel's Fill layer gets its own independent drag-in copy of the same saved mask
- **Scattering channel setup:** Texture Set Settings > Channels > add a channel "support by shader"
- **Local grading trick:** Paint layer (scoped to target channel) + `Levels` filter + blend mode `Pass Through` + masked by a reused smart mask
- **Manual cleanup (if needed):** Painter install directory > `assets/smart masks`

### Difficulty
Intermediate — the individual moves (Fill layers, black masks, Smart Mask save/reuse, Levels+Pass Through) are all basic Painter mechanics, but the video's real value is the workflow discipline of building a reusable library upfront and understanding that dragged-in smart mask copies are independent (not live-linked) — a subtlety that changes how you'd plan reuse versus expecting synced updates.

### App & Version
Not stated numerically on screen. Scattering is added as a channel via Texture Set Settings' shader-supported-channel picker, consistent with this skill's other modern-era ingested tutorials; no other version-specific UI markers were visible in the captured frames.

### Tags
layers, fill-layer, paint-layer, masks, smart-mask, blend-mode, basecolor, roughness, height, alpha, texture-set, pbr, intermediate

---

## Related Tutorials
- [SUBSTANCE PAINTER: Building Masks Explained](substance-painter-building-masks-explained.md) — different creator (Jared Chavez); covers the general Smart Mask creation mechanic that this video applies specifically to a reusable character-region library workflow.
- [Texturing a Clicker - FULL Substance 3D Painter Workflow](texturing-a-clicker---full-substance-3d-painter-workflow.md) — same creator (FlippedNormals); shares the same channel-separated-groups organizational philosophy (Color group / Roughness group per texture set) that this video's per-channel smart-mask reuse pattern builds directly on top of.
- [10 New Features in Substance Painter You Didn't Know About](10-new-features-in-substance-painter-you-didnt-know-about.md) — same creator (FlippedNormals); the "Apply to all channels" blend-mode/opacity propagation feature covered there is a complementary efficiency trick to this video's per-channel smart-mask reuse workflow.
