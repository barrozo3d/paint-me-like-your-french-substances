---
title: HOW to Make a Peeled Paint Effect with ANCHOR Points | SUBSTANCE PAINTER
source: YouTube
url: https://www.youtube.com/watch?v=mLsXRzm7K0c
author: Jared Chavez
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not specified"
tags: [layers, fill-layer, paint-layer, masks, anchor-point, blend-mode, height, generator, procedural, particle-brush, intermediate, advanced]
extraction_status: complete
frames_dir: tutorials/frames/how-to-make-a-peeled-paint-effect-with-anchor-points-substance-painter/
frame_count: 11
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# HOW to Make a Peeled Paint Effect with ANCHOR Points | SUBSTANCE PAINTER

**Source:** [YouTube](https://www.youtube.com/watch?v=mLsXRzm7K0c)
**Author:** Jared Chavez
**Duration:** 12m30s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] So in today's episode, we're gonna go ahead and continue where we left off with talking about anchor points, and in this week, I'm gonna go ahead and show you guys how to actually make something like this.
[0:09] So, what I'm, we're kinda going after here is gonna be a, a sort of lifted edge, flaky sort of paint look to our textures, so that what we're gonna be able to do is we're gonna be able to just paint directly on the model and have this kind of effect follow wherever our paint is.
[0:25] So, we can see here, this is kinda what's going on, we should just be able to paint directly.
[0:30] So, we're gonna recreate this look real quick.
[0:32] So, the first thing that we're gonna do is start off with a layer.
[0:36] So, we'll turn this off, and we're going to make this metal.
[0:40] So, we'll turn that off, we'll go here to give ourself a sort of metal look.
[0:46] We'll do really, really shiny.
[0:48] That should be fine.
[0:50] Then, if we come here, add a black mask.
[0:53] The first thing that we're gonna do is we're gonna add a paint layer.
[0:57] So, this paint layer is gonna be where we're painting our information on.
[1:00] Everything from here is gonna be referenced and used down the line.
[1:05] So, what we'll do is we'll just kinda come in here and start to paint.
[1:09] What you might notice right off the bat, there is like a little bit of the whitening between the blending of the paint to the metal.
[1:16] That's normal, but we might not want that.
[1:19] So, what we're gonna do is we're actually gonna look at our mask.
[1:22] You can see there's a lot of gradation going on where this is applied.
[1:26] We will apply a levels, and we are going to clamp down this shape, so that it's a little bit more harsh.
[1:35] It's a little bit more where we are applying this effect.
[1:38] It's gonna only be in that area.
[1:41] We don't really want much of that transition between the two areas.
[1:44] So, now at this point, we have something that feels pretty good.
[1:48] It might be a little bit noisy on the edge, so I'm going to add a filter and pause.
[1:56] So, my editing team, I'm my editing team, I'm looking at the analytics here, told me that 56% of you guys don't subscribe to the channel.
[2:04] That's a lot. That's more than 50%. That's 6% more than 50%.
[2:08] Not only are 56% of you not subscribed, there's also only 9% of you that have the notifications turned on.
[2:14] So, if you wanna see all of my content, make sure to hit that bell to turn that on as well.
[2:18] So, if you guys could go ahead and do me a favor, make sure to subscribe to the channel so that you can watch more cool content about 3D character art.
[2:25] And if you did it, well, thanks.
[2:27] If you haven't yet, go click the button.
[2:29] Now, back to what we were talking about.
[2:32] We will blur that a little bit, so we'll do maybe like 2.25, something like this.
[2:38] This should be good to start with.
[2:41] We'll add another levels on top of here, and then we're just gonna clamp down that shape again one more time,
[2:47] so that we kind of have a regularity on the edges, but it's a little bit smoother.
[2:51] It's not as noisy and irregular on the edges.
[2:56] So, this is gonna be our starting point.
[2:58] This is gonna be our base mask that we're gonna be able to work with.
[3:02] Now, in order to get this to work, we want to put an anchor point on top of this.
[3:08] We're gonna call this our metal paint anchor.
[3:14] So, now, anytime we reference this, we're gonna be able to find it in the future.
[3:18] So, that's what we're gonna do on this next layer.
[3:20] We'll come up here.
[3:22] We're going to add a new layer.
[3:24] We're going to do a black mask.
[3:28] We will add a fill layer to fill in our anchor point.
[3:31] So, we'll come down here and do metal paint anchor.
[3:34] You can see that highlighted in the stack on the right-hand side.
[3:38] We'll click that, and right off the bat, looks like nothing happened.
[3:41] How can we change that?
[3:42] Well, we can come here and see that it's essentially working, which is good.
[3:46] So, what I'm gonna do is I'm actually going to turn this off for right now,
[3:50] and I'm going to turn height on.
[3:53] So, we can kind of illustrate this.
[3:54] We can see there's actual height and displacement happening,
[3:57] which is good just to kind of visualize what we're after here, right?
[4:01] So, on first glance, this doesn't look good.
[4:04] So, what we're actually gonna do is we're going to build that flaking
[4:09] that's happening on the outside.
[4:11] So, let's see if we can go ahead and work through that real quick.
[4:13] First, we'll start by adding a blur on top of this.
[4:18] So, you can see that this is now what our mask is gonna look like.
[4:22] It's gonna blur, it's gonna kind of bleed outside on the edges a little bit.
[4:25] So, I'm gonna adjust that so that there's a little bit more of a falloff.
[4:30] You can see we're kind of starting to see a little bit of that ramp going on.
[4:34] So, there's two things that I can do.
[4:36] I can take this as a starting point or I could blur a little bit more,
[4:41] which is probably what I'm gonna do just to give us a little bit more clearance.
[4:46] And in order to do that, I'm going to push out on my levels
[4:51] so that now the falloff is further out.
[4:54] You can see we're essentially growing our mask a little bit more.
[4:58] So, you can see there is some of this kind of like faceting and artifacting happening
[5:02] just because we're kind of pushing this blur map to the extreme,
[5:06] but that's not gonna matter.
[5:08] So, now you can see we've essentially grown the outside edge of where we paint.
[5:13] So, if we come down here and start to paint some more,
[5:16] we have that like bubbled up lip effect.
[5:19] Now, the problem is we want to get rid of everything on the inside
[5:24] from affecting that like height being applied to the material.
[5:28] So, how do we do that?
[5:30] Well, the powerful thing about the anchor points is we can reference them
[5:34] on top of themselves and we can use blending modes in order to remove information.
[5:39] So, what I'll do is I will add another fill layer.
[5:41] You can see that got rid of everything because now essentially my map is just a medium gray.
[5:46] We'll come in here and we will select this one one more time.
[5:50] And you can see we're back essentially where we started.
[5:53] Well, where this is gonna come into play is we're actually gonna come down here to our blend mode
[5:58] and set this to subtract.
[6:00] And just like that, now we have this blended or this peeling edge effect that we can control
[6:09] independently from that information.
[6:12] So, we can say, okay, wow, that actually looks pretty good.
[6:15] How could we maybe potentially improve this a little bit more?
[6:20] Well, what I'm gonna do is I'm actually gonna come back down to my first layer.
[6:24] I'm going to go and add a filter.
[6:27] I'm gonna drag this underneath my anchor and then I'm gonna come down here to we'll try warp at first.
[6:33] And that is going to add a little bit of like break up and a regularity to those edges.
[6:38] This one could work.
[6:39] This this is probably fine.
[6:42] But I'm actually also gonna try to do blur slope, which will actually sort of add more of this like flaked edge look to it.
[6:51] So I'm gonna change the blending mode on here to maximum and then I'm gonna change this to 10.
[6:57] And then that'll allow us to kind of come in here and play 10 might not be the best.
[7:02] We might be able to do one, but you can play with kind of the in-betweens that you're getting here.
[7:07] Now, you might be saying, okay, that's cool.
[7:10] One thing that is standing out to me that could use a little improvement is this peeling is happening around the entirety of the edge,
[7:17] which could be cool, but usually things in real life aren't quite as perfect.
[7:22] So what we're going to try and do is we're going to come up here.
[7:26] We're going to add a another fill layer and let's see what happens by putting on a like a clouds or something on top of here.
[7:36] So we'll drag that in.
[7:38] This doesn't look good.
[7:39] Doesn't need to.
[7:40] We're going to set this to multiply.
[7:43] And so we come up here and we can start to break up this mask a little bit.
[7:48] We're actually going to switch this to clouds too, since those shapes are a little bit bigger and we can start to kind of play with that in order to raise up some of this information and subtract some of this information.
[8:03] So if we do like an overlay, you can see we're starting to get some irregularity on that edge, which this might be a cool effect that you're going to get.
[8:12] You're after you could play with this to start to like subtract some of that information from the mask that's below it.
[8:20] So if I start to do something like this, you can see that now I'm I'm getting it affected in certain areas, but I'm getting I'm having it retained in other areas.
[8:30] So you can play with these options.
[8:32] So we'll try maybe something else in here.
[8:36] So let's try like a grunge, for example.
[8:38] So you can see that that changes the effect that we're after.
[8:41] Maybe it's a little bit too harsh.
[8:43] So what I could do is I could move that in my layer stack potentially like down here in order to change the effect that I'm getting on it.
[8:54] So maybe moving it to right here and then running a another blur.
[9:00] But this one is just going to be a little bit less intense like that.
[9:06] And we just need to make sure to adjust it in our layer stack.
[9:10] So if we start to do this, you can see we're starting to push some of these areas down and some of them up, which is cool.
[9:19] So this is ultimately what our mask is going to look like.
[9:23] You can see there's some irregularity around the edges, some break up, you know, different things like that.
[9:28] So you can play to really kind of get different options on here.
[9:32] But not only are we able to play with the height, you know, usually if you look at peeling paint, we can also come here and adjust our color.
[9:40] So say we want this paint to be a little bit more light or like a yellow or something, depending on what's actually happening.
[9:49] And now we have this sort of detail going on, which is really cool.
[9:53] So that is kind of one example of how to use this.
[9:56] There's a lot of ways to use this in your workflow in terms of building different types of anchor pointed processes.
[10:03] I have a whole library of materials that I've made from things like peeled paint, torn fabric, emissive, burned wood, a lot of different cool things.
[10:14] Another one that kind of follows the same process is going to be this one, which is just taking the same sort of workflow,
[10:23] but applying additional information on the outside as well as adding dense on the inside.
[10:29] So you can see if we come here and we start to paint, the more pressure that we're applying here, the more it's going to push down.
[10:41] If I just paint over here, but paint very lightly, maybe come in here and kind of bring that up.
[10:48] Now I can create paint peel, but also dense and the bubbling that's happening around the material as well.
[10:56] So you have a lot of options and abilities to make different things.
[10:59] And all of this stuff is just me painting in the base layer in order to use that and create an anchor point to drive all of this information.
[11:08] So this one, just to walk through things is doing the same thing, painting my shape, painting my dense by creating a mask in order to start to push things down.
[11:18] So if we turn this on and off, you can see kind of that's what's happening there.
[11:23] Also creating and pushing deep dense.
[11:26] So using a bunch of different layers on here in order to kind of get a more pushed down point, creating the bubble shapes on here.
[11:35] So you can see we're creating the mask for these.
[11:38] It's not applying or affecting anything yet, but we're creating that mask.
[11:42] And then up here, we are now applying that detail.
[11:45] So we're actually adding the bumps here so we can make those go down, make those go up.
[11:52] We can change the color of them.
[11:54] And then we also have control of the lifted edges.
[11:57] So that's just thinking outside the box in different ways that I could use this in terms of making complex things.
[12:06] So these are really useful and efficient ways to make cool materials and hopefully adds cool, interesting stuff to your character.
[12:15] So if you found this useful, make sure to comment, like, subscribe, follow for more.
[12:20] Hopefully you guys can find some of this useful in terms of some substance, paint or processes.
[12:25] Let me know some of the things you'd like to see in the future and I'll see you guys in the next one.



---

## Captured Frames

- [0:25] tutorials/frames/how-to-make-a-peeled-paint-effect-with-anchor-points-substance-painter/frame_000.jpg
- [0:50] tutorials/frames/how-to-make-a-peeled-paint-effect-with-anchor-points-substance-painter/frame_001.jpg
- [1:26] tutorials/frames/how-to-make-a-peeled-paint-effect-with-anchor-points-substance-painter/frame_002.jpg
- [3:08] tutorials/frames/how-to-make-a-peeled-paint-effect-with-anchor-points-substance-painter/frame_003.jpg
- [3:53] tutorials/frames/how-to-make-a-peeled-paint-effect-with-anchor-points-substance-painter/frame_004.jpg
- [5:13] tutorials/frames/how-to-make-a-peeled-paint-effect-with-anchor-points-substance-painter/frame_005.jpg
- [6:00] tutorials/frames/how-to-make-a-peeled-paint-effect-with-anchor-points-substance-painter/frame_006.jpg
- [6:45] tutorials/frames/how-to-make-a-peeled-paint-effect-with-anchor-points-substance-painter/frame_007.jpg
- [8:03] tutorials/frames/how-to-make-a-peeled-paint-effect-with-anchor-points-substance-painter/frame_008.jpg
- [9:45] tutorials/frames/how-to-make-a-peeled-paint-effect-with-anchor-points-substance-painter/frame_009.jpg
- [10:41] tutorials/frames/how-to-make-a-peeled-paint-effect-with-anchor-points-substance-painter/frame_010.jpg

---

## Structured Notes

### Core Technique
A freehand-paintable "lifted/flaking metal-edge paint peel" effect built entirely from a single Anchor Point sourced from a hand-painted Paint layer, then processed through chained Levels/Blur/self-subtract-blend and procedural noise breakup — so the artist paints once and the peeling-edge detail (height bump + irregular flake silhouette) generates automatically wherever the paint goes.

### Summary
Direct continuation/production application of Jared Chavez's "Building Masks Explained" anchor-point fundamentals video (demonstrated on a red-and-chrome cylindrical prop, e.g. a grenade/canister). The core insight: to get a *ring-shaped lifted lip* around a paint stroke (not just a flat painted patch), you reference the same anchor point twice inside one mask stack and use `Subtract` blend mode to cancel out the interior, leaving only the grown edge band. That edge band is then broken up with procedural noise (Warp filter, then `Blur Slope` filter set to `Maximum` blend mode at intensity ~1-10) and further irregularized with two Clouds-type fill layers (`Multiply` and `Overlay` blend modes) so the peeling edge doesn't read as a perfect uniform ring. A second demo shows the same anchor-driven principle extended to pressure-sensitive dent/bubbling: brush pressure while painting the base layer controls how deep the anchor-driven height push goes, letting one painted stroke produce both a lifted flaking edge AND a pushed-down dent/bubble in the same pass.

### Key Steps
1. Create a base **Fill layer** set to a shiny metal preset (base material the paint will "reveal") with a black mask.
2. Inside that mask, add a **Paint layer** — this is the layer the artist freehand-paints on; everything downstream references this paint information.
3. Paint a stroke directly on the model. Note the natural soft gradient/whitening at the blend edge between paint and base metal — this softness is undesirable for a hard peel silhouette.
4. Add a **Levels** adjustment on top of the paint mask and clamp down the black/white points to harden the paint shape into a crisp, less-gradated silhouette.
5. Add a **Blur** filter (~2.25) on top, then a second **Levels** on top of that to re-clamp the now-blurred shape — the combination produces a smooth but still well-defined edge (less noisy/irregular than the raw painted stroke, but not razor-hard either). This layer stack is the reusable **base mask**.
6. Add an **Anchor Point** on top of this base-mask stack and name it descriptively (e.g. "metal paint anchor" / `paint anchor`) — anything downstream can now reference this exact mask shape by name.
7. Add a new layer above with a black mask, add a **Fill layer** inside that mask, and set its content source to the anchor point just created (select it from the Anchor Point dropdown). Toggle the `Height` channel on to visualize the raw anchor-driven displacement — at this point it just reproduces the flat painted shape as a flat height push, which is not yet the "lifted lip" look.
8. To build the flaking lip: add a **Blur** on top of the anchor-referenced fill to bleed/grow the mask outward past the original paint silhouette, then push a **Levels** further out so the falloff extends even more (accept some faceting/artifacting from pushing blur to the extreme — it doesn't hurt the result). This grows the *outer* boundary of the effect beyond where the paint was actually applied.
9. **Core trick — cancel the interior:** add a second **Fill layer** referencing the *same* anchor point again, and set this new layer's **blend mode to `Subtract`**. Subtracting the original (non-grown) anchor shape from the grown/blurred one leaves only the *ring band* between the original paint edge and the grown edge — this ring is the lifted, peeling lip; the interior of the paint area is fully cancelled out and unaffected by the height push.
10. **Break up the ring's regularity:** on the base paint layer (below the anchor), add a **Filter** — try `Warp` first (adds mild irregularity/breakup to the edges), then compare against **`Blur Slope`** (produces a more distinct "flaked edge" look); set the Blur Slope layer's blend mode to `Maximum` and dial its intensity (values around 1-10 were tested — lower values like 1 sometimes read better than the default 10, adjust to taste).
11. **Further edge irregularity (optional refinement):** add another fill layer with a **Clouds**-type generator/noise on top, set blend mode to `Multiply` first (darkens/subtracts information from the mask below), then try `Overlay` (adds irregularity while retaining information in some areas and removing it in others) — reposition this layer up/down the stack and try alternate noise types (a second, larger-scale Clouds variant, or a `Grunge` map) to change how harsh/organic the broken edge reads; if a Grunge result is too harsh, move it lower in the stack and add another Blur to soften it.
12. **Color pass:** once the height/mask breakup reads correctly, adjust the paint layer's base color (e.g. shift toward yellow/light) to represent the actual peeled-paint color rather than leaving it a placeholder tone.
13. **Second application — dents/bubbling via brush pressure:** using the identical anchor-referenced-fill-layer architecture, paint pressure on the base paint layer is used as a second control axis — light pressure paints a shallow push, heavy pressure paints a deeper push — so the same anchor-driven pipeline can simultaneously produce a lifted peeling edge on the outside AND a pushed-in dent/bubble on the inside of the same painted stroke, purely by varying how hard you paint.
14. Chavez notes this exact "paint-once, anchor-drives-everything" pipeline is reused across his personal material library for peeled paint, torn fabric, emissive damage, and burned wood effects — treat this stack architecture as a template, not a one-off.

### Layers / Tools / Settings
- Base Fill layer: shiny metal preset, black mask.
- Paint layer (inside the mask) — freehand-painted source information.
- `Levels` (x2, one per hardening pass) — clamps black/white points to control mask hardness/falloff.
- `Blur` filter — softens/grows the mask; also reused post-anchor to grow the outer edge before the subtract trick.
- **Anchor Point** — named reference to the finished base-mask stack; referenced twice downstream.
- Fill layer #1 referencing the anchor — drives the raw Height push; blend mode default (Normal/Passthrough).
- Fill layer #2 referencing the **same** anchor — blend mode **`Subtract`** — cancels the un-grown interior, isolating only the grown edge ring (the core "lifted lip" trick).
- `Warp` filter — mild edge breakup (compared against, not always kept).
- `Blur Slope` filter — blend mode **`Maximum`**, intensity ~1-10 — produces the flaked-edge look; applied on the base paint layer, positioned underneath the anchor layer in the stack.
- Clouds-type fill/generator layers — blend modes `Multiply` then `Overlay` (or `Grunge` map as an alternate noise source) — further breaks up ring regularity; layer stack position changes the effect strength.
- `Height` channel toggle — used purely to visualize/validate the anchor-driven displacement while building the mask (turned off again once validated).
- Base Color adjustment on the paint layer — final color pass (e.g. yellow-tinted peeled paint).
- Brush pressure (pen pressure sensitivity) — used as a second parametric control axis for simultaneous dent depth in the companion "torn/bubbled" variant.

### Difficulty
Intermediate/Advanced — assumes familiarity with anchor points, blend modes, and mask-stack construction (this video explicitly continues from "Building Masks Explained"); the double-anchor-reference-with-Subtract trick and the growth-then-cancel logic are non-obvious.

### App & Version
Substance 3D Painter — version not specified on screen or in narration.

### Tags
layers, fill-layer, paint-layer, masks, anchor-point, blend-mode, height, generator, procedural, particle-brush, intermediate, advanced

---

## Related Tutorials
- [SUBSTANCE PAINTER: Building Masks Explained](substance-painter-building-masks-explained.md) — same creator, direct prerequisite; this video explicitly continues from the anchor-point fundamentals taught there, applying them to a full peeling-paint production effect.
- [Anchor Point Magic 03 - Paint Peel Effect in Substance 3D Painter](anchor-point-magic-03---paint-peel-effect-in-substance-3d-painter-adobe-substanc.md) (Substance3D official) — same peeling-paint goal via a very similar double-anchor-reference technique (inverted+Blur bump, non-inverted+Multiply clip) — useful side-by-side comparison of two different studios' takes on the identical underlying trick (here: grow-then-Subtract; there: invert-then-Multiply-clip).
- [Advanced Peeling Paint Effect in Substance 3D Painter](advanced-peeling-paint-effect-in-substance-3d-painter.md) (Javad Rajabzade) — another anchor-point-driven peeling-paint effect using Voronoi-fractal/Lighten-Divide mask math; compare against this video's Blur-Slope/Clouds/Grunge-based edge-breakup approach.
- [How to create a paint peeling effect in Substance Painter](how-to-create-a-paint-peeling-effect-in-substance-painter.md) (Wes McDermott) — a fourth independent take on paint-peel via anchor points, referenced by 4 downstream layers with filter-native blend modes and a Mask Outline filter — good comparison set now that 4 different creators' peeling-paint methods are all in this library.
- [Creating a Leather Material for Footwear with Anchor Points in Substance 3D Painter](creating-a-leather-material-for-footwear-with-anchor-points-in-substance-3d-pain.md) (footwear anchor trilogy) — shares the chained-anchor-reference-with-Invert architecture for building folds/creases from a single source mask.
- [HOW TO MASTER TEXTURing in SUBSTANCE PAINTER](how-to-master-texturing-in-substance-painter.md) — same creator; conceptual companion — this video's "hero" detail (peeled paint) is a concrete example of the Phase 3 "graphic, readable shapes" detail pass described there.
- [TEXTURING METAL from Scratch in SUBSTANCE PAINTER](texturing-metal-from-scratch-in-substance-painter.md) — same creator; that video's final anchor-point-driven flake/peel mask (Key Step 16) is the same double-anchor-reference peeling technique demonstrated here in full standalone detail.
