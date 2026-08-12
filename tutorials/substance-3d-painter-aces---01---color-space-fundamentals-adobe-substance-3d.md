---
title: Substance 3D Painter & ACES - 01 - Color Space Fundamentals | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=hDiYqODGoHg
author: Adobe Substance 3D
ingested: 2026-08-12
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/substance-3d-painter-aces---01---color-space-fundamentals-adobe-substance-3d/
frame_count: 0
frame_status: pending-selection
---

# Substance 3D Painter & ACES - 01 - Color Space Fundamentals | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=hDiYqODGoHg)
**Author:** Adobe Substance 3D
**Duration:** 7m4s | 9 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py substance-3d-painter-aces---01---color-space-fundamentals-adobe-substance-3d <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hello, my name is Michael Wilde and I'm here to talk to you today about Substance Painter
[0:08] and its use of ASUS CG with OCIO. I've been a VFX artist for nearly 10 years now, modelling
[0:14] and texturing on a number of films and currently work as a senior texture artist at ILM London.
[0:19] I also make YouTube tutorials covering all sorts of 3D topics like this series here.
[0:24] Dealing with Colour Space and ASUS Workflows are a vital part of being a VFX artist for
[0:27] film and TV. So in this 3 part series I'm going to explain what colour spaces are and
[0:32] why they're so important, how Substance Painter handles ASUS CG with its implementation of
[0:36] OCIO, and finally how to fit Substance Painter into your ASUS CG pipeline at home. So let's
[0:42] get into it.
[0:43] First, I want to stress that colour management is a complex topic. We can't cover everything
[0:48] in a 5 minute video but it's really important to have at least a base level understanding
[0:52] since colour space issues pop up a lot. So if you find yourself wanting something more


### What is a colour space? [0:57]
**Transcript (timestamped):**
[0:57] in depth than these videos get, I've provided some really fantastic resources in the video
[1:00] description.
[1:01] We'll be diving into Substance Painter in part 2 but before we get there it's best
[1:05] to break down a bit of terminology so you're comfortable when you get to texturing. So
[1:09] what is a colour space? In its broadest term, a colour space is a range of colours which
[1:14] we can map out and define. The way we define them is on this overly sci-fi sounding CIE
[1:19] Chromaticity diagram. You may have seen one of these before. This graph shows all the
[1:24] chromaticities that are visible to the human eye. Chromaticities are slightly different
[1:28] to colours but for the sake of this beginner's video I'm going to simplify it and refer
[1:32] to them as colours going forward.
[1:34] So how do we define a colour space on this graph? Well, a colour space needs its primary
[1:38] colours. With VFX, due to the nature of how screens create light and colour with red, green
[1:43] and blue lights, we use RGB primaries, unlike say printing which uses CMYK. This is referred
[1:50] to as our colour model. We can plot the primaries down and draw lines between them which produces
[1:55] a triangle enclosing every colour that can be represented within our colour space. This


### sRGB [1:59]
**Transcript (timestamped):**
[2:00] triangle is referred to as a colour gamut. One colour space that you may have already
[2:04] heard of is S-RGB and that's not to be confused with the very closely named RGB, the colour
[2:09] model which we were just speaking about. So S-RGB stands for standard red, green, blue
[2:14] and it's actually the gamut that I just drew on the CIE graph. S-RGB is the colour space
[2:20] most online images are encoded with and it's how most monitors display images too. It's
[2:25] not a linear colour space and to explain what that important term means we're going to have


### Gamma Curves & Transfer Functions [2:26]
**Transcript (timestamped):**
[2:29] to get a little tangential.
[2:32] The way human eyes perceive values of light is not equal. If you were to look into an intense
[2:37] light like a bright sky it's very difficult to pick out differences in values in the clouds
[2:41] or the sun. It all just looks super bright. But if you sit in a dark room it's really
[2:46] easy to pick out small differences in value due to the way our vision works. We can perceive
[2:51] much more variation in lower light than we can in bright light. If you wanted to you
[2:55] could plot that onto a graph and it may look something like this.
[2:59] Since computer monitors are just lots of little lights our eyes perceive them in the same way.
[3:04] S-RGB images take advantage of this and they give more space to darker values which our
[3:09] eyes are more likely to perceive. This is often referred to as the gamma curve or the
[3:13] colour space transfer function. An S-RGB has a gamma curve of 2.2 which we can plot onto
[3:19] a graph.
[3:21] If we go to a brightness value of 50% it's actually only a pixel value of about 20%. That's
[3:28] why we call S-RGB non-linear. If we do want our pixel values to be equal to their brightness
[3:34] we would need the image to handle data in a straight line like this. But more on that later.


### ACES [3:37]
**Transcript (timestamped):**
[3:41] S-RGB sounds great but what about this ASUS that I keep hearing so much about?
[3:45] Well ASUS is a colour management system created by the academy. Yes, that academy. To standardise
[3:51] the colour pipeline for film and TV since filmmakers went digital. Since film can be shot
[3:56] with a variety of different cameras these days all which may see colours slightly differently
[4:01] ASUS helps to unify the data from multiple sources and also make sure footage can be


### ACEScg [4:03]
**Transcript (timestamped):**
[4:06] archived well for future use. ASUS itself isn't a colour space. It's a colour management system
[4:12] but one component of that management is the all too similarly named ASUS CG colour space.
[4:18] The ASUS workflow using ASUS CG has quickly become the standard way to texture and render your 3D
[4:24] assets in VFX and if you're working in a VFX studio applying to one or studying at university
[4:29] it's something you need to be comfortable with. There are other ASUS colour spaces but for VFX


### Why ACES? [4:34]
**Transcript (timestamped):**
[4:34] texturing ASUS CG is the only one we concern ourselves with. Before I overload your brain
[4:40] let's wrap this video up by explaining what makes ASUS CG so good for VFX and why it matters in
[4:44] Substance Painter. If we hop back to our CIE graph and plot our ASUS CG on there we can see how large
[4:51] the range or gamut of colours that it encompasses is. It's almost the whole visible spectrum unlike
[4:57] sRGB. Such a wide gamut helps unify all resources that we may use in VFX so they all play nicely
[5:04] together. On a single asset you may be using compressed jpegs from the internet, on-set raw
[5:09] high bit depth photographs of an actor, and black and white substance procedurals so we want our


### Linear colour spaces [5:14]
**Transcript (timestamped):**
[5:14] pipeline to be able to hold them all and make them all look correct. Also unlike sRGB ASUS CG is a
[5:20] linear colour space. What does that mean and why is it important? Well if I were to plot it alongside
[5:26] the gamma curve of sRGB we can see that its values are equal to its intensity. Basic maths teaches us
[5:33] that if we add 50% and 50% together we should have 100% but if I double the pixel value that we have
[5:41] 50% along these two transfer functions only the linear one gives the visually correct result of
[5:46] 100%. Doing mathematical calculations with non-linear images would give us incorrect results.
[5:53] 3D packages are doing really complex maths behind the scenes with our textures
[5:57] so working in linear is incredibly important for them to calculate and render everything
[6:01] as it should look. All of this matters in Substance Painter for one really simple and
[6:06] important reason. We want what we see in our Substance Viewport to be what we see at render
[6:11] time in other programs which we're going to cover in the next two parts of this video series.


### Recap [6:12]
**Transcript (timestamped):**
[6:15] I've thrown a lot at you here so before we go let's quickly summarize everything we've covered.
[6:20] Colour space is a definable groups of colours which we can plot onto a graph.
[6:24] Two important characteristics of them are their range of colours, the gamma,
[6:28] and how we perceive their brightness, the transfer function. You may already be familiar with the sRGB
[6:33] colour space used on images on the internet. Its transfer function is non-linear meaning it doesn't
[6:38] allocate the same amount of data across the brightness of its pixels, it's often referred to as a gamma
[6:43] 2.2 curve. The ASUS colour management system was created to unify the digital film pipeline
[6:49] and for VFX we use the ASUS CG colour space which is part of it. It has a linear transfer function.
[6:56] So join me in part two to see how we use OCIO to work with ASUS inside a Substance Painter.



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
