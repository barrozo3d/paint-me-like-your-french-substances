---
title: SUBSURFACE SCATTERING: Subsurface Scattering in SUBSTANCE PAINTER for UNREAL ENGINE 5
source: YouTube
url: https://www.youtube.com/watch?v=mjLiJ5yjto0
author: Jared Chavez
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/subsurface-scattering-subsurface-scattering-in-substance-painter-for-unreal-engi/
frame_count: 0
frame_status: pending-selection
---

# SUBSURFACE SCATTERING: Subsurface Scattering in SUBSTANCE PAINTER for UNREAL ENGINE 5

**Source:** [YouTube](https://www.youtube.com/watch?v=mjLiJ5yjto0)
**Author:** Jared Chavez
**Duration:** 8m22s | 17 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py subsurface-scattering-subsurface-scattering-in-substance-painter-for-unreal-engi <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hey, I'm Jared. In this video, we're going to look at making a subsurface scattering map for our Neomorph character.
[0:06] In our last video, we covered the texturing process for this character.
[0:10] But I left out the subsurface scattering portion because I felt like there was a little bit more need for some in-depth explanation as to why I painted the map the way that I did.


### Why Subsurface Scattering [0:21]
**Transcript (timestamped):**
[0:21] So with that said, let's just go ahead and dive right in.
[0:24] With this character, I knew that I really wanted to push the subsurface scattering effect that I was doing.
[0:30] I wanted to push it more towards that kind of deep sea creature feeling with translucent and see-through skin.
[0:38] I really liked the idea of having as much light transmitting through the body of the character.
[0:45] But one thing that you do run into with subsurface scattering is if you push too much subsurface,
[0:51] you can end up with a result that maybe feels like gelatin or like a candle or something like that.
[0:56] So I wanted to be a little bit more intentional with how I created my map in order to get an effect that looked good,
[1:02] but didn't just feel like something that was glowing with no type of internal anatomy.


### Thickness Map [1:08]
**Transcript (timestamped):**
[1:08] So the first thing that I start with whenever I'm doing my subsurface map is going to be my thickness map that I baked out.
[1:14] With this piece, you'll notice that there's a little bit of errors down at the feet where the thickness didn't quite calculate properly.
[1:20] So I just had to manually fix that.
[1:22] I didn't put a lot of time and effort into trying to solve the issue inside of Painter, and I just kind of manually fixed it on the go.


### Secondary Subsurface Layers [1:29]
**Transcript (timestamped):**
[1:30] With my baked map in place, the first thing that I want to start by doing is creating some secondary subsurface layers that are set to black.
[1:38] In this layer, I'm going to start painting on all of the bony landmarks along the model that I don't want any of that light to penetrate through.
[1:46] So I'm thinking about areas where bone is really close to the surface.


### Bone Landmarks [1:51]
**Transcript (timestamped):**
[1:52] With doing the subsurface map for this character, I wanted to kind of start to test things out pretty quickly to make sure that I was getting a result that I liked.
[2:00] So I just did a quick little paint job on the rib cage, and you can see that I'm starting to get a pretty pleasing result.
[2:06] I feel like there's some interest.
[2:08] You can kind of differentiate between the bone and the skin, and you're getting some of that light starting to pass through that we're looking for.


### Blur [2:15]
**Transcript (timestamped):**
[2:16] On this layer, I also apply a blur on top of everything just to kind of soften out and smooth out some of this information.
[2:23] So I'm not creating a harsh transition from subsurface scattering to non-subsurface scattering.
[2:29] It's just going to alleviate my results a little bit and make sure that I'm not dealing with any kind of weird artifacting occurring from that harsh transition between on and off.


### Baked Maps [2:40]
**Transcript (timestamped):**
[2:40] So by using the baked maps, I was able to use this as somewhat of a starting point.
[2:45] I was able to export this over to Unreal and kind of gauge how the material was responding inside of the engine so that I could really start to diagnose and base my textures off of the information that the engine was providing.
[2:58] So it was ultimately just kind of a good starting point so that I could move forward from.


### Bone [3:02]
**Transcript (timestamped):**
[3:03] After seeing what was going on inside of my render, then came the intention to try and push sort of that feeling of bone underneath the skin.
[3:12] So there wasn't light going through specific areas, and it made it feel like there was a little bit more organic matter inside of the model, and there was a lot more life to it.
[3:22] Now, I will say that I kind of ran into a little bit of luck when it came to setting up the shader.
[3:28] When setting up the shader, I was really able to kind of push the subsurface scattering to a pretty far extent and kind of create a lot of light separation that was happening to make it feel like there was more going on inside the body than actually was.
[3:45] Now, one thing that I wanted to mention when creating subsurface scattering for characters that I like to keep in mind is I usually like to determine where light is going to penetrate through the most.
[3:56] For this character, I wanted it to be the top part of the skull.
[3:59] So that is going to be the part that I'm going to color 100% white.
[4:03] That's going to be where I'm getting the most subsurface scattering.
[4:06] Everything outside of that might be a variation of black or gray, but the top part where I want the most subsurface scattering to happen is going to be the pure white and then everything else is going to kind of trickle down from that.


### Top Layer [4:20]
**Transcript (timestamped):**
[4:20] So that's going to be the next layer that I'm going to paint, and it's going to be completely white on this top part of the head.
[4:26] I'm going to make this the most prominent area where the scattering is happening.
[4:30] And you'll see here inside of the engine, you can see the light scattering through more than it is on the rest of the model.
[4:36] And now from here, I can start to gauge how the other parts are starting to work now that I know my top values and I know my bottom values.


### Arms and Legs [4:45]
**Transcript (timestamped):**
[4:45] Now, the next thing I decided to move on to was going to be the arms and the legs as well as the tail.
[4:50] With these areas, I didn't quite want as much light scattering through.
[4:54] I wanted it to feel like there was a little bit more bone than flesh in these areas.
[4:59] So you'll notice that I'm using a little bit of a darker value, not 100% black, but enough that there is just some light starting to penetrate through, but not a ton.


### Second Pass [5:10]
**Transcript (timestamped):**
[5:10] After making my first initial pass on things, I start to take a second pass and here I further refine the map a little bit more.
[5:17] I start to introduce things like tendons or areas that I may feel like wouldn't be receiving quite as much light showing through.
[5:25] And this is going to introduce a little bit more variation and nuance to this map.


### Custom Layers [5:30]
**Transcript (timestamped):**
[5:30] After getting my base painted, I start to add things like the curvature map on top of my model so that I can control some of the areas where scattering is happening in the details.
[5:40] This is going to give me a little bit more control to make things pop.
[5:44] I also start to add custom layers on things for things like the flake and damaged skin that I have.
[5:50] I want to retain that information and I don't want it to feel quite as thin in subsurface scattering.
[5:55] I want to have a little bit more control over it so that I can influence how that looks in the final result.
[6:01] During this process, I also played with the idea of maybe making the stomach feel like there was something going on inside it.


### Stomach [6:02]
**Transcript (timestamped):**
[6:08] This was just done by adding a little bit of extra black to the center of the belly to make it feel like there wasn't a ton of subsurface going on there.
[6:17] So it kind of created this illusion that there was some kind of mass behind it that was preventing the light from scattering through.
[6:24] I did this in a couple of different areas across the body.


### Body [6:25]
**Transcript (timestamped):**
[6:27] Again, this isn't going to be 100% physically accurate because there's not really anything inside of the model to prevent the light from scattering through.
[6:35] I can't necessarily fake that, but I feel like it was able to get the point across and create this nice illusion that there were things going on and it really held up from different angles.
[6:47] Now, the last and final stage, which I like to do during this process is going to be dialing in my subsurface scattering profile.


### Final Stage [6:48]
**Transcript (timestamped):**
[6:54] For this character, I knew that I really wanted to push how much scattering was happening and I feel like after authoring the map, it really gave me that control to do it.
[7:04] You can see here in the final renders, things like the head have a lot of light that's scattering through and it feels like there's some kind of a bone structure in the model, but it also still has that fleshy feel.


### Final Render [7:05]
**Transcript (timestamped):**
[7:17] You can also see areas like the ribs and the tail that it feels like there's a bone inside of that model that's preventing the light from coming through, but you have thin areas of skin where you can see that light starting to glow and create that look of sort of thin skin.
[7:33] Overall, with this piece, I was surprised that I was actually able to get the final result that I did. I was pretty happy with it and I felt like it kind of hit the bars that I wanted to.
[7:44] I wasn't sure if I was going to be able to pull it off for this character, but after a lot of back and forth and kind of iterating and refining and finding my limits with what the shader can offer, I was able to take that knowledge and kind of harness it in the direction so that I could use the shader to benefit me and produce the look that I was happy with.


### Outro [8:03]
**Transcript (timestamped):**
[8:03] So with that, hopefully you guys found this stuff interesting and informative. Let me know what you guys think down in the comments. The next stage for this character is going to be setting up some lights inside of Unreal.
[8:13] So if you're interested in that, make sure to follow so you can keep up with the process. Thanks for watching and I'll see you guys in the next one. Okay, bye.



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
