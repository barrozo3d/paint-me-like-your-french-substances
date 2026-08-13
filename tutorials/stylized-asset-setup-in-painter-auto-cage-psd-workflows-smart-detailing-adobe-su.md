---
title: Stylized Asset Setup in Painter: Auto-Cage, PSD Workflows & Smart Detailing | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=LRy-Nc7B_bk
author: Adobe Substance 3D
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/stylized-asset-setup-in-painter-auto-cage-psd-workflows-smart-detailing-adobe-su/
frame_count: 0
frame_status: pending-selection
---

# Stylized Asset Setup in Painter: Auto-Cage, PSD Workflows & Smart Detailing | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=LRy-Nc7B_bk)
**Author:** Adobe Substance 3D
**Duration:** 6m25s | 5 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py stylized-asset-setup-in-painter-auto-cage-psd-workflows-smart-detailing-adobe-su <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hey, my name is Pablo, I'm a 3D concept and character artist with a passion for education.
[0:04] In this video, I'm gonna show you how I set up a project in Adobe Substance 3D Painter with a flexible, non-destructive workflow.
[0:10] The focus of this video is not on the texturing or painting side of things just yet,
[0:14] but rather on setting up a clean foundation so that we can work a little bit faster with smart tools like the AutoCache and the AutoUpdater.
[0:21] And I'm also gonna give you some tips about the path tool to create high details or high information in your models with just textured information.
[0:27] Alright, so here we are in Adobe Substance 3D Painter.
[0:30] Now, before we jump into any details, let me give you a quick look at the final scene that we are trying to build.
[0:35] It is a simple, still life scene with lemons, sardines and some ceramic pieces.
[0:40] And the idea is to go for a stylized, painterly feel.


### AutoCage [0:43]
**Transcript (timestamped):**
[0:43] The first thing I wanna do is bake some mesh maps.
[0:46] And this step is a key part of the process because it sets the foundations for pretty much everything that comes next,
[0:53] like smart mask, high details or any edge accents like wear and tear.
[0:57] Now, the model itself has some tricky spots.
[1:00] There are some overlapping areas and pieces that sit really close together.
[1:04] And this can make the baking process a little bit of a nightmare if you're doing everything manually.
[1:09] But there is a new feature that takes all the guesswork out of this step.
[1:13] So let's click on the Bake Mesh Maps button.
[1:15] In the baking window, I'm leaving most of the settings on default
[1:19] and I just need to reference my high resolution version of this mesh.
[1:22] Once that is loaded, you'll see this ghost-like yellowish outline appear around the model.
[1:27] And that is basically the cage.
[1:29] This is like a buffer zone used during the baking process
[1:32] to project details from the high poly to the low poly.
[1:35] You can use this slider to adjust how tight or how loose that cage is.
[1:39] And the problem is that if it is too tight, you'll see some of these red zones.
[1:43] And these areas won't get baked properly, which results in some sort of gaps or weird artifacts on the surface.
[1:49] And this is where the Auto Cage method becomes super useful.
[1:52] It is an adaptive mode that wraps the cage around your mesh automatically.
[1:56] It conforms to the volumes of the object, even in the tight corners like this.
[2:00] And it gives you a clean bake with just one click.
[2:03] Let's go ahead and switch to that mode, hit Bake, and we're done.


### Smart Detailing [2:06]
**Transcript (timestamped):**
[2:06] After the baking process is done, we have a nice and clean result without any manual tweaking.
[2:12] Now, for the second part of this initial setup,
[2:14] I want to show you how to use external textures in a smart way.
[2:18] I got a PSD file with a photo of a sardine already matching the UV layout for this mesh.
[2:23] Nothing too fancy here, but I got a really cool workflow tip that will make this way more powerful.
[2:28] So let's start by dragging the PSD file into the Asset Library,
[2:32] make sure this is set as a Texture, and from the Import dropdown, let's select the Import As project.
[2:38] That way, the texture becomes part of this project when we save it.
[2:41] Alright, so now that this is part of our library, let's go ahead and create a new fill layer in the Layer Stack,
[2:46] and I'm going to drag and drop the texture into the Base Color slot.
[2:49] That's it, the map perfectly fits into this mesh.
[2:52] Now, here's what it gets interesting.
[2:53] Say I want to adjust the saturation or tweak some of the contrast in this texture,
[2:58] normally I would go back to Photoshop, export a new version, replace the file in Painter,
[3:02] load it up again, connect things, and that could be very tedious.
[3:06] But without the Auto Update feature, I don't need to do any of that.
[3:09] I just go ahead and open the PSD file in Photoshop, make any edits that I want,
[3:13] save the file, and Painter can refresh it for me.
[3:15] So let's go ahead and set that up.
[3:17] Back in Painter, go to the Asset Library, and look for the small refresh icon at the bottom.
[3:22] You can click on that, and then you can check both of these boxes.
[3:25] One is to update the resources in the library itself,
[3:28] and the other one is to update that resource in all the instances of the project.
[3:32] So basically, whatever we used that texture before.
[3:34] So the texture will reload instantly everywhere that is being used.
[3:38] That is a serious time saver and definitely a smoother way to work.


### Extra Surface Details [3:41]
**Transcript (timestamped):**
[3:41] Now, before we wrap up, I want to show you one last thing.
[3:44] A simple but effective way to sculpt with texture.
[3:47] This is basically a way to add some extra surface details without modifying the model itself.
[3:52] So it would rely 100% on a texture map.
[3:55] So let's take this ceramic jug as an example, and it looks okay, but it's a little bit plain.
[4:00] We can add some stylized ridges or ornaments around the rim and that sort of stuff.
[4:05] So I'm going to start by creating a new field layer,
[4:08] and I'm going to disable every single channel except the hide information.
[4:12] Now we can go ahead and add a black mask followed by a paint effect.
[4:15] Now I can select the path tool, and here's the trick.
[4:18] I'm just going to start clicking around the rim to draw a clean curve.
[4:22] And right now, this doesn't look like much.
[4:24] There's actually nothing happening.
[4:25] But the cool thing is that this path is fully editable.
[4:28] So just so that you can see what we're actually doing,
[4:31] I'm going to increase the value of the hide information.
[4:34] There we go.
[4:35] And now we can go ahead and move the points, shape the curve,
[4:37] and adjust the entire design without needing to redo anything.
[4:41] It's non-destructive.
[4:42] Now changing the placement of the curve points is not the only thing.
[4:45] We can open the stroke settings and increase the size and spacing
[4:49] of the instance that is used by the brush.
[4:51] Now we're starting to see kind of like the detail pop a little bit more.
[4:54] Now for the final touch, let's go ahead and add a smooth bevel effect.
[4:57] This filter allows you to soften and round the stroke.
[5:00] Instead of having a flat line with a bit of height,
[5:03] we end up with a nice smooth ridge around the rim.
[5:06] Of course, you can fine tune the curvature distance, the smoothness slider,
[5:10] and basically anything in this filter to get exactly the look that you want.
[5:15] And because this is non-destructive and procedural,
[5:17] I can change the look of this at any time.
[5:19] For example, I can go to the library and filter for my alphas,
[5:23] and I can just go ahead and drag and drop a brand new alpha into the stroke settings.
[5:27] This changes the alpha that is being applied to the stroke around the path,
[5:30] but we can go ahead and tweak the spacing, we can tweak the size,
[5:34] and essentially create a completely different ornament
[5:37] without losing the non-destructive flexibility.
[5:39] And that's a wrap for this setup.
[5:41] No painting yet, I know, but this video is all about preparing our scene for clean bags,
[5:46] smart texture workflow, and flexible detailing tools.
[5:49] In another video, I'm gonna take this setup and I'm gonna show you how to texture this project
[5:53] to achieve that sort of stylized painterly look with some really cool finishes.
[5:57] Also, I'm gonna keep an eye on the comments of this video,
[5:59] so feel free to drop any questions or suggestions on things that you'd be interesting to know more about.


### Outro [6:05]
**Transcript (timestamped):**
[6:05] So that's a wrap for this video.
[6:06] No painting just yet, but as I said at the beginning,
[6:08] it's all about setting the foundations so that we can work a little bit faster.
[6:11] So now we have some clean bags and everything in the project is ready to start the texturing process.
[6:16] In the following video, I'm gonna take this exact same project with all the setup that we've done,
[6:19] and I'm gonna show you how I textured my scene to create this stylized painterly look.
[6:23] See you there.



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
