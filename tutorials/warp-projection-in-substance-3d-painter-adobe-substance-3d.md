---
title: Warp Projection in Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=6_8CCf6v-uM
author: Adobe Substance 3D
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/warp-projection-in-substance-3d-painter-adobe-substance-3d/
frame_count: 0
frame_status: pending-selection
---

# Warp Projection in Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=6_8CCf6v-uM)
**Author:** Adobe Substance 3D
**Duration:** 10m57s | 3 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py warp-projection-in-substance-3d-painter-adobe-substance-3d <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hi, in this video I'm going to take you through how to use the new warp projection mode that
[0:13] was added in Painter 7.3.1. To do that first I want to distort a simple shape, this arrow
[0:19] here on a fill layers mask. So I'm going to create a new fill layer, I'll set this fill
[0:25] layer to red so that it's very obvious. Then I'm going to add a black mask to it and then
[0:31] in this black mask I'm going to add a fill. Why a fill? Because the warp projection mode
[0:37] only works with fill. I'll then take this alpha, drop it into that slot and we can see
[0:43] it's visible right now on my tiling plane. So ignore the rest, I'm just going to focus
[0:47] on this middle part to show you the warp basics. I scroll up, I can set the projection mode
[0:52] from UV projection to warp projection. Now if you zoom out a bit you see that the warp
[0:59] projection mode is slightly strangely aligned right now. So there's an easy way to fix that.
[1:07] If you want to get it to appear correctly you press the surface tool and the hotkey


### Warp Basics [1:11]
**Transcript (timestamped):**
[1:12] for that is shift W and just move it over the surface to get your warp to appear like
[1:18] that. Now it's still kind of big so I'm going to press R for scale and I'm going to look
[1:24] at it from the top and scale my arrow down a bit like that. If you don't want this to
[1:31] repeat you can also turn off the UV wrap to none but in this case it doesn't make any
[1:36] difference because I'm using a tiling plane anyway. So what I'd like to do specifically
[1:40] to show you the warp basics is I want to bend this arrow slightly. You know a bend modifier
[1:45] that you would do in another 3D program or a 2D program. So once you set it to warp projection
[1:51] there's a few things you can do. The main one would be that if you click on the settings
[1:56] for the warp so that's up here you can set the grid so I can set the number of rows for example
[2:02] I can unlock this as well and I would actually like to have say four columns like that. Maybe
[2:09] let's go for three that's a little easier and I can change the handle size as well so I can
[2:14] make those large. You can change the grid color so it's a little bit difficult to see so let me
[2:19] just set that to purple. That should make it just a little bit more visible. If you actually
[2:25] want to start modifying this warp grid here in a simple case you set the subdivision settings
[2:30] here and then you go into this drop down menu next to it that lets you choose how to affect the warp.
[2:35] Right now I'm transforming the warp so that means I get to move it around but it gets really
[2:41] interesting once you go to edit vertices. This lets you actually select the vertices and modify
[2:46] them so I can draw a selection frame like this and then use the regular move tools just like you
[2:53] would work in 2D or 3D to select parts out. So I'm switching between the different tools with
[3:01] we and are. I'm just going to select a few of these rotate this out and move them like so again
[3:09] using e moving these around and just trying to get this aligned in a simple way. You can even
[3:15] move them individually by just dragging like that. Right so it gives me a little bit more control
[3:20] over it like so. Alright let's push those out a bit more there. So that's a quicker way if you
[3:25] want to move individual points. Move these a bit closer as well. So that's a very simple way to use
[3:32] warp on a 2D shape. You can always switch back to regular moving of the warp as well by going
[3:38] into the transform warp up here and then you can simply move the warped shape around like you did
[3:44] before. Now that's a simple case. Let's move on to a more complex one to go a little bit more in
[3:50] depth. So I've got a new example open here. This is the man that we used for the promotion of the


### Warp Example [3:51]
**Transcript (timestamped):**
[3:57] warp feature and it's a good example of when the warp really makes sense. So I have a scanned face
[4:04] from a website called texturing xyz. So this was scanned from a real person comes with height
[4:09] maps and roughness maps. I have this sculpted face that was made by my coworker geo. Problem is that
[4:15] the proportions of the scanned face don't match the 3D sculpted face and I'd still like to transfer
[4:21] them and for that warp is a perfect case to move things around. So let's set that up first. I'm
[4:26] going to create a fill layer. I'm going to use my textures in the base color and we'll take this
[4:33] and put that into the roughness. We will also put this part into the height. Now the height's a bit
[4:40] too strong. So I'm going to add a levels to the height and I'm just going to really limit the output
[4:47] of that. So the height isn't too strong. Next let's change our projection setting. So we're using
[4:51] warp on a full material here. So I'm going to change the projection to warp projection and set the UV
[4:57] wrap to none. If I zoom out a bit the warps kind of it's gold. See it's floating in 3D space here. I
[5:04] want to get this into a good position first. So I'm going to aim it somewhere towards the center of
[5:10] the face. Right. So just in general I like to get what I think is about the center of the face like
[5:16] that. Now the scale is all off. So what you want to do first is you want to scale this down so that
[5:23] you get the approximate proportions like that. So scale it down a bit more something like that. And
[5:29] I want to do the same in that direction. You said if I'm looking closely you can start to see the
[5:35] issue now. The eyebrows are too low. The eyes aren't in the right position. The nose is too low. The
[5:40] mouth is a bit too low. So let's try and move it up a bit more. There we go. We still want to move
[5:46] this around quite a bit and wrap it around the face as well. So I'm happy with these proportions.
[5:53] Then the next thing I'm going to do is like before go to edit vertices. Take these guys and I'm going
[5:58] to wrap them around all the way to the side. Probably try and get the ear aligned. Do the same
[6:04] for the other side. Take these and wrap them around until we get to a position where that kind of
[6:10] makes sense. And you see that there's a projection depth as well. There's a setting you can use to
[6:14] control this right. It controls the length of the projection. I'll probably set this a bit deeper.
[6:18] It doesn't hurt to go a bit further. Okay. So we've got our basic setup and one very important
[6:25] thing to keep in mind is we want to try and pull this off with as little points as possible. The
[6:30] more points you get, the harder it becomes to manage them. It's really interesting here as well
[6:35] is that if I grab one of these and use the quick move on them, it snaps to the surface immediately.
[6:42] See? So this is instantly snapping to the surface. So I'm going to do that for each of the main
[6:47] points already. And see how they've sort of wrapped and got closer together again. I'm going to have
[6:54] to fix that at a later point. So I'll do the same thing here. Move that about over there. Move this
[7:00] a bit lower. So try and get in a good view and we'll place each of these on our guy. Alright.
[7:07] We can do the same thing for this nose here. Bring it up a bit. And you can see sometimes it gets a
[7:13] bit funky, right? So like this one's jumped away. So I can try and rotate that one a bit to bring
[7:20] it back. But yeah, it's just acting a bit strange. So I'm going to have to cut some extra loops in
[7:27] here to fix this up. So if you click here, you can use this to split the warp horizontal and
[7:33] vertically. So the first thing I want to do is I want to add some vertical splits. So I'm going
[7:37] to split the warp vertically, add one there. And you have to select it again each time you want to
[7:43] do it. So split warp vertically, add one there. Then I'm going to go back into edit vertices and
[7:48] bring these to the surface and get them into like a good position, right? So you can use these to
[7:53] stretch it out. Pull this around and try and get like semi decent proportions. So pulling that in
[8:04] there. And this one, we want to move on the face as well. Right. So we definitely want to add another
[8:15] horizontal cut over here to get it closer to the face. So we're going to do the same thing, split
[8:20] warp horizontally. And I try and estimate by like using the surface normal to see that it goes
[8:27] about in the middle of the mouth. Like so. Then I'm just going to snap this back. If the rotation
[8:36] is strange, remember, you can always simply use the rotate tool to rotate this out. You don't
[8:41] have to use the surface snapping. The regular move is fine for this as well. So we'll get that into
[8:46] that position. Okay, so we're getting closer. Things are getting aligned, but we'll have to add a
[8:52] few more. So we definitely want to add a cut around the eyes to do those. So again, split warp
[9:00] vertically and try to estimate where they're actually going to end up.
[9:11] So after quite a bit of tweaking, this isn't exactly a fast process. This is what I ended up
[9:17] with. So I've tried to make sure to align the nose properly, the eyes are aligned, the eyebrows are
[9:22] aligned, the mouth is aligned. Okay, as well. And I had to add an extra cut around these two to get
[9:30] more control. It's still not completely there. So one tip I can give you is don't start adding more
[9:36] points to a specific section like the mouth, just to get that one thing to align properly. What you
[9:41] would do is create another layer where we simply cropped out the mouth. So you can see this here,
[9:46] the mouth, and the mouth is then a separate war projection that goes on top. And the mouth simply
[9:52] has a mask. See, we've painted out a mask where the mouth appears, and it blends over the top, and
[9:58] allows me to move it in a better position. So key areas like the mouth, the eyes, or even the nose,
[10:05] you could do those with a separate projection where you take the same texture. And this was
[10:09] cropped out in Adobe Photoshop, just align it and do it separately. No point in making your grid
[10:14] for the entire face so dense, that you can't move it anymore. So just use a separate one to get
[10:19] things aligned like that. Also, one tip is if you go into the warp settings, it can get a bit busy
[10:26] with these normals. So you can turn these off right now as well. This makes it a little bit
[10:30] easier to work with, especially if you turn on the vertices, just a little bit easier to see what's
[10:36] going on as well. So there's that setting, show normals. That's it for this video. I hope this
[10:41] helps you get started. Keep in mind war projection needs a fill. Don't use too many points and make
[10:47] use of the shortcuts like WENR and a drag to move across the surface. Good luck with it.



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
