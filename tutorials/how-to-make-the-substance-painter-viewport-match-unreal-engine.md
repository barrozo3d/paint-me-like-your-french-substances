---
title: How to Make the Substance Painter Viewport Match Unreal Engine
source: YouTube
url: https://www.youtube.com/watch?v=UOcNnu2uW1Y
author: Quinn Kuslich
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/how-to-make-the-substance-painter-viewport-match-unreal-engine/
frame_count: 0
frame_status: pending-selection
---

# How to Make the Substance Painter Viewport Match Unreal Engine

**Source:** [YouTube](https://www.youtube.com/watch?v=UOcNnu2uW1Y)
**Author:** Quinn Kuslich
**Duration:** 5m43s | 6 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py how-to-make-the-substance-painter-viewport-match-unreal-engine <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Introduction [0:00]
**Transcript (timestamped):**
[0:00] Hello everyone, in this short tutorial, I'm going to cover how you can use the ACE's LUT to make the renderer inside Substance Painter better match the renderer inside UE4.
[0:08] The main reason you would want to do this is because it will make your texturing workflow with Substance Painter faster and more efficient as it will create a nearly one-to-one match between Substance Painter and UE4.
[0:18] In its current state, the Substance Painter renderer fails to show you how certain roughness and metallic values will look inside Unreal,
[0:24] which may force you to go back and adjust certain values to better fit the edge in rendering.
[0:28] Costing you time and in some cases, money.


### Downloading the ACES LUT [0:30]
**Transcript (timestamped):**
[0:30] So let's get started.
[0:32] The first thing you need to do is follow the link in my description to download the ACE's LUT from Brian Lelux's page on ArtStation.
[0:37] You can also follow the link below it directly to the gumroad posting for the same plugin.
[0:41] Also, Brian, I'm really sorry if I mispronounced your last name.
[0:44] Alright, now we open Substance Painter and just to update you guys, what I did was I changed the environment background from Panorama to Studio 5 because this is just what I prefer to work in when I'm texturing assets.


### Importing the ACES LUT into Substance Painter [0:45]
**Transcript (timestamped):**
[0:56] Now we need to import the ACE's LUT.
[0:58] So to do that, we go to File, Import Resources, and we have to add resources.
[1:03] And what you're going to want to do is navigate to where you've unzipped the ACE's files into your hard drive.
[1:10] So what we want to do is we want to grab the ACE's Standard Log and the ACE's UE4 Log, EXR.
[1:15] And these are just like environment color profiles.
[1:17] And we want to define them both as color LUTs because that's what they are.
[1:22] And you want to import those to library your assets.
[1:25] The reason you want to do this is because you're going to have to kind of set up the environment settings for every Substance Painter project you use with this color LUT system.
[1:32] And it's easiest if you just have it in the library your assets because then you never have to re-import them again as long as you're using the same version of Substance Painter.
[1:40] Since I've already installed these, I'm going to forgo the import because there's really no need for me to re-import them.
[1:46] And so go ahead and click Import and it might take a second to get them all in, but they'll be there.
[1:51] Now you have the ACE's LUT system installed into Substance Painter, but what you really need to do is actually activate it now inside of your Substance Project.


### Activating the ACES LUT [1:52]
**Transcript (timestamped):**
[1:59] So for the purposes of this tutorial, I actually grabbed this asset off of ArtStation.
[2:04] I felt it had some really awesome PBR textures and materials on it and a really good differentiation between roughness values in order to kind of illustrate what I'm talking about in between Substance Painter and Unreal 4.
[2:14] So before I ramble on too much, let's just get started.
[2:17] You basically need to go up to the display settings.
[2:20] That's this little display with a gear in it and you click on that and we already set the environment map.
[2:25] And then I also drag the environment opacity from 0 to 100% and that just brings the background from the IRA renderer directly behind your model in the work section of Substance Painter.
[2:36] But what we really are interested in is scrolling down to these settings where we have the color profile and the pulse process effect.
[2:42] So what you're looking for is this tone mapping tab.
[2:44] First, you need to activate pulse process effects and then you need to click on this tone mapping tab so you can drag it down and take a look at it.
[2:51] So the only thing we're really concerned with is first of all activating tone mapping and then restoring the defaults.
[2:58] So everything is as it was when you open the editor the first time.
[3:03] Then you change this linear to log.
[3:06] That allows us to use the ACEs UE4 log that we need in order to make Substance Painter match on Reels renderer.
[3:12] That way we can get a true feeling of our roughness values and metallic values and how they would look in Unreal.
[3:19] Then you scroll down to where it says activate color profile.
[3:22] This is where you're going to use the color LUTs that we just imported.
[3:25] So you click the checkbox to activate it and you'll notice that the screen gets really dark because you have no color LUTs activated yet.
[3:31] And then you click on this in order to pull up your LUT systems and here we're going to click on ACEs UE4 log.
[3:38] And now we've activated it.
[3:41] That's pretty much all you have to do to make Substance Painter match the UE4 renderer in a literal sense.
[3:47] So now we can really see how our roughness and metallic values are going to be affected with an editor.
[3:52] And we can make the necessary tweaks to our materials that we would need for them to look the best they can inside of UE4.
[3:58] And this is like a really great system that I use all of the time
[4:03] because it just kind of speeds up my workflow.
[4:05] And a lot of times you'll work on an asset and Substance Painter and you'll spend a ton of time, you know, going through and texturing it.
[4:11] And then you import it into Unreal and everything looks wrong.
[4:14] And that's because you're working with an IRA renderer with no color LUTs that match UE4.
[4:19] And when you import it into UE4, it doesn't look good.
[4:22] This will change that completely.
[4:24] So now you can understand exactly what your values are going to look like inside Substance Painter before you even imported into UE4.
[4:30] Saving you time and in most professional artist cases, money as well.
[4:34] So just to kind of illustrate how this looks between UE4 and Substance Painter, I actually went in


### UE4 & Substance Painter Side-by-Side Comparison [4:35]
**Transcript (timestamped):**
[4:40] to Unreal and I
[4:43] put this helmet mesh onto my metahuman asset that I've been working on and messing around with over the last few months.
[4:50] And what you can see is, you know, kind of the connect between the asset in Substance and the asset over in UE4.
[4:57] And we can really see how those roughness values have come forward.
[4:59] Obviously the lighting value is very different in this scene because I went for a, you know,
[5:03] completely different lighting setup than I did in Substance Painter.
[5:06] And if I really wanted to do a true match, I would have to actually take an HGRI inside of my UE4 scene and put it into Substance Painter.
[5:12] But overall the material values we're seeing on the Substance Painter asset and the Unreal asset are pretty close when it comes to roughness value and metallic value.


### Outro + Creepy Metahuman Test [5:20]
**Transcript (timestamped):**
[5:20] Thanks for watching this video.
[5:22] If you have any questions for me, just leave a comment.
[5:24] I try to answer any questions left on my tutorials and feel free to check out some of my other asset creation and VR development tutorials
[5:31] and be sure to check out some of my game analysis videos as well.
[5:34] Also, I hope you enjoyed this really creepy facial capture render of my metahuman wearing this helmet.



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
