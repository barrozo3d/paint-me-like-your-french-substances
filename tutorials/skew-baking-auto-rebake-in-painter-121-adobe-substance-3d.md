---
title: Skew Baking & Auto Rebake in Painter 12.1 | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=WwyElRpiQgY
author: Adobe Substance 3D
ingested: 2026-08-12
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/skew-baking-auto-rebake-in-painter-121-adobe-substance-3d/
frame_count: 0
frame_status: pending-selection
---

# Skew Baking & Auto Rebake in Painter 12.1 | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=WwyElRpiQgY)
**Author:** Adobe Substance 3D
**Duration:** 7m2s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py skew-baking-auto-rebake-in-painter-121-adobe-substance-3d <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hi, welcome to this video on the new baking features in Substance Painter 12.1.
[0:07] In this video, we're going to talk about a couple of new baking features, which is mainly some UI New X improvements,
[0:12] ping the auto rebake function. Let's get started. First, we're going to the baking mode, click here.
[0:18] And before I even delve into this queue, let's take a look at what has changed here. We've got some changes in the UI.
[0:25] First thing you might notice is that the mesh map baker's list has changed. You get some new options here.
[0:31] And the main ones are that we have a different organization where you can easily check in and check all.
[0:36] And we have moved common settings out into its own separate button. So if I click on a map, such as the Empty Occlusion,
[0:42] I see the map settings. If I click on common settings, I see the common settings, but they are separate windows now.
[0:47] So if you would like to, you could even split them up into two separate areas and look at the mesh map settings and common settings at the same time.
[0:54] If you don't have to do this, you could just keep them together as this default setup does.
[1:00] Now, the next thing is we've got these little buttons next to individual maps, and these are pretty interesting.
[1:05] If you click this one, you'll instantly view a bake map. Now, we don't have any maps baked yet, so they don't do anything yet.
[1:11] But if we would want to bake our normal map, we could, for example, click this one, it instantly bakes that map and we can take a look at it.
[1:18] And the last one is the auto rebake toggle. Now we'll talk a bit more about that one later.
[1:24] Now, at the top of the common settings, you also see that we've started introducing categories for things.
[1:29] We've got the common settings, we've got the cage settings, and we've got the skew correction settings.
[1:34] If you click on these tabs, you quickly jump to the relevant section.
[1:38] So because the section's gotten bigger, we've made it easier to navigate through them.
[1:42] So to use these skew correction, which you're probably pretty interested in, you want to start painting skew correction, but it doesn't let you.
[1:48] And if you hover over it, it'll tell you why we need to load a high-poly mesh.
[1:52] So let me do that really quickly.
[1:54] Load a high-poly mesh, scroll down, and then I can actually start painting skew correction.
[1:59] Now, when I do that, it automatically bakes my normal map because skew is actually something that you easily see in your normal map.
[2:06] And this mesh, we've specifically chosen this because skew will be very visible in here.
[2:10] So if I zoom in, you see that because of the low-poly nature of this mesh, it's fairly low-poly.
[2:15] It's got a detailed high-poly. We see some heavy skewing.
[2:19] You'd expect these bolts to be head-on, but it's not.
[2:22] And same as here, you can actually see it.
[2:25] Now, these strange vectors that are peering over it, you can tweak them.
[2:28] Once you go into the paint skew mode, you can open the skew vectors.
[2:32] You can change their length. You can change their density.
[2:35] And they'll actually show you why the skewing is happening.
[2:38] The skew vectors represent the direction in which the baked rays are traced.
[2:42] And if these deviate a lot from what you'd imagine the surface is pointing at,
[2:47] you tend to get these skew errors if your high-poly is fairly detailed.
[2:50] So what skew correction lets you do is it lets you paint those out.
[2:54] So how do you paint skew correction? Well, pretty easy.
[2:57] You go into that mode, you use regular brush tools and you simply paint.
[3:01] And what is corrected appears in blue.
[3:04] You let go and auto-rebake is instantly going to rebake that.
[3:08] Let's just do that again. Let me paint here real quick. Go over it.
[3:13] So you let go, auto-rebake picks up on it.
[3:17] Now auto-rebake is going to rebake a single map.
[3:20] It's right now set up on the normal map and it does this automatically
[3:23] when you enter skew correction.
[3:25] The very first time if you tend to turn it off, then go back, it won't turn it on
[3:28] and you have to toggle it yourself.
[3:30] If you would like another map to be baked for your skew correction, you can do that.
[3:33] But you can only bake one at a time.
[3:36] Only one map can be auto-rebaked to ensure that the performance is good.
[3:39] So when it comes to skew correction, there's a few other things you can do.
[3:42] So let's get a little bit closer in here, make my brush a bit smaller.
[3:45] There's some skewing going on here. Let me just paint over that.
[3:49] Get this to bake.
[3:51] Now if we get closer, then you can see that we are getting scene errors.
[3:54] Because we've painted over UV scene errors skew correction,
[3:57] doesn't quite like that. We're getting problems whether rays are split
[4:00] and you're getting missed areas and your normal map just doesn't look very good.
[4:03] So let's go back to the skew correction.
[4:06] Now you'd expect the solution to be to just press X
[4:09] and then paint over those areas in black manually.
[4:12] But that's quite a bit of work. You might not have time for that.
[4:15] So instead, what you can do is there's a setting down here,
[4:18] edge protection. If you turn that on, it automatically adds
[4:21] a protective mask on the edges that's based on your
[4:24] UV borders and your hard edges. You can change the distance, right?
[4:27] So I can make it a bit smaller like so.
[4:30] And I can even change the contrast to make it look a bit smaller.
[4:34] Like so. And I can even change the contrast for it to be softer or harder.
[4:37] So in this case, I'll just make it a bit softer.
[4:40] This means that you get easy skew correction
[4:43] and you don't have to pay attention to those edges that you might paint over.
[4:48] Now another tool that you can use here is the
[4:51] polygon fill. And the polygon fill works extra well together
[4:54] with the edge correction. Because if I were to fill
[4:57] entire polygons like this, it'd be pretty useless
[5:00] because I would always be going up until edges.
[5:03] So in a lot of cases, you might even be able to work
[5:06] by simply using the polygon fill
[5:09] and selecting entire polygons at a time
[5:12] like that. That'll just give you a very
[5:15] rough and blunt tool, but it might work in some cases.
[5:18] Now as expected, all the regular hotkeys for you
[5:21] tools such as one, two and four for these tools, they work.
[5:24] You can use X to invert the color. There's a color picker up top
[5:28] to choose if you want to be black or white. You can enable
[5:31] symmetry and you'll notice then the brush tool, you get
[5:34] quick controls here like size, flow, stroke,
[5:37] capacity and spacing. Now if I
[5:40] would right click, I still get access to the
[5:43] full brush properties in this case. So
[5:46] if you were to make any changes, you could still do it
[5:49] in here as well. Then lastly, we've made a few small
[5:52] updates down here. If you go into the
[5:55] menu, we actually need a different mesh for that.
[5:58] If you're used to managing your syncing of layers, just this
[6:01] one here, this menu tended to be a bit confusing. So what we've
[6:04] done is we have changed the wording, changed the design
[6:07] slightly to make these a little bit easier to understand.
[6:10] Things are now called checked instead of selected. We have
[6:13] harmonized terms to use sync. So this just demystifies
[6:16] these unusual menus just a little bit. Additionally,
[6:19] what we've also done is the bake button down here. It's changed.
[6:22] So drop down there because you now have quick access to
[6:25] quick baking with the cross on button over here. Instead,
[6:28] this button is a single action and between brackets, it shows you
[6:31] the amount of maps that will bake. So that is the
[6:34] texture sets times the amount of UV tiles times
[6:37] the check textures that are enabled here. So in this case, if you were to bake
[6:40] everything, you would bake 21 maps. You could also of course
[6:44] individually bake a single map so you don't have to juggle this
[6:47] check state anymore. All of that to make baking
[6:50] smoother, easier and faster to access. That's about it for these changes.
[6:54] I hope they're useful and let us know in the comments if you have any feedback.



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
