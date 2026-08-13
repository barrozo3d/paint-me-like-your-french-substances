---
title: Baking in Substance 3D painter 8.3 | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=hYtHp4IXvsM
author: Adobe Substance 3D
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/baking-in-substance-3d-painter-83-adobe-substance-3d/
frame_count: 0
frame_status: pending-selection
---

# Baking in Substance 3D painter 8.3 | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=hYtHp4IXvsM)
**Author:** Adobe Substance 3D
**Duration:** 15m26s | 9 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py baking-in-substance-3d-painter-83-adobe-substance-3d <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Introduction [0:00]
**Transcript (timestamped):**
[0:00] Hello everyone and thanks for joining me in this work through of Painter New Baking Features.
[0:13] Painter 8.3 has a brand new baking mode that gives you more control over the baking process
[0:17] while letting you interact dynamically with your mesh.
[0:20] Now don't be afraid if this all sounds a bit overwhelming or if you're used to
[0:24] paint a former baking system, we're going to take each step at a time.


### How to access baking mode [0:28]
**Transcript (timestamped):**
[0:28] There are several ways to access the new baking window.
[0:31] The first one is by going to the top right of the viewport where a little croissant icon has now appeared.
[0:36] If you don't see it, no worries, it can get hidden by one of these panels.
[0:41] You can also go to the mode menu up here where you can access all the different modes in Painter,
[0:46] baking mode, painting mode, rendering mode, etc.
[0:49] Alternatively, you can use the shortcut F8.
[0:53] You can at any point return to painting mode by clicking here on return to painting mode.
[0:58] Or by clicking on the brush icon here.
[1:01] Alright, so we are now in the brand new baking interface of Painter.
[1:05] If you were used to the previous one or if you're new to Painter,
[1:08] this may be a little daunting, so please bear with me as I go over each panel.
[1:12] Keep in mind that a lot of familiar actions are still available in baking mode.
[1:16] You can display the 2D view just as in painting mode.
[1:20] The environment settings, log and history are still in the right toolbar.
[1:25] And like everywhere else in Painter, you can undock and move around panels to your own liking.


### The interface [1:29]
**Transcript (timestamped):**
[1:30] Now let's go over the interface itself.
[1:32] On the top right, you'll find your texture set list along with your UV tiles.
[1:36] Notice that both the texture sets and the UV tiles are selectable,
[1:40] allowing you to bake only specific parts of your mesh.
[1:44] Right beneath it are the individual bakers with the command settings on top.
[1:48] This looks pretty similar to Painter's former baking system,
[1:52] but some things are new, such as this little links icon next to each baker.
[1:56] We will go over this in a bit.
[1:58] And on the right are the bakers settings, displaying the parameters of whatever baker you have selected.
[2:04] These panels follow a natural hierarchy.
[2:06] You can think of it as a path that gets more and more specific.
[2:10] You start by choosing what texture sets and UV tiles you want to bake,
[2:13] then you specify the type of baking you want to do,
[2:16] and finally you adjust the settings of the bakers.
[2:19] Below it are the baking logs.
[2:21] This is a partly new feature that lets you keep track of not only the baking process,
[2:26] but also the loading of your high poly meshes,
[2:29] as well as any potential mismatch between your high poly and low poly.
[2:33] These logs are very useful, as they will not only display a warning,
[2:37] but also point you towards the source of the problem.


### The interactive viewport and baking overlays [2:40]
**Transcript (timestamped):**
[2:40] Now let's move on to one of the most important features of this update.
[2:44] I'm talking of force about the viewport.
[2:46] As you can see, we have our project mesh here,
[2:48] but it looks somehow different than in painting mode.
[2:52] That's because if you pay attention to the panel attached to the left here,
[2:55] we have several overlays to help us.
[2:59] Namely, the yellow tint and wireframe depicts the cage
[3:02] that represents how the rays will be cast during the baking.
[3:06] To better illustrate this, let's prepare a simple bake.
[3:09] I'm going to load my high poly meshes here in the command settings,
[3:14] and see how the loading is tracked in the log.
[3:17] Perfect.
[3:19] Now you'll notice that something has changed in the viewport.
[3:22] A blue layer has appeared underneath the cage.
[3:25] That's the high poly model.
[3:27] You now have three elements displayed at the same time.
[3:30] The low poly mesh that is a bit buried underneath everything else here,
[3:34] the high poly mesh, and the cage.
[3:37] Now what is great about this feature is that it allows for direct visual feedback
[3:41] as you fiddle with your cage.
[3:43] No more blind tweaking.
[3:45] Here, for example, the cage offset is way too big,
[3:48] so let's reduce the max frontal distance
[3:51] until the cage tightly wraps around the model.
[3:55] If we go too far, matching errors will start to appear in red,
[3:58] helping us find the right balance.
[4:02] We can now inspect our mesh and search for missing areas,
[4:07] and simply adjust the cage accordingly.
[4:09] To make those fine adjustments easier,
[4:11] the sliders are now exponential instead of linear,
[4:15] meaning you can tweak values within a very small range.
[4:19] If you accidentally went too far and want to go back to your previous setting,
[4:22] you can also undo your last action with Ctrl Z.
[4:26] Now let's go over the baking visualization panel in more details.
[4:31] First off, you can always disable all the overlays
[4:34] by clicking here on the hide icon.
[4:36] It's especially useful if you want to see your project mesh only
[4:39] to check the result of a baking pass, for example.
[4:42] You can also choose to see the baking meshes only for the selected texture set.
[4:47] If you combine that with the focus mode of your texture sets,
[4:50] you can isolate the part of your project that you want to focus on.
[4:55] Below that is your hyperlink mesh, if you have any.
[4:58] Like the rest, you can customize it or disable it altogether,
[5:01] which can prove useful if your mesh is very heavy
[5:04] and is eating up too much of your memory.
[5:07] I personally hide it once I'm happy with my cage.
[5:10] Next up is the cage that instantly reflects the value you set up in the command settings.
[5:16] And here again, you can disable it, change its color, its opacity, etc.
[5:21] Then we have an option to display missing seams on hard edges.
[5:25] I don't have any on that mesh, but we'll take another example in a moment.
[5:29] And finally, we have our project mesh, or LP for low poly.
[5:34] This is what remains when you disable the baking visualization.
[5:38] Notice that it comes with a neutral material that you can adjust to better inspect your mesh
[5:42] after the baking.
[5:44] For example, it can be interesting to make it smoother and metallic
[5:47] to search for any artifacts or errors.
[5:51] You can also decide how much ambient occlusion you want,
[5:54] if you want to display the bent normals, and so on.
[5:56] Don't forget that at any point, you can reset your parameters to default by clicking here.
[6:02] Alright, we're now happy with our settings, so let's launch a simple bake.


### Baking example n°1 [6:03]
**Transcript (timestamped):**
[6:05] Like I said earlier, it's best to follow the logical path that goes from the texture set
[6:10] selection to the baker's settings.
[6:12] For the sake of this example, I'm going to bake the whole mesh,
[6:15] so I leave all texture sets selected.
[6:18] As for the bakers, for now I'd like to experiment with the normal only,
[6:22] so I'm going to deselect all the others by alt clicking it.
[6:26] Now careful here.
[6:27] You'll notice that if I select my other texture sets,
[6:31] they still have the other bakers selected.
[6:34] And that's because I need to explicitly apply my selection to all texture sets
[6:38] by clicking here on apply selection to all.
[6:43] Now only the normal will be baked across all texture sets.
[6:47] Okay, I'm all set.
[6:48] Let me just change the output resolution and click on bake texture sets.
[6:53] Just as before, you can choose to bake only the texture set currently selected if you want.
[6:58] Now prepare to be amazed.
[7:00] Baking is no longer a process that freezes your interface.
[7:04] You can interact with your mesh as it gets baked
[7:07] and inspect tricky areas to make sure you don't have any errors.
[7:11] Now that the baking is finished, I'm going to disable the overlays to check if everything is okay.
[7:18] Like in painting mode, pressing B will display the baked map,
[7:21] so I'm going to cycle through them until I get to the normal map.
[7:25] Okay, all looks decent, except this.
[7:30] Something went wrong with the claws, so let's investigate what happened.
[7:34] Pressing M to go back to material mode
[7:37] and hiding the cage and the low poly to check the high poly mesh.
[7:41] See, the claws are missing here, hence the wrong baking that we got in that area.
[7:46] There are different ways we can fix this.
[7:48] We can open our mesh in the modeling tool that we used
[7:51] and re-export a high poly version of the claws
[7:54] and then upload it back in Painter.


### Desynchronize common settings [7:56]
**Transcript (timestamped):**
[7:56] Or we can decide that we don't really need a high poly for that
[8:00] and simply bake the low poly onto itself
[8:03] by enabling use low poly mesh as high poly mesh.
[8:07] As soon as I do that, the high poly mesh disappears,
[8:10] but it does so for all the texture sets, and this is not what I want.
[8:15] What happened is that by default, the common parameters are synchronized across all texture sets,
[8:21] hence the link icon that I mentioned earlier.
[8:23] But there is now a new feature that lets you break that link
[8:27] and adjust the common settings per texture set.
[8:31] So let's uncheck that first and making sure we are in the right texture set,
[8:35] the claws one, click the link icon next to the common parameters.
[8:40] It brings up a pop-up window that says, and let me read that for you,
[8:43] that all the selected texture sets will share the same common parameters.
[8:49] In other words, if I want one texture set to have different settings than the others,
[8:54] all I have to do is to uncheck it from that list.
[8:58] The link has now disappeared for this set,
[9:01] meaning that we can now tweak its parameters without affecting the other texture sets.
[9:07] See? If I change the cage, it only changes for the claws.
[9:12] The other texture sets, on the other hand, remain linked
[9:15] and so the cage offset stays synchronized for them.
[9:18] We can now enable the local yes-hypoly option
[9:21] and relaunch the bake for the claws to see if it fixes the issue.
[9:26] And it does.
[9:28] Being able to synchronize or desynchronize the common settings allows for a much more granular
[9:33] workflow, letting you adjust each texture set individually.
[9:38] You could, for example, have a different group of hypolymeshes,
[9:41] different resolution, and so on.
[9:44] This takes a bit of practice to get used to,


### Troubleshoot artifacts [9:46]
**Transcript (timestamped):**
[9:46] so let me switch to another project to better illustrate it.
[9:50] So I now have this low poly gun that I'd like to bake.
[9:53] I've uploaded the hypoly all right, but I've already noticed an issue.
[9:57] Painter wants me that it found a hard edge without a seam here.
[10:01] This is the pink outline that I mentioned earlier.
[10:04] And if we inspect the mesh real quick in Blender,
[10:07] we can understand better what's going on.
[10:09] A hard edge means that the vertex normals between two faces are split.
[10:14] If I smooth this edge back, then my vertices normal will
[10:18] average in the middle like so, allowing for a clean, continuous bake.
[10:23] If I keep them split, then the baker will have to interpolate somehow that gap between the two
[10:28] normals, and it will result in artifacts, because there is not enough space between the faces in
[10:33] the UVs. To fix this, I can either smooth that edge or separate the UV islands by adding a UV
[10:40] seam here. In this case, I'm just going to smooth it, re-export the mesh, and reload it in Painter
[10:47] by going to Edit, Re-Inport Mesh. See? The issue is gone, and so is the pink outline.
[10:54] This is a very helpful visual cue because it's easy to miss those artifacts,


### Baking example n°2 and match by mesh name [10:55]
**Transcript (timestamped):**
[10:59] especially on complex meshes. Now let's set up our bake.
[11:03] Selecting all my texture sets, and to go faster, I can simply expand the menu here
[11:08] and click on Select All Texture Sets and UV tiles. Then choosing what I want to bake.
[11:13] In this case, I'd like to focus on the normal, ambient occlusion, and curvature.
[11:19] Now remember, if I want to share that selection across texture sets, I have to go to the top
[11:24] right corner here, and click on Apply Selection to All Texture Sets. I can also do it individually
[11:30] per baker. Say for example, I want to add the thickness to it. Then I can right click the baker
[11:37] and say Apply Thickness to All Texture Sets, and then thickness will be baked everywhere.
[11:43] It's a quick way of adding a baker without disrupting the rest of your setup.
[11:47] Now you may have noticed that we can also synchronize or desynchronize settings between texture sets.
[11:53] As you see from the link icon here, the bakers are by default synchronized across all texture sets,
[11:59] and in most cases, this is just as well. So for example, if I decide to bump up the
[12:04] secondary race of the ambient occlusion baker to have a better occlusion quality,
[12:09] this value will be passed on to all the texture sets by default. But since this might also make
[12:16] the process heavier, maybe I want to tone that down for less visible parts of my mesh, like the
[12:21] trigger for example. Now if I want to isolate this set and assign a lower value to it, it's the same
[12:28] process as with the common settings. Simply click on the link next to the relevant baker,
[12:33] then uncheck the texture set you want to single out. Now again, the ambient occlusion settings
[12:40] remain linked for all texture sets, except for the trigger that I can now adjust separately.
[12:46] I can always re-sync everything by clicking on sync settings, and my trigger ambient occlusion
[12:51] will go back to the group settings. Now in the case of this asset, it proves very useful.
[12:57] If it's going to be animated later on, and the magazine of the gun for example is one of the
[13:01] removable parts, then I don't want to bake in the occlusion that comes from the case.
[13:06] See, this would be a problem. To fix this, the usual solution is to go to the common settings,
[13:12] scroll down to the match menu, and select match by mesh name. This ensures that the various parts
[13:19] of the mesh won't occlude each other. But in this case, I do want that mutual occlusion, I just
[13:26] don't want it on the magazine because it's eventually going to be animated. Thanks to the
[13:30] split parameters, I can now enable the match by mesh name only to certain texture sets,
[13:36] allowing me to fix the occlusion for the movable parts. All I have to do is go to the
[13:41] common settings of the magazine texture set, desynchronize it, then enable match by mesh name.
[13:48] Notice that as soon as I do that, I get a warning from the matching by name log.
[13:53] It has listed all the meshes that miss a low poly equivalent. In our case, this won't be a
[13:58] problem, but this is great for tracking naming errors and inconsistencies. Now I also need to go
[14:04] to the occlusion baker, desynchronize it too, and select here as well only some mesh name.
[14:12] Okay, so let's launch the bake, focusing on the magazine by hiding the rest,
[14:17] and investigate the result. Ah, see here, I have a cage issue. The rays don't go deep enough,


### Recap [14:18]
**Transcript (timestamped):**
[14:24] so let's just fix that in the common settings, increase the max rear distance.
[14:30] Perfect, I now have a clean bake for the magazine and it will stay consistent even when the magazine
[14:36] moves or is reloaded. Let's sum up what we covered in this video. So you can now access the baking
[14:42] window by clicking on the croissant icon on the top right corner of the viewport or by pressing F8.
[14:48] New logs have been added to the baking window, letting you keep track of your high poly meshes
[14:53] and warning you of any problem or mismatch. An interactive viewport has been added with
[14:58] baking overlays that give real-time visual feedback to help you adjust your settings and
[15:03] troubleshoot issues. And you now have the ability to synchronize or desynchronize even the common
[15:09] parameters per texture set, which gives you much more control over how to bake specific parts of
[15:14] your mesh. We hope you enjoy these new features and that they will help you create even more beautiful artworks.



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
