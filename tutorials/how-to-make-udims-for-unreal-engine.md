---
title: HOW to Make UDIMS for UNREAL ENGINE
source: YouTube
url: https://www.youtube.com/watch?v=fonCA0jiEF8
author: Jared Chavez
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/how-to-make-udims-for-unreal-engine/
frame_count: 0
frame_status: pending-selection
---

# HOW to Make UDIMS for UNREAL ENGINE

**Source:** [YouTube](https://www.youtube.com/watch?v=fonCA0jiEF8)
**Author:** Jared Chavez
**Duration:** 10m39s | 8 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py how-to-make-udims-for-unreal-engine <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hey, I'm Jared. Today we're going to take a look at UVs and UDIMs. So for those of you
[0:07] who've been following the channel, a couple months back I released a video showing how
[0:11] I went about sculpting the details on my Neomorph model. Well, the next obvious phase that we're
[0:16] going to be moving into is going to be creating UVs so that I can start to get my bakes done
[0:21] for this character. So that's where we're going to be headed next with this video. For


### Project Overview [0:22]
**Transcript (timestamped):**
[0:25] this project I actually wanted to try something out a little bit different than my normal
[0:29] workflow, which was going to be using UDIMs inside of UE5. I was actually unfamiliar with
[0:35] the fact that UDIMs were supported inside of Unreal until someone had pointed it out
[0:39] to me on-street. For this sculpt, it seemed like a really good candidate because I really
[0:44] wanted to try and push the level of detail that I put into the model. I really wanted
[0:49] to see if I could show all of that little fine, crisp detail and pull out as much information
[0:55] inside of UE5 as possible. With that said, let's take a look at getting started inside


### UV Mapping [0:58]
**Transcript (timestamped):**
[1:01] of Maya. For the mesh with this asset, I didn't actually spend any time creating a low poly
[1:07] for it. I just created a Z-Remesh for this project in particular. I didn't have any
[1:12] plans to animate this character, and I really just wanted to work fast so I used the quickest
[1:18] solution. So to aid with keeping things fast, I decided to Z-Remesh the model from ZBrush
[1:24] and then just take that mesh that I had used for my high poly sculpt and take the lowest
[1:29] subdivision level and build my UVs off of that. The UV mapping process for this character
[1:35] was actually pretty straightforward, mostly because the fact that it was an organic model
[1:40] so I didn't have to worry about things like assets or accessories on the character. The
[1:45] first thing that I needed to do to start my UV process was create a base to start working
[1:50] off of and then I could start making my cuts on my UVs. The first cuts I started by making
[1:57] were cuts around joint areas like the shoulders and the hips. Once I had those cuts, I wanted
[2:06] to make sure to try and squeeze as much out of each texture set as I possibly could. So
[2:11] to help with that, I added cuts on the wrists and the ankles so that I could just get a
[2:15] little bit more resolution for those areas independent from the rest of the body. Lastly
[2:21] was the cut for the head as that was going to be needing some separate space from the
[2:25] rest of the body as well. After going through and creating my initial cuts, I made some
[2:33] seams on the insides of the limbs where I could start to lay out some of the UVs. The
[2:53] torso I used seams on the sides to cut the mesh so that I was able to place both halves
[2:58] on a single tile space. Same with the head. I split the head right down the middle and
[3:04] created a UV seam to split it directly in half. Once I had all the seams set up, I can start
[3:10] getting the UVs unfolded and placed. When placing my UVs, I just wanted to ensure that
[3:16] I had consistent texel density between all of my UV shells. So I started by getting the
[3:21] torso fit into a zero to one space. Once I had that done, I was able to grab the level
[3:27] of texel density that the mesh had and start building all of my other tiles using that
[3:31] info. Using the texel density that I established, this allowed me to figure out how I wanted
[3:37] to pack each tile. From there, I set up each part of the model in different UV spaces so
[3:43] that I had a UDIM setup. Overall, the process for getting the UVs was pretty straightforward.
[3:57] Now, the next thing that I had to worry about was having my high poly geometry retain that
[4:01] crispness for the baking. So to help with that, what I did was I split my high poly model
[4:07] up so that it more or less matched what my UV seam placement had. From there, I would
[4:13] extend the geometry cap just a little bit further to ensure that I was able to capture
[4:18] all of the detail up to the seam. So for example, you can see here with the arms what that looks
[4:24] like. Once I had everything split up, I went through the process of decimating each part
[4:46] of the split mesh. Now, there are a couple of reasons that I work this way. One is because
[4:52] I want to ensure that each piece of the model has the crispness detail possible. The other
[4:57] is because this is going to allow me to export each individual piece of the model as a separate
[5:02] FBX file. This process will allow for the model to be split up into more pieces that
[5:08] will make it a little bit easier to load all of this information into memory once I start
[5:13] my baking process. If I was to have to keep this model as one entity, the final export
[5:19] would have been a lot heavier and harder for the computer to manage. Now, the next step


### Baking [5:24]
**Transcript (timestamped):**
[5:25] in the pipeline is going to be baking. And while baking is important, I've already covered
[5:29] this part of my workflow in some of my other videos, so make sure to go check that out
[5:33] if you're interested. That being said, I did want to mention a quick side note that when
[5:38] working with UDIMS, you do want to ensure that you have the use UV tile workflow enabled
[5:45] when you import your mesh. As long as you have that, your mesh should be loaded as you'd
[5:50] expect and your bakes should bake properly. When baking inside of Painter, I approach
[5:57] my settings the same way that I would with any of my other bakes in any other project.
[6:03] One thing that you may notice though is that there are a couple of bakes, like with the
[6:07] thickness map, that could potentially pose some differences between each part of the
[6:12] UDIMS seams. With that, I just went into Painter and manually fixed that to alleviate
[6:18] that issue if it did arise. Now, at this point in the process, I normally would do one of
[6:25] two things. I'd either start texturing my asset from this point and just continue forward
[6:31] in the pipeline, or I would head to my render engine and start to set up the scene so that
[6:36] this would allow for an iteration loop. Now, because with this project, I knew that I


### Setting up UE5 [6:39]
**Transcript (timestamped):**
[6:42] wanted to use UDIMS, I had to go forward and set up my project inside of UE5 just to ensure
[6:48] that my UDIMS were set up properly and working inside the engine. So to do that, the first
[6:54] thing that we're going to want to do is come over into UE5 and we're going to come up to
[6:58] our project settings. Once we have that open, we're going to search for virtual. Then when
[7:07] we come down here to our virtual texture setting, in here, we're going to enable these four
[7:13] switches. The main one that you do have to ensure that's checked is enable virtual texture
[7:19] support. Once you've turned these on, you will get a prompt to restart the engine. So restart
[7:25] that and you should now be able to use your virtual textures. Now, once we've got our


### Creating Material [7:30]
**Transcript (timestamped):**
[7:31] virtual textures enabled, the next thing that we're going to do is create a material. We're
[7:36] going to do this so that we can start to test out the UDIMS and just make sure that the material
[7:41] and the UDIMS are working properly. So the first thing I'm going to do to create this
[7:45] material is I'm going to right click and hit create new material. Once we have that, we're
[7:53] going to want to bring over our textures and start slotting in and checking our UDIMS. So
[7:58] back over in Painter, I'm going to export out all of my textures, which if we did set up
[8:03] Painter properly, everything should export with that tile support. Once those are exported,
[8:10] back inside and Unreal, we need to import our textures now. So the first thing that you
[8:16] should notice once you import your textures is this little VT in the right corner. This
[8:21] means that the textures are now loaded as virtual textures. So right here, now I'm just


### Testing [8:27]
**Transcript (timestamped):**
[8:30] in a process of testing. So the first thing that I want to do is I just want to import
[8:34] one texture set so that I can ensure that my texture sets are working and I can plug
[8:39] things in the material just to make sure that everything is working as intended. Once we
[8:44] have our texture set loaded in, the next thing we want to do is just drag and drop all of
[8:49] these in and start to slot them into the correct channel. Once we have this, we can see that
[9:05] we're getting the result on our model. The textures are a little bit jumbled on this
[9:10] part of the model because we aren't loading all of the textures in, but we are getting
[9:14] a result that we would expect. So from here to get things finished up, we're going to
[9:20] start importing in all of the rest of our textures. One thing that you'll notice is once you
[9:26] import all of your textures, you'll see here on the little texture icon that it looks like
[9:31] all of your texture images are squeezed into this small little box. That means that we
[9:36] are viewing this as our UDems. Now, if everything is loaded in properly, you should get a result
[9:43] similar to this where you have all of your textures propagated to the model the way that
[9:48] you would expect. So now you can see here that I've ultimately exported out multiple
[9:53] texture sets that all work on this model and it goes across all of the texture UV seams
[9:59] and we now have a result that we can really squeeze a lot of fidelity and texture resolution
[10:04] out of. So now after doing all of that, we have our model set up inside Unreal with the


### Outro [10:06]
**Transcript (timestamped):**
[10:11] ability to use UDems. The next part of the stage is going to be creating our final textures
[10:17] back inside Substance Painter. So in the next video, what we're going to do is we're going
[10:21] to move forward with our character working on creating and completing our textures. This
[10:26] model was a fun one to really experiment on. So if you're interested in seeing the final
[10:31] textures, make sure to subscribe so that you can see those next steps. Hopefully you found
[10:36] this useful and I'll see you guys in the next video.



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
