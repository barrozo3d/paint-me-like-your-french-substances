---
title: Paint On Baked Maps To Fix Issues | Substance Painter
source: YouTube
url: https://www.youtube.com/watch?v=oRkgEuGKPtw
author: Stu Lloyd (CG Stu)
ingested: 2026-08-12
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/paint-on-baked-maps-to-fix-issues-substance-painter/
frame_count: 0
frame_status: pending-selection
---

# Paint On Baked Maps To Fix Issues | Substance Painter

**Source:** [YouTube](https://www.youtube.com/watch?v=oRkgEuGKPtw)
**Author:** Stu Lloyd (CG Stu)
**Duration:** 12m52s | 4 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py paint-on-baked-maps-to-fix-issues-substance-painter <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hi.
[0:02] You got your nice bake, but then you might have this, or this, or this.
[0:09] So I'll show you how to change this into this. Woohoo!
[0:14] Alright, so we've got our mesh with our baked maps, but we've got some dodgy artifacts going
[0:29] on here. So we can actually manually fix this up.
[0:33] But first, I'd just like to separate every different section into its own layer, create
[0:39] a new folder, just call that eyes, and then chuck a new fill layer in there, and just
[0:46] change that color so it stands out. And then on the folder, just right click, go black
[0:51] mask, and then add a paint layer on top of that. Then we'll go to polyfill mode, change
[0:59] it to UV shell, make sure it's 100% white, and then just click on the eye.
[1:03] So I'll just go through and do that for each section.


### Fixing Ambient Inclusion [1:06]
**Transcript (timestamped):**
[1:06] Alright, so now we've got the head and the eyes masked out into their own folders.
[1:10] So first we'll work on the Ambient Occlusion channel, but by default the Ambient Occlusion
[1:15] channel is not exposed to us. So if we go to texture set settings, scroll down here, click
[1:21] on the little plus symbol, and then click on Ambient Occlusion. Now it's going to add
[1:25] it to our channels. So what I like to do first is just add sort of a global fill layer, just
[1:32] drag that all the way to the bottom, and I'll just call this base. Because we want to edit
[1:37] the Ambient Occlusion map, everything we add as a layer is going to multiply to the
[1:42] global Ambient Occlusion channel. So we can go over texture set settings, and if we scroll
[1:47] down to Ambient Occlusion mixing, if we change that to replace, then what's going to happen
[1:52] is it's going to basically, everything we add is going to replace our Ambient Occlusion
[1:56] map. So if we just go to our base layer, and scroll down to where Ambient Occlusion is,
[2:02] if we just add our Ambient Occlusion map to this base, then now basically this is just
[2:08] replacing our Ambient Occlusion map. So if I go and choose our Ambient Occlusion channel,


### Fixing Highlight Issues [2:13]
**Transcript (timestamped):**
[2:14] now you can see all the issues we have with our Ambient Occlusion map. So let's say we
[2:18] might want to just work on this eyelid section first just to get rid of this dodgy detail.
[2:23] So we'll go to the head because that's what we've got masked out here. And in this layer,
[2:28] if we add a new paint layer in here, and let's just call this something like AO Fix. Now
[2:35] all we want to do is adjust the AO. So I'll scroll down and I'm just going to only enable
[2:41] Ambient Occlusion and nothing else. And you can see here that by default it's set to
[2:48] full white, which means if I go to my paintbrush and start painting on it, nothing's going to
[2:55] show up because it's set to multiply mode. If I change this to a darker color, you can
[3:01] see now it's going to start showing up because that's how multiply works. If I go to the
[3:07] Ambient Occlusion settings, you can see here it's always set to multiply by default. So
[3:13] if we want to actually show the highlights, we have to change this mode to normal mode.
[3:17] If you change it on just a layer, the highlights are still not going to show up because this
[3:24] is in a global folder and the global folder is set to multiply mode as well. So we just
[3:28] change that to normal. Now you can see that we can start to paint those highlight details.
[3:33] They'll replace our global Ambient Occlusion map. One way you could fix this is by just
[3:40] selecting P for the color picker, selecting a color nearby, and then maybe going in and
[3:46] manually painting this area away. And that's great, but if you start to go over here, obviously
[3:51] you start to just, you're going to have to use the color picker a lot. So one way you
[3:55] might want to do it is by using the Clone Stamp Tool. So if we go to Clone Stamp Tool
[4:01] now and just make this a little bit smaller, if I press V to select an area and then start
[4:08] trying to paint, it's actually not going to work because it's not sampling this area
[4:15] this actual map. It's only using this paint layer, which is basically transparent. So
[4:21] if we want to paint directly on this Ambient Occlusion map, what we have to do is we first
[4:25] have to fill this paint layer with the Ambient Occlusion map. So if we go right click on
[4:30] the Ambient Occlusion Fixed Layer, add a Fill mode, and then on this Fill, so click on the
[4:37] Fill, we're going to basically only enable Ambient Occlusion. And then on our map here,
[4:42] we're going to replace Ambient Occlusion with a Fill map. And then what we can do on top
[4:47] of this is we can just right click and go Add Paint. And now this is going to work similar
[4:52] to how it was before. But now we want to affect the Ambient Occlusion map that we've filled
[4:58] it with. So if we change it from Multiply to Pass Through mode, now what's going to happen
[5:04] is we can actually paint on this layer and we can affect the fill. So we can use our
[5:10] Clone Stamp brush now. So if I go to say, let's just sample the color here, and now I start
[5:15] using the Clone Stamp tool, you can see that we're actually affecting it, we're affecting
[5:22] the paint layer like we're affecting the actual baked map. So it just makes it a little bit
[5:28] easier to go in here and paint those details. And we can also use cool things like we can
[5:33] go in and we can use the Blur brush, and we can just go in here and start blurring everything
[5:38] we wanted to. So let's just keep Clone Stamping this away. And you can see now we've just fixed
[5:51] up this area and the eyelid. And it's non-destructive, so you can just turn this layer on and off.
[5:56] So now we can essentially just do the same thing with the eye layer. So if I scroll down
[6:01] to the eye layer, let's add a new paint layer to the eyes folder. And on this we're going
[6:08] to call it AO Fix. And again, I'm only going to enable the Ambient Occlusion channel. I'm
[6:14] going to right click and go Add Fill, and then only enable Ambient Occlusion, select
[6:20] our Ambient Occlusion map. And then we're going to set the overall Ambient Occlusion blending
[6:27] mode of that layer to Normal mode so that it doesn't multiply to the global one. And
[6:34] so then I'm going to add a paint layer on top of that. And we're going to set the paint
[6:40] mode to pass through. And now we should be able to do all the changes on the eye here.
[6:46] So we could go in and we could start painting this color in, or we could maybe experiment
[6:54] with using the Smudge brush, so we could start to smudge this up if we wanted to. But in some
[7:00] cases you might want to just eliminate the Ambient Occlusion around this eye because you
[7:06] might want to animate your eyes moving around, which means you don't want to bake that Ambient
[7:09] Occlusion in. So what I'm going to do is I'm going to actually just choose a paint brush,
[7:14] and you can just press P to select, say, you know, some sort of bright color. And now we
[7:20] can start to paint the Ambient Occlusion map away. And once you've done that, you might
[7:27] want to just switch over to your blur brush, and just blur the areas in a little bit just
[7:32] to make it not so harsh. So if I go back to Material mode now, you can see that our Ambient


### Fixing Normal Issues [7:36]
**Transcript (timestamped):**
[7:39] Occlusion map is going to work a lot better. Alright, so now we can fix the Normal map.
[7:44] So to do that we actually have to do, similar to what we did with the Ambient Occlusion,
[7:48] we have to replace our global Normal map so we can paint over it. So we'll go to Texture
[7:52] Set Settings, and by default the Normal map is exposed, but its mixing mode is set to
[7:58] Combine. So let's just change that to Replace, and then you can see it's all gone because
[8:04] we don't actually have it applied yet. So if we go back to our Layers, scroll all the
[8:09] way down to our Base Layer, and because we've got Normal activated here, we can scroll down
[8:14] and we can add our Normal map in here. So I'll just filter this by Project, go to Textures,
[8:20] and then drag our Normal map in, and now it's going to show up again. So let's go to the
[8:27] Eyes Layer, and we'll add a new paint layer, and just chuck that into the Eyes folder, and
[8:33] call this Normal Fix. And then similar to what we did with the Ambient Occlusion, we
[8:38] want to fill this with our Normal map. But first we just want to make sure that we're
[8:43] only affecting the Normal. So on this Normal Fix, I'm going to scroll down and only select
[8:47] Normal here. And then let's add a Fill, and we're going to fill this, make sure that
[8:55] it only has Normal mode enabled, and again we're going to drag our Normal map into our
[9:02] Normal channel. It's actually doubling the effect of our Normal map. And that's because
[9:08] if we go to our Normal map settings here, the Layer mode is set to Normal map detail
[9:15] by default. So we want to actually set this to Normal, so that it will replace our base
[9:21] Normal map with just a Normal, with our Normal map that's set to Normal mode. So if we change
[9:28] our Eyes folder, because this is the top layer, change that from Normal detail to Normal, and
[9:34] now we'll get our Normal map showing exactly how it should. So on our Normal Fix layer,
[9:40] I can now add a Paint mode, and I can set this to Pass Through. Let's go back to our
[9:49] just a Normal Paint brush. And if we scroll down, we can see that if I just enable only
[9:57] Normal on this Paint brush, we can see that the Normal color is set to our base Normal
[10:03] color, which is basically flat. So if I grab this now and start painting, you can see it's
[10:07] painting away all those dodgy artifacts. So I can show you if I go to the actual Normal
[10:13] mode, you see this is what our Normal looks like. And now you can see I'm actually painting
[10:18] away that dodgy detail. And because we don't want any, we just want to keep this completely
[10:27] smooth, we can basically paint away all these edges around the eye there. Go back to Material
[10:32] mode, and then you can see that eye is essentially fixed. So now we can just start the same thing
[10:37] with the eyelid. So we'll scroll up to the head. Let's add a new Paint layer. We'll call this
[10:41] Normal Fix. I'm going to drag it into the head layer. So I'm going to add a Fill, and then
[10:48] I'm going to make sure it's only got Normal mode enabled. Drag our Normal map onto that
[10:54] Normal mode, so now it puts it back. But again, it's doubling up the Normal channel, because
[10:59] we have to change our head folder to Normal mode. So now we've got our proper Normal showing
[11:04] up. So now I can add a paint on top of this. Set the paint to Pass Through mode. Make sure
[11:10] our brush settings is on Normal, and our Normal is selected. Now you should see here I can
[11:16] start painting away those details. The only problem is you can see that it's not as simple
[11:23] as just replacing it with a flat Normal color, because we actually have Normal detail of
[11:28] this curve here that we want to keep. So all we actually have to do is if we go to the
[11:34] actual Normal mode here, instead of just simply painting out a flat color, so you get this
[11:44] edge here, you might have to do a Mixger, so you might have to go in and use the color
[11:49] picker to select this color and paint that in, and just keep doing this. So you could
[11:56] just keep reselecting that color and drag that in. That's fine. Let's go back to our
[12:02] Clone Stamp brush over here, and I can just basically select a color out here somewhere,
[12:09] and then I can start painting this back in. Alright, so our Clone Stamp brush isn't working,
[12:14] and that's because our Clone Stamp is only set to AO, so we just want to set that to Normal.
[12:19] Now we should be able to sample that Normal detail with our Clone Stamp brush.
[12:29] Alright, so once you've got your, you've painted in your Normal fixes, go back to Matera mode,
[12:34] and you can see now your eye details are all being fixed up. This is the Dodgy Eye, and that's the Good Eye.
[12:44] Alright, well, hope that helped. Cheers, thanks, bye!



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
