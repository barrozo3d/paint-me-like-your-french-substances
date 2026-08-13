---
title: Advanced Peeling Paint Effect in Substance 3D Painter
source: YouTube
url: https://www.youtube.com/watch?v=VE8aILV053Y
author: Javad Rajabzade
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/advanced-peeling-paint-effect-in-substance-3d-painter/
frame_count: 0
frame_status: pending-selection
---

# Advanced Peeling Paint Effect in Substance 3D Painter

**Source:** [YouTube](https://www.youtube.com/watch?v=VE8aILV053Y)
**Author:** Javad Rajabzade
**Duration:** 11m27s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py advanced-peeling-paint-effect-in-substance-3d-painter <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hello everyone, this is Javad and today I'm going to show you how to create a peeling
[0:12] paint effect in Substance Painter.
[0:15] As you can see I'm already imported my model and baked the textures, so the model is ready
[0:22] to go.
[0:23] And let's get started.
[0:27] So in games and 3D props we usually deal with the three main types of paint damage,
[0:32] HVIR, peeling or police streaming, paint and cracking.
[0:37] HVIR is what you normally see on things like weapons or tools where the paint naturally
[0:44] drops around the edges.
[0:46] But in this video I want to focus more on the peeling paint and show you how to make
[0:51] a more advanced version of it in Substance Painter.
[0:56] If you're interested in learning more about all these types of paint damage, I actually
[1:01] wrote an article that explains each one in detail.
[1:06] You can check it out and download it from my Patreon.
[1:11] It will help you figure out which type of paint damage fits the best for your assets.
[1:20] Alright let's start by creating a new fill layer and adding a black mask.
[1:26] Next I'll apply a generator to control where the paint starts to peel off.
[1:32] Now depending on the look you want you can use different generators, for example the
[1:36] edge damage mask, builder or even curvature mask.
[1:39] Each of them gives you a slightly different result.
[1:43] So it really depends on your material and what kind of VIR effect you are going for.
[1:48] Here I'm using the Metal HVIR generator, I don't want any extra grunge in this case
[1:52] so I reduce the grunge amount and then increase both the VIR level and the contrast to make
[1:57] the effect a bit sharper.
[1:59] Okay now I'm going to add a blur filter and slightly increase its value.
[2:07] Then I'll change the blending mode to Lighten.
[2:12] What the Lighten mode does it keeps the maximum color value between the top and the bottom
[2:17] layer.
[2:18] In this case it means we are keeping our sharp edge VIR mask while blending the blur mask
[2:26] on top of it.
[2:27] We'll start with two values here.
[2:32] The first value is the sharp, completely white mask.
[2:36] This means that the paint will be fully removed in that area and we won't see any paint there
[2:42] at all.
[2:44] In other words that sharp white mask completely erase the paint.
[2:48] On the other hand the blurred mask or the softer edge will add a more gradual grunge
[2:54] effect creating a natural worn look.
[2:57] For adding edge damage I usually use a cell texture however in this case I'm using a 3D
[3:03] Perun effectal that gives me more control over the parameter.
[3:08] Also since we are working with UDIM we need to adjust the projection to feel.
[3:15] Next we'll adjust the 3D Perun effectal parameter until we achieve the desired look.
[3:26] After that we'll change the blending mode to Divide.
[3:31] The result you'll notice the effect primarily appears under softer blurry edges while the
[3:39] sharp white mask remain unchanged.
[3:42] Then I'm using a level to invert the mask.
[3:45] Next we'll add a histogram shift.
[3:48] What this does is shift any black values in the mask to white without altering other values.
[3:57] After that histogram shift we'll add another level and invert the mask to finalize it while
[4:04] we could use an invert filter.
[4:09] Invert filter actually doesn't offer as much control over the mask values by using the
[4:17] level we can fine tune the edges and get more precise results.
[4:22] The height value to bring out the age damage.
[4:25] This increase our height value to bring out the age damage effect.
[4:30] As you can see everything looks good and the age detail are no visible.
[4:35] The next step is to create our paint mask.
[4:37] To do that we'll add an anchor point between the level and the histogram shift.
[4:42] This will give us a mask that we can later on use to mask our paint layer.
[4:50] Now I'm going to add another layer.
[4:54] Place it inside the group.
[4:56] Let's rename this layer to paint layer.
[5:01] I pick a color and adjust roughness.
[5:10] Inside the group I'll add a black mask for paint layer.
[5:16] I'll reference it using the anchor point and apply a level adjustment.
[5:25] By tweaking the level we can control how and where the paint becomes visible.
[5:31] Now we can go back and use the belayer filter to either enhance or soften that age damage
[5:38] effect.
[5:39] Letting it gradually grow and blend more naturally.
[5:44] The cool thing about this setup is that by tweaking the parameters you can achieve a
[5:49] completely new look and effect on your material.
[5:52] As you can see I already inverted this 3D VOR effectal noise.
[6:00] That gives me this beautiful blistering effect.
[6:04] But the effect looks a bit too perfect to be realistic.
[6:09] So what I'm going to do is add a belayer filter on top of my layers.
[6:16] This is gonna be a solid effect but it gives a sort of erosion to this blistering effect
[6:23] and making the blistering look more natural and realistic.
[6:31] Let's duplicate our belayer filter using CTRL T and place it below the histogram shift.
[6:37] And by tweaking the parameter we can achieve more variation and enhance the overall effect.
[6:48] It actually doesn't look very natural when the paint damage shows up all over the entire
[6:52] model.
[6:53] In real life this kind of wear only happens in certain spots.
[6:58] So we need a way to control where it appears.
[7:02] So here is a cool trick.
[7:04] Add a paint layer and place it under the generator.
[7:09] Then switch the generator blending mode to multiple light.
[7:13] And now the magic happens.
[7:15] Whenever we paint on that layer, paint layer, it only reveals the edge wear effect exactly
[7:22] where we want.
[7:32] Okay, so here I'm adding another paint layer right above the metal edge wear generator.
[7:50] If I paint in black it will add the peeling paint effect to those areas.
[7:56] You can also press X to invert the mask.
[7:59] So painting in white will remove the effect from the spots that are already peeling.
[8:07] Okay here I want to add more details to my edge paint.
[8:10] So I'm creating an anchor point on top of my mask layer.
[8:16] Okay let's name it edge paint.
[8:19] And then I'll make a new layer with a black mask.
[8:27] And okay add a fill layer.
[8:32] And inside that fill layer I reference the anchor point.
[8:37] As you can see the mask shows up automatically because it's pulling the information from
[8:42] that anchor point.
[8:46] In a real world scenario the color on the edge of peeling paint usually fades a bit.
[8:52] So here I'm picking a slightly brighter color and setting blending mode to soft light.
[9:03] Okay let's duplicate this 2DVoronai fractal.
[9:09] And this time I'm switching to the regular 2DVoronai.
[9:12] I'm just going to grab the cell tiles preset and as you can see it gives me the sharp,
[9:19] cracking effect on the edges of my peeling paint.
[9:23] It's nice ways to break up the surface and make those edges feel more detailed.
[9:29] This kind of sharp cracking usually happens when the paint surface is constantly exposed
[9:34] to the sun.
[9:36] So if you are texturing a prop for an environment like a desert turn or somewhere with a really
[9:41] harsh sunlight, this type of cracking makes a lot of sense.
[9:46] It helps sell that dry sun beaten look.
[9:50] Before I even start texturing I always try to understand the story behind the asset.
[9:55] Like where is this thing actually sitting?
[9:58] What kind of place is it in?
[10:01] Has it been there for a few months or for decades?
[10:05] All those legal details actually decide how the surface should look.
[10:11] So it was thinking about them first.
[10:13] So for example if the asset is in a humid area, the type of damage you expect is totally
[10:19] different.
[10:20] In humidity you usually get moss slowly growing from the bottom up wart.
[10:25] And instead of this sharp cracking effect you'd probably go for a blistering effect
[10:32] because the humid environment traps moisture underneath the paint.
[10:37] But that trap butter pushes the paint out fart and creates those bubbles.
[10:43] So always think about the environment first.
[10:46] It makes your texture way more believable.
[10:48] To keep things organized I will place my mass layer inside this folder.
[10:52] My goal is to create a folder that contains my paint layer and any details I want to add
[10:58] will be created inside this folder.
[11:00] Anything placed underneath this folder will then be revealed as the underlying material.
[11:06] Then I'm going to drag and drop a metal rust material underneath my paint folder.
[11:11] As you'll notice here the height of the rust material is affecting the paint layer.
[11:15] So to fix that you're first going to change the channel from roughness to height and
[11:19] then we'll switch the blending mode from linear to normal.



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
