---
title: Creating Fabric stitches for Footwear with Anchor Points in Substance 3D Painter | Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=dIO6cJiE7JM
author: Adobe Substance 3D
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/creating-fabric-stitches-for-footwear-with-anchor-points-in-substance-3d-painter/
frame_count: 0
frame_status: pending-selection
---

# Creating Fabric stitches for Footwear with Anchor Points in Substance 3D Painter | Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=dIO6cJiE7JM)
**Author:** Adobe Substance 3D
**Duration:** 8m31s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py creating-fabric-stitches-for-footwear-with-anchor-points-in-substance-3d-painter <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Welcome to this multi-part tutorial series where we will go over some more advanced techniques
[0:13] on how to use anchor points in your projects.
[0:16] This series is a follow up of our basic anchor point series which you can also find on this
[0:21] channel.
[0:22] In this first video we will go over on how to create this really nice stitch effect that
[0:27] you can use on any type of fabric.
[0:30] This will include creating the actual stitches using a built in stitch brush along with these
[0:35] really nice dents that you often see that come along with the stitches.
[0:39] So that will be it for this chapter and let's dive right in.
[0:42] So what are anchor points?
[0:45] Anchor points are a powerful feature that let you reuse a part of your layer stack.
[0:50] This means that you can define a mask or layer once and reference it dynamically in other
[0:56] layers.
[0:58] If you change the anchor point, all references are updated as well, letting you work smarter
[1:03] and faster.
[1:04] Okay, so we have this really nice model over here that we are going to use for our example.
[1:10] So the first thing that we want to do is we want to go ahead and create a simple layer.
[1:15] The reason for this is because we are going to use a special brush that has built in settings
[1:20] for our stitches.
[1:22] So what you want to do is in your assets, simply go to brushes and type in stitch over
[1:27] here and then we have this one.
[1:30] If you double click on it, it will activate and then if you go into your properties, you
[1:35] will see a bunch of different settings here.
[1:37] And you can already see that if I would drag this around here, see, you can see that these
[1:42] are the typical stitches that you often see.
[1:45] Now what I'm going to do is first of all, I'm going to go ahead and just remove the
[1:50] seam in between so that we only have these stitches like this and not that thin line
[1:54] in between.
[1:56] Next to that, I feel they are maybe a little bit small, so you can always just go up here
[2:02] and set the size a little bit bigger or of course you can do it up here or you can right
[2:06] click and do it up here.
[2:07] So many ways to do that.
[2:09] I also often like to just click and hold shift because then I can often create nice straight
[2:15] lines like this.
[2:17] So let's see, this is looking pretty good.
[2:19] Yeah, I quite like this.
[2:22] So let's use this one as a base and then start by building the rest of our structure.
[2:27] First of all, let's go ahead and just call this stitch underscore base.
[2:32] And then what you want to do is you want to go ahead and go up here and add an anchor
[2:36] point.
[2:37] So this is the whole goal of this tutorial with this anchor point, we can still reference
[2:41] the shape and we can manipulate it using fill layers and a bunch of other stuff.
[2:46] And that's what we're going to do now.
[2:47] We are first going to go ahead and give it some interesting denting around the stitches
[2:52] as if it has been pushed inside of the fabric.
[2:56] The way that you can do that is go ahead and add a fill layer and let's just call this
[3:01] the form for example.
[3:03] And honestly, we only really need our height map for this.
[3:07] So just go ahead and turn everything off except for height map and then set the height map
[3:11] into the minus.
[3:12] I don't yet know how much, but we will see that soon enough.
[3:17] Now what we want to do is we want to go ahead and go up here to our masks and create a black
[3:22] mask.
[3:24] Once we've done that, we can start by referencing our stitches over here and we can extract
[3:28] the mask from it.
[3:30] The way that you do that is simply go up here, add a fill and then if you click on your grayscale
[3:36] you can see your anchor points up here, which will have our stitch base.
[3:42] So we basically grab it.
[3:44] Now one thing we need to do is in the alpha behavior, we want to extract specifically
[3:48] the alpha which will be the stitches.
[3:51] And as you can see here, you can see that that gives quite a big impact.
[3:55] Honestly for the rest we don't really need to do much.
[3:57] If you want, you can always play around with your levels to make it stronger or less strong.
[4:02] But what we are going to do is we are going to blur it.
[4:05] Because if you blur it, this will just give us like a nice transition.
[4:08] However, I'm going to use a slightly special technique because if we are just blurring
[4:13] this once, here let's art a filter and art a blur, you can see that the transition is
[4:21] never so nice.
[4:23] It's a bit difficult to see maybe for you, but I can see like a very clear blur look
[4:28] and I don't really like that.
[4:30] But a cool tip that you can do is if you go ahead and set this blur a little bit stronger
[4:35] to maybe like 0.6 and if we then go ahead and art another blur, so art another filter
[4:43] with a blur like this and this one to 0.5, you can see that the transition becomes a
[4:47] little bit nicer.
[4:49] And then at this point all we need to do is just play around with our height to get like
[4:53] a stronger or less strong transition as you can see.
[4:56] I'm going to go for probably like minus 0.3 seems about fine.
[5:03] Well, actually let's do minus 0.4.
[5:06] There we go.
[5:08] Now, something that we can also do is we can also give it some color.
[5:11] This is once again very easy.
[5:13] All we need to do is just add a new fill layer over here.
[5:16] Let's call this color and let's only art like a color and some roughness.
[5:22] So far roughness maybe like set it down a little bit just to make it a little bit duller.
[5:27] And for your color, you can just go ahead and grab whatever you want.
[5:30] Let me just use red for now just because it's a very clear color.
[5:34] Then all you want to do is we want to once again mask our stitches using an anchor point.
[5:39] We can do this by adding a black mask along with a fill.
[5:43] And once again in this fill, we just want to go ahead and we want to grab our stitch base.
[5:49] Now don't forget to set the alpha behavior to extract alpha because else once again it will just give us like a gradient look
[5:56] or a gray scale look.
[5:58] And now I'm just going to use my black levels to basically push my color back a little bit because it was bleeding out a little bit.
[6:05] And I don't really like that.
[6:07] So just give it like a nice balance.
[6:09] And there you go.
[6:11] So at this point you will be ready to start by just going in and painting everything.
[6:15] Now one cool trick that you can do.
[6:17] So right now if we go back and we would paint this, for example, let's say that I do like this.
[6:23] Then it is quite annoying because we have over here our laces that are sitting in the way.
[6:28] What you can do is you can always go down here and you can basically turn off specific models.
[6:35] So we can click off the laces like this on these bits.
[6:41] And now if I would go ahead and I would paint here, you can see that they are gray scale to get out of this mode.
[6:46] Simply click on your layer again.
[6:48] So now if you would paint, it would simply ignore this specific model.
[6:52] See, so what I will do is I will just go ahead and start by painting these specific stitches over here.
[6:57] And then we will go ahead and continue.
[7:00] Okay, so here we go.
[7:01] I just went ahead and quickly paint in some stitches just to show you the power of it.
[7:05] And now what I want to show you is that we can, thanks to anchor points, also use different brushes within this layer.
[7:12] And it will all simply be deformed the same way.
[7:16] So what we can do, for example, is let's say that we create like some sort of a seam line.
[7:20] If we go ahead and grab our basic heart brush over here and just double click on it and let's set the size a little bit smaller, maybe something like this.
[7:29] And don't forget right now your stitches are still over here assigned.
[7:34] So you just want to go ahead and scroll down and just press the X button on this material.
[7:39] Now what you can see is if we just paint in a simple white line, let's say over here, you get this seam line.
[7:47] And you can basically go ahead and just have like the same deformation on this.
[7:51] So this is quite nice.
[7:53] Now what I would recommend is of course, play around a bit with the size.
[7:56] If you do stuff like this, let's go like a little bit smaller.
[7:59] And then you can see that one.
[8:01] And let's say that I want to also place another one, let's say from like here to, for example, over here.
[8:09] And then my stint my laces are a little bit in a way.
[8:12] So I might need to just quickly go in and do this.
[8:15] But there we go.
[8:16] So that's why you can also just create like some interesting looking seams and stuff like that.
[8:21] And that was about it for this tutorial.
[8:23] I hope that you find it useful and I hope to see you next time.



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
