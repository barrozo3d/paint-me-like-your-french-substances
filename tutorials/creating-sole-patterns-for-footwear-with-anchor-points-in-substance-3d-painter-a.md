---
title: Creating Sole Patterns for Footwear with Anchor Points in Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=AoGXdldOWQA
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated on screen; window title reads 'License: 109 days remaining - 02 Soles', shader Displacement/Tessellation settings visible in-frame"
tags: [anchor-point, masks, layers, fill-layer, paint-layer, blend-mode, height, basecolor, roughness, procedural, alpha, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/creating-sole-patterns-for-footwear-with-anchor-points-in-substance-3d-painter-a/
frame_count: 7
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Creating Sole Patterns for Footwear with Anchor Points in Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=AoGXdldOWQA)
**Author:** Adobe Substance 3D
**Duration:** 9m42s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Welcome to this multi-part tutorial series where we will go over some more advanced techniques
[0:13] on how to use anchor points in your project.
[0:16] This series is a follow up of our basic anchor point series which you can also find on this
[0:21] channel.
[0:22] In this video we will go over on how to create these shoe soles with the help of anchor points.
[0:28] This means that we will go over on how to create the actual base of your sole, how to
[0:33] derive color from it, and also how to place a pattern inside of it all using anchor points.
[0:40] So this is going to be quite a fun video and let's dive right in.
[0:44] So what are anchor points?
[0:46] Anchor points are a powerful feature that lets you reuse a part of your layer stack.
[0:52] This means that you can define a mask or layer once and reference it dynamically in other
[0:58] layers.
[0:59] If you change the anchor point, all references are updated as well, letting you work smarter
[1:05] and faster.
[1:06] Okay, so what you want to do is you want to get started by creating the actual indents
[1:10] of our sole first.
[1:12] So for this, this is not very difficult, just go out and out of fill layer and we want to
[1:16] go ahead and just call this like sole for example.
[1:20] And honestly, we only really need the color and the height map over here.
[1:24] So we can turn everything else off and just go ahead and set your height in the minus.
[1:29] And the reason we do this is because we of course want to indent.
[1:32] Now, as you can see, this completely breaks your model, but don't worry because as soon
[1:36] as we go ahead and add a black mask, that will fix it.
[1:40] The reason, by the way, that it breaks our model is because I have my height map turned
[1:46] on.
[1:47] So if you go ahead and go to this little settings box over here, which is your shader settings
[1:51] and you scroll down, you can go ahead and if you want, you can copy my settings.
[1:55] I just have displacement turned on so that we get actual jump tree displacement.
[2:00] So it's just enabled source channel height, scale 0.035 and then add some tessellation
[2:07] to it.
[2:08] So just so you know, it's just like a nice extra detail.
[2:11] So for this, all we really need to do is we need to stop by just painting in like a
[2:15] soul.
[2:16] Now, because this is quite time consuming, I will just show you one where I go to my
[2:21] brushes and grab a basic hard brush and then just go ahead and give it like a nice size.
[2:27] Let's say around five.
[2:28] And then you just basically want to paint in the large shape that is going to be indented
[2:34] in your ship in your zone.
[2:36] So I'm just going to hold shift and I'm just going to drag it like this.
[2:39] And it doesn't have to be super precise yet because we are going to blur this.
[2:44] So I'm just going to carefully try and just get like an even distance away from like the
[2:49] end of my soul like this.
[2:52] And I know that it might look quite bad, but don't worry, this will be fixed later.
[2:58] Yeah, let's say that we do something like this, for example, over here.
[3:03] And then what we can do is we can just paint in this inner center bit.
[3:07] You can see over here.
[3:08] Yeah, let's say my brush size a bit bigger.
[3:10] There we go.
[3:11] So let's say you have something like this.
[3:13] Then what you want to do is you just want to go ahead and go up here and add a filter
[3:19] and then add a blur.
[3:20] For example, I'm not very good at like painting.
[3:22] So the blur will also once again, like help me just improve my shape a little bit more
[3:28] and like that you could get a shape.
[3:30] Now I did this quite quickly.
[3:31] So what I will do is I will go ahead and I will paint in my shapes and I will then improve
[3:37] them also a little bit more because I need to do quite precise painting, but this can
[3:41] take a few minutes.
[3:42] So let me just quickly do that and then we will continue with the tutorial.
[3:46] Here we go.
[3:47] So as you can see, I just paint in like a random patch one in here.
[3:51] And if you hold Alt and click, you can see that this is my mask.
[3:55] So it is a very basic just to get like something that looks pretty decent.
[4:00] So what we're going to do now is we are going to give the soul a specific color.
[4:04] This is always nice to just have control over the color.
[4:07] Now for this, we now need to jump into anchor points.
[4:10] So first of all, click on your mask and add a simple anchor point so that we can reference
[4:15] this mask that we just spent time painting.
[4:19] Then if we go ahead and add a new fill layer over here, we can call this soul color.
[4:27] And once again, we only need to color.
[4:29] And if you want, you can also have the roughness in here.
[4:32] It's not really needed, but let's just go ahead and give it like a darker color, something
[4:36] like this and maybe make the roughness like a little bit duller.
[4:40] Honestly, the roughness is not that needed in this case.
[4:43] It's just an example.
[4:45] So we can then go ahead and add a black mask.
[4:47] And all we really need to do is we need to reference our anchor point by going down here,
[4:53] adding a fill, going into grayscale and then selecting our anchor point.
[4:58] Now at this point, as you can see, it is not looking very nice.
[5:01] There's like these little stripes and everything.
[5:03] So what we want to do is we just want to go ahead and play around with our levels.
[5:07] For example, by pushing our black levels down and our white levels up until we get a pretty
[5:13] nice, even color over here.
[5:19] There we go.
[5:20] That's looking pretty good.
[5:23] And that is already it for our color.
[5:24] So that's really nice about the anchor points that we just have control over our levels
[5:28] on top of it.
[5:29] So let's get started with the thing that we all came here for, which is our patterns.
[5:34] Let's go ahead and create one more fill layer that we will call pattern.
[5:40] And now with this one, I once again, I think I only need my height and I need my color.
[5:45] Now one thing I do want to do is I want to go ahead and first of all, set my height in
[5:52] the minus.
[5:53] It will not make much sense just yet, but set my height in the minus, then art a black
[5:58] mask.
[5:59] And once we have our black mask, we want to go ahead and go from base color up here to
[6:05] height.
[6:06] And you want to set this pattern specifically to be in the max, light and max.
[6:13] So this will make the transition a little bit better.
[6:16] And this will also only allow our pattern to go up and not go down.
[6:21] Once we've done that, we can go ahead and we can start by adding our actual pattern.
[6:25] And to do this, we simply want to go ahead and let's art a fill.
[6:29] And this fill is not for anchor point, because what you can do with this fill also is you
[6:33] can insert like grayscale image.
[6:36] So if we go to textures, there are a lot of patterns in here.
[6:40] See here, you can see a lot of them.
[6:43] And I know that this one is quite nice, like the fabric diamond alternate.
[6:47] So I'm just going to drag this one on.
[6:49] I'm going to boost up my scale to around 10 so that it is a lot smaller.
[6:55] Which you can see over here.
[6:56] So now we got something like this.
[6:59] And with this one, we can just go ahead and we can go up here and we can play around a
[7:03] little bit more with our height.
[7:04] See now, as you can see, this looks really, really bad right now.
[7:08] But don't worry.
[7:09] What we're going to do now is first of all, let's add a nice little blur.
[7:14] So let's add a filter with a blur.
[7:17] And this one will be specific so that our shapes you see so that we can make our shapes
[7:21] a little bit nicer.
[7:24] Like that.
[7:25] And then finally, we need to, of course, mask it out so that it is not being included
[7:30] in the rest of our shoe and only on the inside of our soul over here.
[7:35] The way that we can do this is we can add a simple fill and reference our anchor point,
[7:40] which is our soul mask over here.
[7:43] And then you just want to set this fill to be a multiply.
[7:47] And then you can already see it working.
[7:49] So at this point, all you really want to do is you just want to go ahead and play around
[7:53] a little bit more with your levels, maybe you can see that the transition is pretty good,
[7:58] but you can use your levels to basically make the transition a little bit better.
[8:03] So let's go for something like something like this.
[8:07] I think it looks quite nice.
[8:09] And then it is just up to you to play around with your blur to see how much of a blur you
[8:14] want to give it.
[8:15] And also to play around with your height.
[8:17] You can see over here to just give it like a nice height.
[8:19] You can also push it out if you want.
[8:21] But let's just go ahead for like quite a subtle height like this.
[8:25] OK, that's pretty cool.
[8:26] Now, of course, if you want to go ahead and you want to give this pattern also a color,
[8:32] you can always go ahead and go into your pattern.
[8:35] Add another anchor point.
[8:37] And then let's say that we like, for example, add another layer and call this pattern underscore
[8:43] color.
[8:44] And let's give this like something interesting.
[8:46] So let's make the roughness.
[8:50] Yeah, let's actually keep it a bit shiny.
[8:52] Let's go for like a yellowish color.
[8:54] I don't know.
[8:56] You're like a nice yellow color.
[8:58] And then all you need to do is once again, the repetition of your soul color after black
[9:02] mask after fill layer to the mask.
[9:05] And this time in your anchor points, just grab your patron mask.
[9:10] And then once again, it is just a matter of playing around over here with your levels.
[9:15] To get it the way that you want.
[9:17] And just like that, you can also play around with your patron and you can always go back
[9:21] in and like change it a little bit if you want.
[9:24] So that's the cool thing about this.
[9:25] You can create any color you want.
[9:28] You can have like a lot of flexibility with this just to create something interesting.
[9:32] And that is about it for this tutorial.
[9:34] I hope that you find it useful and I hope to see you next time.



---

## Captured Frames

- [1:55] tutorials/frames/creating-sole-patterns-for-footwear-with-anchor-points-in-substance-3d-painter-a/frame_000.jpg
- [2:39] tutorials/frames/creating-sole-patterns-for-footwear-with-anchor-points-in-substance-3d-painter-a/frame_001.jpg
- [3:51] tutorials/frames/creating-sole-patterns-for-footwear-with-anchor-points-in-substance-3d-painter-a/frame_002.jpg
- [5:13] tutorials/frames/creating-sole-patterns-for-footwear-with-anchor-points-in-substance-3d-painter-a/frame_003.jpg
- [6:49] tutorials/frames/creating-sole-patterns-for-footwear-with-anchor-points-in-substance-3d-painter-a/frame_004.jpg
- [7:47] tutorials/frames/creating-sole-patterns-for-footwear-with-anchor-points-in-substance-3d-painter-a/frame_005.jpg
- [8:56] tutorials/frames/creating-sole-patterns-for-footwear-with-anchor-points-in-substance-3d-painter-a/frame_006.jpg

---

## Structured Notes

### Core Technique
Building a shoe sole from a single hand-painted mask reused through Anchor Points three times over: once to derive the sole's own recessed shape/color, and again to constrain a separate tiled pattern layer (plus its own color pass) strictly inside that same sole area — all editable independently via Levels without repainting anything.

### Summary
Second video in the "advanced anchor points" footwear series (follow-up to a more basic anchor-point series on the same channel). Enables real-time viewport **Displacement + Tessellation** in Shader Settings (Source Channel = Height, Scale = 0.035, adaptive tessellation) purely as a nice-to-have visual aid while sculpting the sole in texture. Builds the sole shape: a "Sole" fill layer with only Color + Height enabled, Height set negative (to indent), which visibly breaks the model until a black mask is added; the sole outline and inner section are hand-painted with a basic hard brush (Shift-drag for straighter strokes) roughly, then cleaned up with a **Blur** filter on the mask rather than painted with high precision — Alt-click the layer to preview the raw mask. Sole color: add an **Anchor Point** to the sole mask, create a new "Sole Color" fill layer (Color, optionally Roughness), mask it with a black mask + fill referencing the sole anchor, then use **Levels** (push black point up, white point down) to even out the raw mask's blotchiness into a clean flat color fill — demonstrating that anchor-referenced layers stay independently tunable after the fact. Pattern layer: new "Pattern" fill layer (Height + Color only), Height set negative first, add a black mask, and critically set that mask's blend mode from Base Color to **Height**, with the pattern set specifically to **Max (Lighten) blend** so the tiled pattern can only ever push detail up, never down, into the sole recess. Inside that mask, add a fill (not an anchor reference) and drag in a built-in tileable pattern texture (Fabric Diamond Alternate used in the demo) from the pattern library, scaling it up (~10) to shrink the tile size; blur the result to soften the raw pattern edges, then mask the whole pattern layer to the sole's footprint by adding a fill referencing the **sole anchor point** with blend mode set to **Multiply**, and fine-tune the sole/pattern-edge transition with Levels; finally adjust the pattern's own Height push (kept subtle in the demo) for the final embossed look. Pattern color (optional): add a second Anchor Point on the pattern mask, create a "Pattern Color" fill layer (Color + Roughness, kept shinier/yellow in the demo), and repeat the same black-mask-plus-anchor-referencing-fill-plus-Levels recipe, this time referencing the pattern anchor instead of the sole anchor — giving the tiled pattern its own independently colored, independently editable pass.

### Key Steps
1. Enable viewport Displacement for a nicer real-time preview while sculpting: Shader Settings → Displacement/Tessellation → enable, Source Channel = Height, Scale ≈ 0.035, with adaptive Tessellation — purely a visual aid, not required for the technique itself.
2. Create a "Sole" fill layer: enable only Color + Height, set Height negative to indent, then add a black mask (fixes the initially broken/inverted-looking model preview).
3. Hand-paint the sole's outer boundary and inner center section using a basic hard brush (size ~5), holding Shift for straighter strokes; precision isn't critical since a blur pass will clean it up afterward.
4. Add a **Blur** filter to the mask to smooth and improve the rough hand-painted shape; Alt-click the layer/mask to preview it directly.
5. Add an **Anchor Point** to the finished sole mask so it can be referenced elsewhere.
6. Create a "Sole Color" fill layer (Color, optionally Roughness for a duller finish); add a black mask, then a fill inside it referencing the sole Anchor Point (via the grayscale/anchor-point field).
7. Clean up the raw anchor-referenced mask with **Levels** — push the black point up and the white point down until the color reads as an even, clean fill rather than a blotchy/streaky one.
8. Create a "Pattern" fill layer: enable Height + Color, set Height negative initially, add a black mask.
9. On that mask, change the channel dropdown from Base Color to **Height**, and set the pattern's blend to **Max (Lighten)** — this lets the tiled pattern only raise detail upward, never push further into the sole's recess.
10. Inside the mask, add a fill and drag in a tileable grayscale pattern texture from the built-in pattern library (Fabric Diamond Alternate demoed); increase its Scale (~10) to shrink the tile repeat to a usable size.
11. Add a **Blur** filter to soften the raw pattern's harsh edges.
12. Constrain the pattern to only the sole area: add another fill inside the mask referencing the **sole Anchor Point**, with its blend mode set to **Multiply** — instantly confines the pattern to the sole footprint.
13. Fine-tune the sole/pattern boundary transition with Levels, and adjust the overall Blur amount and Height push amount to taste (kept subtle in the demo).
14. Optional pattern coloring: add a second Anchor Point, this time on the Pattern layer's mask; create a "Pattern Color" fill layer (Color + Roughness — kept shinier/yellow in the demo); repeat the black-mask + anchor-referencing-fill + Levels recipe, referencing the pattern anchor this time, to give the tiled pattern its own independent, freely re-tunable color pass.
15. Because every stage references an Anchor Point rather than duplicating paint data, any of the three layers (sole shape, sole color, pattern color) can be revisited and adjusted independently at any time without repainting.

### Layers / Tools / Settings
- **Shader Settings → Displacement/Tessellation**: Source Channel = Height, Scale ≈ 0.035, adaptive Tessellation (viewport-only aid).
- **Sole** fill layer: Color + Height (negative), black mask, hand-painted with a basic hard brush + Blur filter, carries an **Anchor Point**.
- **Sole Color** fill layer: Color (+ optional Roughness), black mask + fill referencing the Sole anchor + Levels.
- **Pattern** fill layer: Height (negative) + Color, black mask with channel set to **Height** and pattern blend mode **Max (Lighten)**; built-in tileable pattern texture (Fabric Diamond Alternate) scaled up; Blur filter; second fill referencing the Sole anchor with **Multiply** blend mode to confine it to the sole area; carries its own Anchor Point.
- **Pattern Color** fill layer: Color + Roughness, black mask + fill referencing the Pattern anchor + Levels.
- Recurring pattern throughout: black mask → fill referencing an Anchor Point → Levels for cleanup — the core reusable recipe demonstrated across all three color/pattern passes.

### Difficulty
Intermediate (anchor-point-chained layer construction; more approachable than fully procedural generator-driven masking since hand-painting is the primary shape-definition tool).

### App & Version
Substance 3D Painter. No version number stated on screen; window title bar reads "License: 109 days remaining - 02 Soles" (subscription license countdown, not a version indicator).

### Tags
`anchor-point`, `masks`, `layers`, `fill-layer`, `paint-layer`, `blend-mode`, `height`, `basecolor`, `roughness`, `procedural`, `alpha`, `intermediate`

---

## Related Tutorials
- **Creating Fabric stitches for Footwear with Anchor Points in Substance 3D Painter** (`tutorials/creating-fabric-stitches-for-footwear-with-anchor-points-in-substance-3d-painter.md`) — first video in the same footwear/anchor-points series, same shoe asset.
- **Creating a Leather Material for Footwear with Anchor Points in Substance 3D Painter** (`tutorials/creating-a-leather-material-for-footwear-with-anchor-points-in-substance-3d-pain.md`) — third video in the same series.
- **How to TEXTURE like a PRO with ANCHOR POINTS | Substance Painter Tutorial** (`tutorials/how-to-texture-like-a-pro-with-anchor-points-substance-painter-tutorial.md`) — Jared Chavez's independent anchor-point deep-dive, same core reuse technique.
- **Anchor Point Magic 01** (`tutorials/anchor-point-magic-01---double-layer-setup-in-substance-3d-painter-adobe-substan.md`), **02** (`tutorials/anchor-point-magic-02---micro-normals-micro-height-in-substance-3d-painter-adobe.md`), **03** (`tutorials/anchor-point-magic-03---paint-peel-effect-in-substance-3d-painter-adobe-substanc.md`), **04** (`tutorials/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance.md`) — the "basic anchor point series" this video explicitly builds on.
