---
title: Anchor Point Magic 04 - Rust Fade Effect in Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=LmtepSmnRQs
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not stated on screen; window title reads 'License: 171 days remaining - Anchor_Video_04_Texture_Begin' (same project/license-countdown pattern as series entries 01-03)"
tags: [anchor-point, masks, layers, fill-layer, paint-layer, generator, smart-mask, blend-mode, height, basecolor, roughness, metallic, procedural, advanced]
extraction_status: complete
frames_dir: tutorials/frames/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance/
frame_count: 12
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Anchor Point Magic 04 - Rust Fade Effect in Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=LmtepSmnRQs)
**Author:** Adobe Substance 3D
**Duration:** 15m6s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] In our fourth and final video of this multi-part tutorial series on how to use anchor points
[0:12] in various ways, we will go over a much more complex setup in order to basically generate
[0:19] a bunch of different types of rust on our model.
[0:22] Using just a simple rust generator like you can see over here, we can fully generate a
[0:27] rust along with the glow around it and even along with all of the leaks also around that.
[0:33] So this is a really cool setup that we will go over.
[0:36] So what are anchor points?
[0:39] Anchor points are a powerful feature that lets you reuse a part of your layer stack.
[0:44] This means that you can define a mask or layer once and reference it dynamically in other
[0:50] layers.
[0:52] If you change the anchor point, all references are updated as well, letting you work smarter
[0:57] and faster.
[0:58] Ok, so before we get started, I just wanted to go over our base scene.
[1:04] So over here, let's get started with the first one.
[1:07] We will have a simple bronze material over here which will act as our base material and
[1:12] it's just a dull looking bronze material.
[1:14] On top of this, we have a simple fill layer that only has the height map activated and
[1:20] this fill layer has a mask that contains this little bit of text over here.
[1:25] And finally, we will have a paint layer on top of this.
[1:29] This is also a fill layer that just has like a white base color and then you can just play
[1:34] around with your roughness to get all shiny paint or a very dull looking paint.
[1:40] Now this white paint layer contains a simple black mask and this black mask contains a
[1:46] smart mask to basically control how much of the paint that we want to have.
[1:51] In this case, I used the surface worn smart mask that you can find in your assets library.
[1:59] So that is it for the base setup.
[2:01] Now I want to get started by already placing my anchor points so that I can reference them
[2:06] later on.
[2:07] So over here in our white paint, just simply click on the mask and we can go down here
[2:11] and we can add our anchor point and I'm just going to leave the name the same.
[2:16] I will do the same for our text height.
[2:18] Click on the mask, go down here and let's add an anchor point.
[2:23] Once this is done, it is time for us to start adding our rust.
[2:27] If you go into your library, you want to go to materials and over here you have two different
[2:32] rust materials that you can use.
[2:34] So you can use whichever one you want.
[2:36] I'm just going to go ahead and I'm going to use the first one and simply drag this
[2:40] onto my layers.
[2:42] Now this rust, it's a little bit too intense for my taste.
[2:46] So what I'm going to do is I'm just going to go down to my rust color and I'm going
[2:50] to like just move my slider to make it like a little bit more darker and also slightly
[2:55] duller and maybe like a little bit more reddish.
[2:57] I'm not sure.
[2:59] You just kind of like play around with it.
[3:01] Let's say we go for something like this.
[3:04] And lastly what I want to do is I just want to go into my UV transformations and I'm just
[3:09] going to set the scale to maybe two.
[3:11] Yeah, I think two looks pretty good.
[3:14] Now off camera, I already went ahead and I just played around a little bit more with
[3:18] the color because I didn't want to record that.
[3:21] So this is the color that I'm going to go for over here.
[3:24] And if you want, you can also play with your cavities to like control a little bit more
[3:27] of like the damage that the rust has contained.
[3:30] Okay, perfect.
[3:31] So now that we have this, the first thing that we want to do is we want to add a simple
[3:36] black mask over here and then we want to reference our white paint anchor points.
[3:43] So we go to our black mask, we go down here and add the fill layer just like in the other
[3:47] videos.
[3:48] And then we just want to go ahead and click on our gray scale, go to anchor points and
[3:53] grab our white paint mask that you can see over here.
[3:57] Now at this point, it looks like that I need to invert it so I can just go into my levels
[4:01] and press invert.
[4:03] And for the rest, if you want, you can of course play around a little bit more with
[4:06] your levels to make it more or less strong.
[4:09] But I'm just going to go ahead and I'm just going to keep it at the default over here.
[4:13] Okay, perfect.
[4:14] So now what we're going to do is we are going to create our glow system for this.
[4:19] What we want to do is we want to add a brand new plain fill layer over here and let's go
[4:25] ahead and call this rust underscore glow.
[4:29] Now with this one, the ones that you want so we don't need a hard map for this, you
[4:34] want to probably keep the metallic map on and you don't need a normal map for this.
[4:38] So for our rust glow, I'm going to set my roughness quite low so that it is not as shiny
[4:43] because I don't really feel like rust glow would be shiny.
[4:47] Then in your base color, you just want to get like a very strong orange looking color.
[4:51] Once again, I just went ahead and off camera.
[4:53] I already found the perfect color, which was a d 6 7 0 B in the hash code.
[5:02] And it's just basically like this very strong orange looking color.
[5:06] Now once you've done that, all you need to do is you need to go ahead and you need to
[5:09] add another mask to this one.
[5:12] And we are going to add a black mask.
[5:15] Okay, so this is where it is going to get a little bit more advanced.
[5:18] So let's go ahead and zoom in.
[5:20] What we want to do is first of all, we need to reference our white paint mask.
[5:25] That's quite basic.
[5:26] So we're just going to go ahead, add a fill layer.
[5:30] And in here, we can go to our anchor points and grab the white paint mask fill layer that
[5:35] you have over here.
[5:36] Now once again, we do need to invert this so that we actually have to glow over here.
[5:41] So what are we going to do now that we have this fill layer?
[5:44] So we have this mask.
[5:45] We are now going to add a filter and this filter will contain a blur.
[5:50] We do this to basically push our orange looking glow outside of the mask boundaries.
[5:58] So it's quite similar to the previous video where we used it for paint peeling.
[6:02] So you can basically control this blur over here and you can set it as strong as you want.
[6:07] So let's set this to around 1.6 for example.
[6:12] And then the next thing that you want to do is you want to go down here and you want to
[6:15] add the levels.
[6:16] The levels just gives you a little bit extra flexibility to basically control how strong
[6:22] your glow is going to be.
[6:24] Now finally, all that we need to do is the same technique as that we did with our paint
[6:29] peeling, which is that we go down and add another fill layer over here.
[6:35] And once again, we are going to reference the same white paint mask.
[6:40] And for this one, of course, what we need to do is we need to go ahead and set our blending
[6:45] mode to multiply.
[6:47] But this time we do not want to invert this mask.
[6:50] So if you do this, what you will get is you should get like a quite a strong glow.
[6:56] I would say that if we go ahead and go into our white paint and in our mask editor, boost
[7:01] up your contrast a little bit, then it works a little bit better because else the glow,
[7:05] the glow has a little bit of trouble with like very soft contrast to actually see the
[7:10] difference.
[7:11] So if we boost up our contrast a little bit like this into our rust paint layer, and you
[7:16] can just of course mess around with this, get it the way that you want it looking nicely.
[7:21] You can then go back into your blur and you can like control.
[7:24] Okay, how much of a glow do I want to give this?
[7:27] And finally, you can go also into your levels in which you can control like how strong that
[7:32] you want the glow to be.
[7:34] So if I have a look at this, I would say that I would like here, let's set the levels around
[7:38] 0.63 and our blur is pretty good.
[7:43] So maybe a little bit less.
[7:45] Let's do 1.4 for example, around 1.4.
[7:51] And yeah, I think our mask editor is now also correct.
[7:54] Maybe give it like a little bit more rust just to make it a little bit more damaged like this.
[7:58] But I think it's quite good if we just keep our contrast quite high.
[8:01] And just like that, now we have our rust and on top of this, we now also have our glow over here.
[8:07] So our next stop would probably be to include our text over here because this looks a bit
[8:13] strange that our text is just completely not affected.
[8:16] So for this, we already added an anchor point to our text.
[8:19] And all that we need to do is we need to go into our mask editor of our white paint, scroll
[8:25] all the way down.
[8:26] And this also gets referenced in the previous video.
[8:29] I believe it was video zero two.
[8:31] And then if you go into your micro height, you can go to anchor points and grab your text
[8:36] height over here, at which point that you can see that it is included.
[8:41] Now, of course, make sure to go into your micro details and have the micro height set
[8:46] to true.
[8:47] But for me, it was already set to true because of a previous test, but just make sure that
[8:51] you have it set to true.
[8:53] And for the rest, honestly, you can just play around with your AO radius and your settings
[8:56] to basically increase or decrease the amount of rust that you are going to get.
[9:01] So that is all up to you.
[9:02] However, you want to create it.
[9:05] So that will include a text and already makes it feel a lot more fitting and makes it feel
[9:09] a lot better.
[9:11] Now, also, once again, remember, if you want in your white paint, you can always just go
[9:16] at an other paint layer.
[9:18] And as long as the paint layer is below our anchor point, it will be referenced.
[9:23] This is great.
[9:24] For example, if I want to go to my brushes and like double click on the brush that I
[9:28] want, let's say that over here, we have like a harsh seam that is hard to get rid of.
[9:33] I can just go ahead and set my color to white and I can simply paint away the rust around
[9:38] this area to basically control wherever my seams are and make them less or stronger like
[9:44] that.
[9:45] Or if I simply have an area that I do not want to have any rust on, I can simply go
[9:50] ahead and I can just paint it in and out just like this.
[9:53] And it will be completely dynamic like always.
[9:57] So finally, what would be extra cool is for us to add a little bit of rust leaks and have
[10:03] these rust leaks only located near our actual rust so that they are not randomly in like
[10:08] these really large open spaces.
[10:10] For this, we are actually also going to use folders for the first time into this tutorial
[10:15] series.
[10:16] So if we go ahead and move down, we want to go all the way to the top.
[10:19] And let's go ahead and just click on here so that we are hiding basically all of our
[10:23] settings.
[10:24] It just makes everything a little bit more organized.
[10:27] And we want to get started by just duplicating our rust glow over here.
[10:31] And this rust glow, you just want to go into your mask.
[10:34] Let's call this rust underscore leaks.
[10:37] And you just want to go ahead and get rid of everything.
[10:39] I'm just duplicating this so that I do not have to reset my colors and my roughness
[10:44] in my fill layer.
[10:46] I'm going to probably make them a little bit darker.
[10:48] So let's just go into our base color and already set this a little bit darker like
[10:52] this.
[10:53] Yeah, around here should be fine.
[10:56] And now what we're going to do is we are going to add a generator to this to generate
[11:00] our rust leak.
[11:02] We can right click on the generator.
[11:06] And in this generator, there is actually one that is literally called dripping rust.
[11:10] So that's perfect.
[11:11] So we can simply click on here.
[11:13] And now you can see that it will just add this extra layer of rust.
[11:17] We can turn on the drip intensity to basically make the dripping like a little bit stronger.
[11:22] You can play around a bit more with your rust spreading to make it less or more and
[11:26] stuff like that.
[11:27] The smoothness spreading, which even actually resembles our glow that we have created.
[11:33] So that's also pretty cool.
[11:34] And just in general, you can just go ahead to like mess around with this until you get
[11:38] like something that looks quite cool.
[11:40] However, as you can see, it is all over the place right now.
[11:43] And that is not exactly what I want, especially because it is also over here.
[11:47] It is just like marking on top of our rust and everything.
[11:50] And yeah, it just doesn't feel as nice.
[11:54] So how can we fix this?
[11:56] Very easy.
[11:57] We are going to go ahead and we are going to create a folder or a group.
[12:00] So this folder, if we go ahead and call this, uh,
[12:05] dripping rust masking, it is quite cool because you can always out masks to
[12:12] folders so we can simply drag our rust leaks in here.
[12:15] And then we can add a simple black mask to this, like you can see over here.
[12:19] So now you can see that everything has disappeared because of course our mask is
[12:22] currently still black.
[12:24] We want to get started with something familiar, which is by adding a fill layer.
[12:29] And on top of this fill layer, we are going to go to anchor points and we are
[12:32] going to use our white paint over here.
[12:35] So now you can see that the dripping rust only happens around our rust over
[12:40] here and it is not overlaying on top of them.
[12:43] Now what we're going to do is we are now going to go ahead and we are going to
[12:46] add a very strong blur to this by going to art filter and adding our blur.
[12:52] And just make it really strong until you can almost not see it.
[12:55] Then once this is done, we are going to add a levels because we are going to use
[12:59] a levels to basically clamp this blur down.
[13:02] And because it is blurring only around our mask, it will automatically just
[13:06] remove all of the really flat areas.
[13:09] So if I go ahead and I can go in here and for example, use my black slider,
[13:14] you can see that over here it is working.
[13:16] So right now it is removing all of this stuff around here.
[13:21] And you can also go ahead and you can like, see, let's play around with this a
[13:24] little bit more.
[13:24] So we make the white slider a little bit towards the right, black slider towards
[13:28] the left, like this.
[13:31] And once you've done that, you can also go ahead and press invert.
[13:33] And now you can see that the drips only happen mostly wherever rust is located.
[13:39] And just like this, you can of course, just go ahead and like play around with
[13:42] this, make it less or more strong.
[13:44] This technique works really great if you have really large models.
[13:47] Of course, over here, we don't have a lot of real estate to work with, but the
[13:52] same basic concept is still here.
[13:54] Now, finally, let's say that, okay, I want to have a little bit of dripping
[13:59] rust in specific locations.
[14:01] I can now simply go ahead and add a paint layer on top.
[14:05] And I can use this paint layer.
[14:06] It's a by size bit bigger to let's say that I want to have dripping rust here.
[14:11] I can just go ahead and while my brush is white, I can just paint in a little
[14:16] bit more rust in these locations.
[14:18] And just like that, we can also paint in or out more dripping rust to basically
[14:23] overwite the system that we have right now.
[14:26] But as always, the amazing thing about anchor points is that having this, it is
[14:31] completely dynamic.
[14:33] I can now go all the way back to my white paint mask over here, go into my mask
[14:38] editor, and I can still just play around with my balance.
[14:41] And just like that, everything just works.
[14:44] And that's why anchor points are so amazing to use.
[14:47] So having this all done, of course, if this was not just a quick presentation, I
[14:52] would like to clean up these seams nicely.
[14:54] But now you can see the anchor points magic that is happening.
[14:58] And you can see how powerful that anchor points are in substance 3D painter.



---

## Captured Frames

- [1:12] tutorials/frames/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance/frame_000.jpg
- [2:11] tutorials/frames/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance/frame_001.jpg
- [2:55] tutorials/frames/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance/frame_002.jpg
- [3:53] tutorials/frames/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance/frame_003.jpg
- [4:50] tutorials/frames/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance/frame_004.jpg
- [5:50] tutorials/frames/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance/frame_005.jpg
- [6:40] tutorials/frames/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance/frame_006.jpg
- [8:36] tutorials/frames/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance/frame_007.jpg
- [9:35] tutorials/frames/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance/frame_008.jpg
- [11:13] tutorials/frames/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance/frame_009.jpg
- [12:15] tutorials/frames/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance/frame_010.jpg
- [13:14] tutorials/frames/anchor-point-magic-04---rust-fade-effect-in-substance-3d-painter-adobe-substance/frame_011.jpg

---

## Structured Notes

### Core Technique
The series finale: chaining everything from entries 01-03 (basic anchor referencing, generator Micro Height referencing, and the double-reference invert+blur+Multiply-clip technique) into one composite system where a single rust material's mask drives its own rust glow, a separate rust-drip generator is spatially confined to only appear near the existing rust (via the same blur+Levels+Multiply clip trick, now applied through a **folder mask** rather than a single layer's mask), and a text-height detail is pulled in via Micro Height so recessed lettering rusts convincingly too — with everything remaining fully hand-paintable and non-destructive throughout.

### Summary
Fourth and final video in Adobe's "Anchor Point Magic" series (same bronze valve model as entries 01-03, featuring the "MADE IN SP / 17 A" embossed plate), described as the most complex setup in the series: a single rust generator drives fully generated rust, an accompanying glow around it, and dripping rust leaks — all from anchor references. **Base scene:** a dull bronze base material; a Height-only fill layer ("Text_Height") masked with the embossed text; and a "White_Paint" fill layer (white Base Color, adjustable Roughness) whose black mask is driven by the **Surface Worn** smart mask (from the Assets library) to control how much paint coverage remains. **Setup:** add an Anchor Point to the White_Paint mask, and a separate Anchor Point to the Text_Height mask — both placed early so they're ready to reference later. **Base rust:** drag one of the two library **Rust** materials onto the layer stack above White_Paint; tune its Rust Color (darker, duller, more reddish to taste), set UV Transformations Scale to around 2, and optionally adjust Cavities for more/less damage detail. Add a black mask to the rust layer, add a **fill** inside it, reference the White_Paint anchor via the fill's Anchor Points tab, then **Invert** it (via Levels) so rust appears where paint is worn away rather than where paint remains intact. **Rust glow system:** add a new plain fill layer named "Rust_Glow" — keep Metallic on, skip Normal, lower Roughness (glow shouldn't look shiny), and set Base Color to a strong orange (~`#D6700B`-range, tuned by eye). Add a black mask to it, then: (1) add a fill referencing the **same White_Paint anchor**, inverted, to place the glow relative to worn paint; (2) add a **Blur filter** on top to push the orange glow outward past the mask's hard boundary (same push-outside-the-mask trick as series entry 03's paint peel); (3) add a **Levels** adjustment for extra strength control; (4) add a **second fill**, again referencing the White_Paint anchor, this time **not inverted** and set to **Multiply** blend mode — this clips the blurred glow back down so it reads as a tight rim around the rust rather than bleeding everywhere. Boosting the White_Paint mask's own **Contrast** (in its Mask Editor) helps the glow read clearly against soft-contrast base masks. **Including the text:** scroll to the rust layer's generator's **Micro Details** section, confirm **Micro Height** is enabled, click its field, go to Anchor Points, and select the **Text_Height** anchor — the recessed lettering now rusts convincingly along with the rest of the surface; AO Radius and related sliders further tune how much rust the text detail picks up. **Hand-painting on top:** because the White_Paint mask sits below the anchor and everything downstream references it live, painting directly into that mask (e.g. painting white to erase rust along an ugly UV seam, or painting black to remove rust from an area entirely) propagates instantly through the entire rust/glow system — fully dynamic at any time. **Dripping rust leaks, confined near existing rust:** duplicate the Rust_Glow layer (to reuse its Roughness/Metallic setup), rename its mask contents "Rust_Leaks," darken its Base Color, then add the **Dripping Rust** generator to it (found by right-clicking to add a generator) — tune **Drip Intensity** and **Rust Spreading**/**Spreading Smoothness** for the desired drip look. Because a raw Dripping Rust generator drips everywhere indiscriminately (including on top of already-rusted areas, which looks wrong), the fix is: create a new **folder** ("Dripping_Rust_Masking"), drag the Rust_Leaks layer into it, add a **black mask to the folder itself** (masks can be applied at the folder level, not just per-layer), add a fill inside referencing the White_Paint anchor (confines drips to only appear near existing rust, not in open unrusted areas), add a strong **Blur filter** (pushed nearly to the point of being unrecognizable) plus a **Levels** adjustment used specifically to **clamp** the blur — dragging the black point removes flat/low-value blurred areas entirely, and dragging the white point tightens the remaining spread — finished with **Invert** so the drips concentrate specifically around, not on top of, the rust. A final **paint layer** on top allows hand-placing extra drips in specific chosen spots, white to add / black to remove, overriding the procedural system exactly where desired.

### Key Steps
1. **Base scene:** bronze base material; a Height-only "Text_Height" fill layer masked with the embossed text detail; a "White_Paint" fill layer (white Base Color, adjustable Roughness) whose black mask uses the **Surface Worn** smart mask to control paint coverage.
2. **Place both Anchor Points early:** add one to the White_Paint mask and one to the Text_Height mask, before starting the rust work.
3. **Add a library Rust material** above White_Paint; tune Rust Color (darker/duller/redder), set UV Transformations Scale (~2), and optionally adjust Cavities.
4. **Confine rust to worn paint:** add a black mask to the rust layer, add a fill inside referencing the White_Paint anchor, and **Invert** it (via Levels) so rust shows where paint has worn away.
5. **Build the rust glow layer:** new plain fill layer ("Rust_Glow") — Metallic on, no Normal needed, low Roughness, strong orange Base Color.
6. **Glow mask, step 1 — placement:** black mask on Rust_Glow, add a fill referencing the White_Paint anchor, **Invert** it.
7. **Glow mask, step 2 — push outward:** add a **Blur filter** on top to spread the orange glow past the mask's hard edge; add a **Levels** adjustment for extra strength control.
8. **Glow mask, step 3 — clip back down:** add a second fill, reference the **same** White_Paint anchor again, **do not invert** this one, and set its blend mode to **Multiply** — this confines the blurred glow to a tight rim rather than bleeding everywhere.
9. **Improve glow contrast:** boost the White_Paint mask's own Contrast (in its Mask Editor) if the glow struggles to read against a soft-contrast base mask.
10. **Include the text detail:** on the rust layer's generator, open **Micro Details**, confirm **Micro Height** is enabled, reference the **Text_Height** anchor through it, then fine-tune with AO Radius and related sliders.
11. **Hand-paint touch-ups directly into the White_Paint mask** (white to erase rust/reveal clean paint, black to remove paint/expose more rust) — changes propagate live through every downstream anchor reference.
12. **Duplicate Rust_Glow to start the leaks layer** (reuses its Roughness/Metallic setup); rename appropriately ("Rust_Leaks"), darken its Base Color.
13. **Add the Dripping Rust generator** to this layer's mask (right-click to add a generator, search/select "Dripping Rust"); tune Drip Intensity and Rust Spreading/Spreading Smoothness.
14. **Confine the drips near existing rust using a folder-level mask:** create a new folder, drag the leaks layer into it, add a **black mask to the folder itself**.
15. Inside the folder's mask: add a fill referencing the White_Paint anchor (confines drips near rust, not open unrusted space), add a strong **Blur filter**, add a **Levels** adjustment to **clamp** the blur (drag the black point to remove flat/low-value blurred zones, the white point to tighten the remaining spread), then **Invert** so drips concentrate around — not on top of — the rust.
16. **Add a final paint layer on top** for hand-placing extra drips in specific spots (white brush to add, black to remove), overriding the procedural placement exactly where wanted.

### Layers / Tools / Settings
- **Text_Height** — Height-only fill layer, mask = embossed text detail, carries its own Anchor Point
- **White_Paint** — white Base Color fill layer, black mask driven by the **Surface Worn** smart mask, carries the primary Anchor Point referenced throughout the rest of the build
- **Rust base layer** — library Rust material (Rust Color, UV Transformations Scale, Cavities); mask = fill referencing White_Paint anchor, **Invert**
- **Rust_Glow** — plain fill layer (Metallic on, no Normal, low Roughness, strong orange Base Color ~`#D6700B`); mask = [fill referencing White_Paint anchor + Invert] → **Blur filter** → **Levels** → [second fill referencing White_Paint anchor, no invert, blend mode **Multiply**]
- **Rust generator's Micro Details:** **Micro Height** enabled, referencing the **Text_Height** anchor; AO Radius and related sliders
- **Rust_Leaks** — duplicated from Rust_Glow (reused Roughness/Metallic), darker Base Color, mask driven by the **Dripping Rust** generator (Drip Intensity, Rust Spreading, Spreading Smoothness)
- **"Dripping_Rust_Masking" folder** — contains Rust_Leaks; **folder-level black mask** = [fill referencing White_Paint anchor] → strong **Blur filter** → **Levels** (used to clamp/clip the blur) → **Invert**
- Final **paint layer** on top for manual drip placement (white add / black remove)
- Confirmed: masks can be applied at the **folder** level, not only per-layer

### Difficulty
Advanced (the series' most complex build — chains generator Micro Height referencing, double-reference invert+blur+Multiply clipping, and folder-level masking into one system; explicitly framed by the video as "a much more complex setup").

### App & Version
Substance 3D Painter. No version number stated on screen; window title bar reads "License: 171 days remaining - Anchor_Video_04_Texture_Begin" (subscription license countdown plus project filename, matching the pattern in series entries 01-03 — not a version indicator).

### Tags
`anchor-point`, `masks`, `layers`, `fill-layer`, `paint-layer`, `generator`, `smart-mask`, `blend-mode`, `height`, `basecolor`, `roughness`, `metallic`, `procedural`, `advanced`

---

## Related Tutorials
- **Anchor Point Magic 01 - Double Layer Setup in Substance 3D Painter** (`tutorials/anchor-point-magic-01---double-layer-setup-in-substance-3d-painter-adobe-substan.md`) — series 1/4, introduces the fundamental anchor-referencing mechanism this finale chains together.
- **Anchor Point Magic 02 - Micro Normals & Micro Height in Substance 3D Painter** (`tutorials/anchor-point-magic-02---micro-normals-micro-height-in-substance-3d-painter-adobe.md`) — series 2/4, teaches the generator Micro Height anchor-referencing technique this video reuses directly to include the text detail in the rust.
- **Anchor Point Magic 03 - Paint Peel Effect in Substance 3D Painter** (`tutorials/anchor-point-magic-03---paint-peel-effect-in-substance-3d-painter-adobe-substanc.md`) — series 3/4, teaches the double-reference invert+blur+Multiply-clip technique this video reuses twice (for the glow, and for the drip-leak confinement).
- **How to TEXTURE like a PRO with ANCHOR POINTS | Substance Painter Tutorial** (`tutorials/how-to-texture-like-a-pro-with-anchor-points-substance-painter-tutorial.md`) — Jared Chavez's independent anchor-point deep-dive; complementary treatment of the same core reuse mechanism this whole series is built on.
- **Creating a Leather Material for Footwear with Anchor Points in Substance 3D Painter** (`tutorials/creating-a-leather-material-for-footwear-with-anchor-points-in-substance-3d-pain.md`) — footwear anchor-points trilogy; explicitly references "the basic anchor point series on this channel" (this exact series) and applies the same generator Micro Height anchor-referencing technique in production.
