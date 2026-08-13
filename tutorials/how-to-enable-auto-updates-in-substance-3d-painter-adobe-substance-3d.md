---
title: How to Enable Auto-Updates in Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=13B82VtLuQY
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "11.0.0"
tags: [layers, masks, alpha, beginner]
extraction_status: complete
frames_dir: tutorials/frames/how-to-enable-auto-updates-in-substance-3d-painter-adobe-substance-3d/
frame_count: 5
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# How to Enable Auto-Updates in Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=13B82VtLuQY)
**Author:** Adobe Substance 3D
**Duration:** 4m33s | 3 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Introduction [0:00]
**Transcript (timestamped):**
[0:00] Hi, in this video we'll talk about the new auto-updater in Substance 3D Painter 11.
[0:07] You can find the new auto-updater here at the bottom.
[0:10] By default, everything is disabled.
[0:11] In the automatic updates, you can set specific types of updates.
[0:15] Let's create a hypothetical situation and I'll show you how it works.


### Using auto-update with image files [0:19]
**Transcript (timestamped):**
[0:19] First of all, inside Photoshop, I've created a very small, simple decal texture.
[0:24] This decal texture will be brought in to Painter.
[0:27] So I'll drop it in.
[0:29] I'll say that this is a texture which goes into the project and I'll import it.
[0:35] Then I'll simply drop it on my mesh and use it as a mask.
[0:40] Make it a little bit bigger.
[0:42] Right, so we've brought this in and we've decided to make a change to our texture.
[0:46] So I'm going to Photoshop.
[0:47] I'll just change this a little bit, change the text to say two.
[0:51] And we're going to export it again to the exact same file.
[0:55] All right, if I jump back into Painter, this doesn't update automatically.
[0:59] You can already do that now, update things, but it takes a few manual steps.
[1:02] You'd have to right click it.
[1:03] You would have to reload it.
[1:04] You would have to go in here into the mask and redrag it in there again so that takes
[1:08] quite a bit of time.
[1:09] What you can do instead is use the auto-updater to turn on two types of automatic updating.
[1:14] First of all, it's automatic updating in the assets panel.
[1:16] It means everything in the assets panel here will automatically reload when it finds a
[1:20] new version on this.
[1:21] So if I turn that on, you see instantly it's detected that there was a new decal.
[1:25] And it has loaded it.
[1:27] You can see that it hasn't updated in the project itself.
[1:30] So where it's used in the stack, that is not updated.
[1:32] We've decided to make this an option because depending on how you're working, you might
[1:36] want or not want this.
[1:38] So if we turn on resources used in project, you see that it instantly updates as well.
[1:43] And if we do another change, show you like, so by changing this to three, wait for the
[1:48] update to pass.
[1:50] And as you see, it instantly updates in your project.
[1:53] So this means that working with external resources that you're changing in different
[1:56] programs like Photoshop, design or anything is much faster.


### Using auto-update with filters [2:00]
**Transcript (timestamped):**
[2:00] Let me show you another way to work that's a little bit more advanced.
[2:03] All right.
[2:06] So I've got a case here where we have a nice scene and we want to use a filter on it.
[2:10] It's going to be a custom version of the stylization filter that ships with Substance Painter.
[2:15] The scene is set up and I'm going to go to designer where I've got my stylization filter
[2:20] and we're going to send the initial version.
[2:22] This is the unchanged one.
[2:23] So as usual, you can right click and I can say send to which you substance 3D painter,
[2:29] go back to painter, stylization custom.
[2:31] This is the one that I'm making has appeared.
[2:33] We're just going to apply it.
[2:35] So I'll drag and drop it on as a new layer.
[2:37] As you see, the coffee pot changes to be stylized and then we're going to switch to the table.
[2:41] We'll also drag it on there.
[2:43] So this is a common use case where you would be making something in designer.
[2:46] You want to go back and forth with painter.
[2:48] You make a change.
[2:49] You want to see what happens there.
[2:50] And before you'd have it pop up in here.
[2:52] You'd have to drag it in all the time.
[2:54] It'd be very annoying to get things to update.
[2:56] So like we set up before, I can in you, I've set up assets panel to update automatically
[3:01] and I've set resources used in project update automatically.
[3:03] Now this one, I said we're going to mention it before and this is skip assets when the
[3:07] parameters mismatch.
[3:09] When you're working on a filter and you're setting up the parameters, it might be that
[3:12] you rename, move or delete parameters.
[3:15] And in this case, this is sort of safety setting where it will skip them if the parameters
[3:19] mismatch.
[3:20] If you turn it off, which I might want, it'll actually says in the description here, it
[3:25] will set any unmatched parameters to their default value, which is a safe option to do
[3:30] it.
[3:31] But you can turn it off in case you want to play it safe and not have any mismatched
[3:34] parameter options appear.
[3:36] Now, let's all talk.
[3:38] Let's just show you what happens when you want to go back and forth.
[3:40] I'm going to go into designer and I'm going to add a small change here.
[3:43] So I'll take my base color here and I'm going to add a blur after that.
[3:49] And I'm going to expose this value.
[3:53] That's a new option.
[3:54] The base color will be blurred before it's filtered into a stylized version.
[3:57] And done.
[3:58] I'll say send to, send to substance 3D painter again.
[4:03] There we go.
[4:04] It's just updated and you see that we have a blurred version.
[4:06] So if I now select my stylization custom and scroll down, my intensity blur has appeared
[4:12] here at the bottom and you see I have control over that.
[4:16] So this option using it together with designer with the full auto update makes it much easier
[4:20] to go back and forth and set up your own custom assets.
[4:22] You don't have to do all of these steps of dragging it in again and updating it or using
[4:26] the resource update.
[4:27] So there's that.
[4:28] Enjoy.
[4:29] And that's it for the auto updater.



---

## Captured Frames

- [0:10] tutorials/frames/how-to-enable-auto-updates-in-substance-3d-painter-adobe-substance-3d/frame_000.jpg
- [1:22] tutorials/frames/how-to-enable-auto-updates-in-substance-3d-painter-adobe-substance-3d/frame_001.jpg
- [1:40] tutorials/frames/how-to-enable-auto-updates-in-substance-3d-painter-adobe-substance-3d/frame_002.jpg
- [3:05] tutorials/frames/how-to-enable-auto-updates-in-substance-3d-painter-adobe-substance-3d/frame_003.jpg
- [4:05] tutorials/frames/how-to-enable-auto-updates-in-substance-3d-painter-adobe-substance-3d/frame_004.jpg

---

## Structured Notes

### Core Technique
Auto-Updater settings panel (bottom of the Assets/Shelf panel, all off by default) that automatically reloads externally-modified resources — image files re-exported from Photoshop, or filter/graph assets round-tripped from Substance 3D Designer — without the old manual right-click → reload → redrag-into-mask routine.

### Summary
Short feature explainer, split into two demos. First: a decal PSD is imported into Painter as a project texture and dragged onto a mask; without auto-update, re-exporting the PSD from Photoshop does nothing in Painter until it's manually reloaded and redragged. Turning on **Assets panel** auto-update makes the Shelf/library thumbnail refresh instantly when a new file version is detected, but the layer stack still isn't updated — a separate **Resources used in project** toggle is needed to also refresh every place that resource is actually used (e.g. the mask), and both together make external-tool round-tripping (Photoshop, or any other editor) effectively instant. Second, more advanced demo: a custom Stylization filter is built as a Substance 3D Designer graph, sent to Painter via "Send to Substance 3D Painter," and applied as a filter layer on two objects; with both auto-update toggles already on, editing the graph back in Designer (e.g. adding an exposed Blur-intensity parameter before the stylization step) and re-sending it updates the filter live in Painter, including exposing the new parameter in its Properties panel — no manual re-drag needed. A third toggle, **Skip assets when their parameters mismatch** (Advanced Settings), is a safety net for this Designer workflow: if a graph's parameters get renamed/moved/deleted between sends, this setting skips applying the mismatched update rather than silently resetting affected parameters to default.

### Key Steps
1. Open the Auto-Updater controls at the bottom of the Assets/Shelf panel — everything is disabled by default.
2. Import an external image (e.g. a PSD decal from Photoshop) as a project texture, drag it onto the mesh, and use it as a mask.
3. Edit and re-export the source file to the same path from the external tool; without auto-update, Painter does not reflect the change until you manually right-click → reload the asset and redrag it into the mask.
4. Enable **Assets panel** auto-update — the Shelf/library thumbnail now refreshes automatically the instant a new file version is detected on disk.
5. Enable **Resources used in project** auto-update — every place that resource is actually used in the layer stack (not just the library thumbnail) now updates automatically too, essentially instantly after each external re-save.
6. Advanced workflow: build a custom filter (e.g. a Stylization-based graph) in Substance 3D Designer, right-click → **Send to Substance 3D Painter** to bring it in as a Shelf asset, then drag it onto a layer in Painter as normal.
7. With both auto-update toggles already on, edit the Designer graph (e.g. add a Blur node before the stylization output and expose its intensity as a parameter) and **Send to Substance 3D Painter** again — the filter updates live in the already-applied layer, including any newly exposed parameter appearing in its Properties panel, with no manual re-drag or reload step.
8. Use **Skip assets when their parameters mismatch** (Advanced Settings) as a safety toggle for the Designer round-trip: if renaming/moving/deleting graph parameters between sends would otherwise cause Painter to reset the mismatched parameters to their default value, this setting instead skips applying that particular update.
9. Manual fallback buttons (**Update Assets panel** / **Update resources used in project**) remain available in the same panel for one-off refreshes without leaving auto-update on permanently.

### Layers / Tools / Settings
- Auto-Updater panel (bottom of Assets/Shelf): **Assets panel** toggle, **Resources used in project** toggle, **Update every [interval]** setting
- Advanced Settings: **Skip assets when their parameters mismatch**
- Manual buttons: **Update Assets panel**, **Update resources used in project**
- Substance 3D Designer → Painter round-trip: right-click graph → **Send to Substance 3D Painter**
- Demoed on: an image-based mask (PSD decal) and a custom Designer-built Stylization filter graph

### Difficulty
Beginner (the core toggle) to Intermediate (the Designer round-trip use case).

### App & Version
**Substance 3D Painter 11.0.0** — stated explicitly on screen and in narration ("the new auto-updater in Substance 3D Painter 11"); matches `references/release-notes-painter-11.0.md`'s "Auto-update feature for modified assets" entry.

### Tags
`layers` `masks` `alpha` `beginner`

---

## Related Tutorials
- **"6 Powerful New Filters in Substance 3D Painter"** (`tutorials/6-powerful-new-filters-in-substance-3d-painter-adobe-substance-3d.md`, video `aCi0RG9-9so`) — same 11.0.0 release; that video's Stylization filter is the same one customized in Designer and round-tripped here.
- **"Stylized Asset Setup in Painter: Auto-Cage, PSD Workflows & Smart Detailing"** (`tutorials/stylized-asset-setup-in-painter-auto-cage-psd-workflows-smart-detailing-adobe-su.md`, video `LRy-Nc7B_bk`) — that video's PSD-Auto-Update workflow (decal texture, "Import As project", refresh icon with the same two checkboxes) is exactly the feature this video explains in more depth, applied there to a stylized still-life scene.
