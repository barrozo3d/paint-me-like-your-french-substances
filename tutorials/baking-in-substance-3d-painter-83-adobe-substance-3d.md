---
title: Baking in Substance 3D painter 8.3 | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=hYtHp4IXvsM
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "8.3.0 (stated in title; exact match confirmed against references/release-notes-painter-8.3.md — see App & Version note)"
tags: [baking, mesh-maps, high-to-low-poly, cage, ambient-occlusion, curvature, thickness, position-map, world-space-normal, id-map, texture-set, opacity, python-scripting, python-api, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/baking-in-substance-3d-painter-83-adobe-substance-3d/
frame_count: 10
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Baking in Substance 3D painter 8.3 | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=hYtHp4IXvsM)
**Author:** Adobe Substance 3D
**Duration:** 15m26s | 9 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


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

## Captured Frames

- [1:01] tutorials/frames/baking-in-substance-3d-painter-83-adobe-substance-3d/frame_000.jpg
- [2:52] tutorials/frames/baking-in-substance-3d-painter-83-adobe-substance-3d/frame_001.jpg
- [3:37] tutorials/frames/baking-in-substance-3d-painter-83-adobe-substance-3d/frame_002.jpg
- [6:53] tutorials/frames/baking-in-substance-3d-painter-83-adobe-substance-3d/frame_003.jpg
- [7:41] tutorials/frames/baking-in-substance-3d-painter-83-adobe-substance-3d/frame_004.jpg
- [8:35] tutorials/frames/baking-in-substance-3d-painter-83-adobe-substance-3d/frame_005.jpg
- [10:01] tutorials/frames/baking-in-substance-3d-painter-83-adobe-substance-3d/frame_006.jpg
- [11:37] tutorials/frames/baking-in-substance-3d-painter-83-adobe-substance-3d/frame_007.jpg
- [13:12] tutorials/frames/baking-in-substance-3d-painter-83-adobe-substance-3d/frame_008.jpg
- [14:24] tutorials/frames/baking-in-substance-3d-painter-83-adobe-substance-3d/frame_009.jpg

---

## Structured Notes

### Core Technique
Painter 8.3's ground-up rebuild of baking into a dedicated, non-blocking **Baking Mode** (F8) with a fully interactive viewport (live cage/high-poly/low-poly overlays you can tweak with instant visual feedback instead of blind trial-and-error bakes), plus a new synchronize/desynchronize system that lets per-Texture-Set and per-baker settings either follow shared "common" values or break off and be tuned independently — including Match by Mesh Name applied selectively to just the parts that need it.

### Summary
Official Adobe walkthrough (a dragon model, then a submachine-gun model) of the then-brand-new dedicated Baking Mode introduced in Painter 8.3, replacing the old inline "Bake Mesh Maps" dialog. **Access:** the croissant-shaped icon at the top-right of the viewport, the Mode menu, or the **F8** shortcut; return to painting via "Return to painting mode" or the brush icon. **Interface tour:** Texture Set List + selectable UV tiles (top right, lets you bake only specific mesh parts) → individual Mesh Map Bakers with a **link icon** per baker (shared/synchronized settings indicator) → Baker Settings panel for the currently selected baker → Baking Log at the bottom, which now also tracks high-poly mesh loading and any high/low-poly mismatches, with warnings that point directly at the offending setting. **Interactive viewport / Baking Visualization panel:** overlays for the high-poly mesh (blue), the cage (yellow tint + wireframe, showing exactly how rays will be cast), missing-seam warnings on hard edges (pink outline), and the low-poly/"Project mesh" itself shown with an adjustable neutral material (quality, roughness, metallic, bent-normal options) for post-bake inspection; all overlays can be hidden individually, and cage-offset sliders are exponential (fine control at small values) with full undo (Ctrl+Z) support. **Baking workflow:** select Texture Sets/UV tiles → select which bakers to run (Alt-click to isolate one) → explicitly **Apply Selection to All Texture Sets** if you want the same baker choice everywhere (baker selection is NOT synchronized by default) → set output resolution → **Bake Texture Sets** (or bake just the selected set) — the whole interface stays responsive during the bake, so you can keep inspecting the mesh while it runs. Press **B** post-bake to cycle through baked-map preview channels; press **M** to return to material/high-poly inspection mode. **Fixing baking artifacts (claws example):** a bad or missing high-poly region produces visibly wrong output on that baked map; fixes are either re-exporting a corrected high-poly from the DCC tool, or enabling **"Use Low Poly Mesh as High Poly Mesh"** for a self-baked (cage-less) result — but this common-settings toggle is synchronized across all Texture Sets by default, so changing it for one part changes it everywhere unless you first **break the link** (click the link icon next to Common Settings, uncheck the Texture Set you want to isolate from the shared pop-up list) to desynchronize just that Texture Set. **Hard-edge/seam artifacts (gun example):** a pink outline flags a hard edge without a matching UV seam — vertex normals split across two faces there confuse the baker's UV-space interpolation; fix by smoothing the edge (or adding a UV seam) in the DCC tool, then **Edit > Re-Import Mesh** in Painter to reload without restarting the project. **Granular per-baker sync (gun example continued):** individual bakers (not just the whole Common Settings block) can also be synchronized/desynchronized via their own link icon — demonstrated by giving the trigger a lower Ambient Occlusion secondary rays value than the rest of the mesh, and re-syncing later via **Sync Settings**. Right-clicking a baker also offers **Apply [Baker] to All Texture Sets**, a quick way to add a new baker everywhere without disturbing the rest of the per-Texture-Set setup. **Selective Match by Mesh Name (magazine example):** for an asset with parts meant to be animated/removable (e.g. a magazine), global mutual occlusion is usually wanted between parts EXCEPT the moving one; the fix is desynchronizing just that Texture Set's Common Settings, enabling **Match by Mesh Name** there (Common Settings > Match dropdown), then also desynchronizing and enabling Match by Mesh Name on the relevant Ambient Occlusion baker specifically — enabling Match by Mesh Name immediately surfaces a **Matching By Name** log tab listing any mesh names missing a low-poly counterpart, useful for catching naming inconsistencies even when no fix is currently needed.

### Key Steps
1. **Enter Baking Mode** via the croissant icon (top-right of the viewport), the Mode menu, or the **F8** shortcut; return to painting via "Return to painting mode" or the brush icon.
2. **Select Texture Sets and UV tiles** to bake (top-right panel) — both are individually selectable, so you can bake only specific mesh parts. Use the panel's "Select All Texture Sets and UV Tiles" shortcut to grab everything quickly.
3. **Load high-poly mesh(es)** in the Command/High Poly Parameters settings; watch the Baking Log to confirm successful loading and catch any high/low-poly mismatch warnings (which link directly to the offending setting).
4. **Read the interactive viewport overlays:** yellow tint + wireframe = the cage (ray-casting boundary), blue = the high-poly mesh, plus the low-poly "Project mesh" itself — all three can be shown simultaneously for direct visual feedback.
5. **Tune the cage interactively:** adjust Max Frontal Distance / Max Rear Distance while watching the cage in the viewport wrap around the model live; matching errors appear in red if pushed too far. Sliders are exponential for fine control; Ctrl+Z undoes the last adjustment.
6. **Use the Baking Visualization panel's individual toggles** to hide/show the high-poly mesh, the cage (with its own color/opacity), missing-seams-on-hard-edges warnings, and the low-poly/Project mesh (shown with an adjustable neutral material — quality, roughness, metallic, bent normal — for post-bake artifact inspection).
7. **Choose which bakers to run** (Normal, World Space Normal, ID, Ambient Occlusion, Curvature, Position, Thickness, Height, Bent Normals, Opacity, etc.) by Alt-clicking to isolate one; remember baker selection is per-Texture-Set by default, so click **"Apply Selection to All Texture Sets"** to broadcast your choice everywhere.
8. **Set output resolution, then click Bake Texture Sets** (or bake just the currently selected Texture Set) — the UI remains fully interactive during the bake; you can keep inspecting the mesh while it processes.
9. **After baking, press B to cycle through baked map previews**, and **M** to return to material/high-poly inspection — use this to spot artifacts (e.g. a body part with no matching high-poly geometry bakes incorrectly).
10. **Fix a missing-high-poly-detail artifact** either by re-exporting a corrected high-poly mesh from your DCC tool and re-importing, or by enabling **"Use Low Poly Mesh as High Poly Mesh"** for that part (self-bake, no cage needed).
11. **Desynchronize Common Settings for one Texture Set** before making a part-specific change like step 10: click the **link icon** next to Common Settings, uncheck the Texture Set(s) you want isolated from the shared pop-up list — that Texture Set's cage/common parameters can now be tuned independently without affecting the rest.
12. **Diagnose a pink hard-edge-without-seam warning** by checking the mesh in your DCC/modeling tool: a hard (non-averaged) edge with insufficient UV-island spacing causes normal-interpolation artifacts at the bake. Fix by smoothing the edge (average the vertex normals) or by adding a UV seam there.
13. **Reload a fixed mesh without restarting the project:** Edit > **Re-Import Mesh** — the pink warning outline disappears once the fix lands.
14. **Desynchronize an individual baker (not just Common Settings)** the same way — click that baker's own link icon, uncheck the Texture Set to isolate, adjust its parameter (e.g. a lower Ambient Occlusion secondary-rays value for a less-visible part), and use **Sync Settings** later to re-join it to the shared group value.
15. **Quickly add a baker to every Texture Set without disturbing existing per-set setups:** right-click the baker in the Mesh Map Bakers list and choose **Apply [Baker] to All Texture Sets**.
16. **Set up selective Match by Mesh Name for an animated/removable part:** desynchronize that Texture Set's Common Settings, open the **Match** dropdown, select **By Mesh Name** — this immediately surfaces a **Matching By Name** log tab listing any mesh names lacking a low-poly counterpart (useful diagnostic even beyond this specific use case).
17. **Also desynchronize and enable Match by Mesh Name on the relevant baker itself** (e.g. Ambient Occlusion) for that same Texture Set, so mutual occlusion with the rest of the mesh is suppressed only for the part that will move independently (e.g. a gun magazine) while staying intact everywhere else.
18. **Isolate and re-bake just the affected Texture Set** (hide the rest via the Texture Set List) to verify the fix, adjusting cage rear/frontal distance further if the rays still don't reach deep enough.

### Layers / Tools / Settings
- **Baking Mode entry points:** croissant icon (viewport top-right), Mode menu, **F8** shortcut
- **Texture Set List + UV tiles** (top-right, individually selectable) → **Mesh Map Bakers** list (each with a link/sync icon) → **Baker Settings** panel → **Baking Log** (tracks high-poly loading, mismatches, links warnings to their source setting)
- **Bakers covered:** Normal, World Space Normal, ID, Ambient Occlusion, Curvature, Position, Thickness, Height, Bent Normals, Opacity
- **Baking Visualization panel toggles:** high-poly mesh (blue), Cage (surface/wireframe, color + opacity), missing-seams-on-hard-edges (pink), Project mesh/low-poly (adjustable neutral material: quality, roughness, metallic, bent normal)
- **Cage controls:** Max Frontal Distance, Max Rear Distance (exponential sliders), live red error highlighting when mismatched, Ctrl+Z undo
- **Sync system:** link icon on Common Settings and on each individual baker — click to open a per-Texture-Set opt-out list (desynchronize), **Sync Settings** to re-join
- **High-poly options:** "Use Low Poly Mesh as High Poly Mesh" (self-bake, no cage)
- **Match dropdown (Common Settings):** includes **By Mesh Name** — surfaces a **Matching By Name** log tab listing meshes missing a low-poly counterpart
- **Right-click baker context menu:** "Apply [Baker] to All Texture Sets"
- **Post-bake inspection shortcuts:** **B** cycles baked-map previews, **M** returns to material/high-poly mode
- **Edit > Re-Import Mesh** — reload a corrected mesh without restarting the project
- **Bake Selected Textures** / **Bake Texture Sets** action buttons; "Apply Selection to All Texture Sets" for broadcasting baker choice

### Difficulty
Intermediate to Advanced (the basic bake-and-go workflow is approachable, but the synchronize/desynchronize-per-Texture-Set system and Match-by-Mesh-Name troubleshooting require understanding Painter's Texture Set/baker settings hierarchy).

### App & Version
Substance 3D Painter **8.3.0** — stated directly in the video title, and every feature described (dedicated Baking Mode replacing the old inline dialog, F8 shortcut, croissant icon, interactive viewport with cage/high-poly/low-poly overlays and live cage feedback, exponential cage sliders, the new Baking Log tracking mesh loading/mismatches, baker-settings synchronization with per-Texture-Set/per-baker desync via the link icon, Match by Mesh Name selective application) is an exact match against this skill's own `references/release-notes-painter-8.3.md`, which documents Painter 8.3.0 (January 10, 2023) as introducing precisely this "Dedicated Baking Mode" — confirming this video is a first-party feature-launch tutorial for that exact release, not a later video mislabeled with an old version number.

### Tags
`baking`, `mesh-maps`, `high-to-low-poly`, `cage`, `ambient-occlusion`, `curvature`, `thickness`, `position-map`, `world-space-normal`, `id-map`, `texture-set`, `opacity`, `python-scripting`, `python-api`, `intermediate`, `advanced`

---

## Related Tutorials
- [Hand Painted Workflow in Substance 3D Painter](hand-painted-workflow-in-substance-3d-painter-adobe-substance-3d.md) — same channel (Adobe); uses AutoCage-assisted baking (11.0.0+) as a starting step, a later evolution of the baking pipeline this video documents at its 8.3.0 foundation.
- [Complex Wooden Medieval Door Tutorial in Substance 3D Painter](complex-wooden-medieval-door-tutorial-in-substance-3d-painter.md) — same channel (Adobe); production use of Auto-Cage baking (11.0.0+), useful to read alongside this video to see how the baking-mode fundamentals here evolved by 11.0.0.
- [HOW to Make UDIMS for UNREAL ENGINE](how-to-make-udims-for-unreal-engine.md) (Jared Chavez) — different creator; applies these general baking-mode fundamentals to a multi-tile UDIM mesh specifically, including the `Use UV Tile` import requirement and a Thickness-map UDIM-seam gotcha not covered here.
- `references/release-notes-painter-8.3.md` — this skill's own version-tracker entry for the exact release this video demonstrates; every UI element and workflow named in this video (Baking Mode, F8, Baking Log, cage overlays, settings synchronization, Match by Mesh Name) is independently confirmed there.
