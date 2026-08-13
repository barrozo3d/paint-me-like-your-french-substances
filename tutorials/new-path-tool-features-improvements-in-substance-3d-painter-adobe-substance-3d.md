---
title: New Path Tool Features & Improvements in Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=exE0-1ftNeE
author: Adobe Substance 3D
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/new-path-tool-features-improvements-in-substance-3d-painter-adobe-substance-3d/
frame_count: 0
frame_status: pending-selection
---

# New Path Tool Features & Improvements in Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=exE0-1ftNeE)
**Author:** Adobe Substance 3D
**Duration:** 6m16s | 7 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py new-path-tool-features-improvements-in-substance-3d-painter-adobe-substance-3d <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Introduction [0:00]
**Transcript (timestamped):**
[0:00] Hi, in this video we'll be looking at some new features for paths in Substance Painter 11.


### Working with Filled Paths [0:06]
**Transcript (timestamped):**
[0:06] Let's take a look at this wing of a dragon at the back and we'll be using the filled
[0:10] path to create some shapes similar to this.
[0:13] So to use that, first of all, you have to create a new empty layer and then you select
[0:17] the path tool.
[0:19] By default, you'll have the paint along path selected, but if you click the tool again,
[0:23] you'll see a list of two options and you can choose the filled path over there.
[0:28] Filled path works similar to the regular paint along path.
[0:30] So you click to create a shape and it automatically adds tangents and you'll see once I click
[0:36] on the last one to close it, you get a filled shape that shows up on your mesh.
[0:41] This is just a quick test, but one thing I want to point out is that these green stripes
[0:46] that you're seeing here, they're actually options for the normals and they show how
[0:49] deep this shape is projected.
[0:52] So if I change that, which is also new, you look at the path options at the top here,
[0:56] you see the type, the depth.
[0:58] If I change the depth, you should see the length of the normals change.
[1:02] You can even type in values here because if I look closely on the other side, they're
[1:05] projected through.
[1:06] So if I were to type in a tiny value of say 0.05, I still get some projection to the other
[1:14] side and I can reduce this a little bit.
[1:16] So for example, 0.03 or I might want to go even smaller, 0.01.
[1:22] And you can see in this case, it's a little bit too small.
[1:24] So you want to find an in-between obviously that works for your case.
[1:29] Now let me get rid of that one, remove it.
[1:32] And when you're drawing paths, something that's new as well is if you click and shift click,


### Changing Path Types [1:33]
**Transcript (timestamped):**
[1:39] you create straight lines.
[1:40] So this is similar when using the regular brush tool and I'm going to create a little
[1:45] jagged shape similar to the existing ones that are already on there.
[1:51] And then close by shape like that.
[1:53] So I've got a single one now and keep in mind that these filled paths, they only fill with
[1:57] solid values.
[1:59] So you cannot actually paint materials with them.
[2:01] You can paint materials if you use them as a mask.
[2:03] So you could just create a new mask and in a paint layer, use them there.
[2:08] In this case, they're just filling with solid colors.
[2:10] So I'm going to really quickly go for a color similar ish tool we already have like that.
[2:18] And say I would want to add a stroke around this.
[2:20] Now, how would I create two different variations of that?
[2:22] Well, you can select the path, control D to duplicate it.
[2:26] And I have two separate ones now.
[2:28] They're both exactly the same, but I can convert the type.
[2:31] You do it two ways.
[2:32] You can right click it and change the type to be paint along path.
[2:36] Then you see it gets painted and it's very thick now right now because the size is too big.
[2:40] So reduce the size a lot like that.
[2:44] And again, just as before, I can change these settings
[2:49] so that it looks like another fill running around it.
[2:53] Another way to do this and you could actually use this to go between multiple layers.
[2:57] Say that I don't want these two to be on the same layer.
[3:00] So I'm actually going to remove this path.
[3:04] I'm going to copy it.
[3:08] Then I'll create a new layer.
[3:10] I'll start a quick new path here.
[3:13] Not do much to it and then say paste.
[3:15] And then say paste.
[3:17] But instead of paste, I'll say paste all vertices.
[3:19] And this actually pastes the vertices, the actual shapes from the last path into the new one.
[3:24] So that's another way to sync paths.
[3:27] And then again, you can obviously change the type to be paint along path
[3:31] and then do the same thing here.
[3:35] So this would have to be tweaked a little bit.
[3:36] Tricks you can do on this, of course, are adding a filter.
[3:39] For example, I would add a filter here.
[3:42] And I could choose a warp.
[3:45] And let's wait for that to calculate.
[3:48] So that tweaked.
[3:48] Another thing that you can do is right up here, if this path gets in the way,
[3:52] you can show or hide the viewport interface.
[3:54] In some cases, they might actually get in your way.
[3:56] So you just toggle it on and off to see what's going on.
[3:59] This is not a new feature, but people might have missed it so far.
[4:03] Another thing that you can do while you're drawing paths, that's also new.


### Snap paths to mesh [4:04]
**Transcript (timestamped):**
[4:06] So if we start a new one is you can turn on snapping.
[4:08] So snapping snaps to the mesh wireframe and you see that the mesh wireframe
[4:12] turns on and there's actually settings for it.
[4:14] I can say snap to mesh wireframe to vertices, the edges or to edge centers.
[4:20] With snapping activated, when you draw a path, it will snap to the closest
[4:25] vertex position.
[4:26] You can change this as mentioned before up here.
[4:30] The hot key for snapping is shift Z and you hold Z for temporary snapping.
[4:35] Another thing you can do is you can use angle snapping now.


### Snape to angles [4:37]
**Transcript (timestamped):**
[4:37] So if you're called control shift and you should see
[4:42] that your path lines are snapping to increments of 45 degrees.
[4:47] This can be modified as well.
[4:49] You open up the settings you'll see here.
[4:50] There's an angle step setting.
[4:52] You can set it to every one, five, 15, 30, 45 and 90 degrees.
[4:56] You also set the reference.
[4:58] So in screen space means it's always aligned to the camera.
[5:00] A vertex space means it's aligned with your mesh and world space means it's aligned with your mesh.
[5:03] World space means it's aligned with your mesh and world space means it's aligned with the world.
[5:07] Use whatever you feel fits.
[5:09] So once again, it's control shift to do specific angle snaps.
[5:15] And you can do very precise shapes with that.
[5:18] Lastly, paths can also be transformed.


### Transforming your path [5:19]
**Transcript (timestamped):**
[5:21] So when you turn on the transform manipulator, you can actually move paths in a different way.
[5:27] Normally the way to move points is to drag on them.
[5:30] But if you turn on the transform manipulator, you can actually move them with a 3D gizmo.
[5:36] You can stack multiple points as well.
[5:38] You shift to click them.
[5:43] It lets you move multiple points at the same time.
[5:46] Keep in mind that this is not always the easiest to use, since it will align to the world when you're doing this.
[5:55] But it lets you move an entire path over fairly quickly without having to drag each point individually.


### Conclusion [6:02]
**Transcript (timestamped):**
[6:03] That's a quick overview of most of the new features that are in the new path tools for Substance Painter 11.
[6:09] I hope you have fun with them.



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
