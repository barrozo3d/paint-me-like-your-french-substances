---
title: Create Trim Sheets in Substance 3D Painter - Part2 | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=QoVWM-IKmFw
author: Adobe Substance 3D
ingested: 2026-08-13
app: "Substance 3D Painter (texturing) + Unreal Engine (final in-scene showcase) + 3ds Max (UV unwrap of dependent assets)"
version: "not stated on screen; UI (Smart Materials library, anchor-point-referencing Micro Normal/Micro Height in generator settings, pass-through filter trick, Extract Alpha behavior) matches a modern Painter release, not precisely pinnable"
tags: [layers, fill-layer, masks, generator, anchor-point, smart-material, blend-mode, curvature, ambient-occlusion, pbr, metal-rough, basecolor, roughness, metallic, height, normal-map, opacity, alpha, procedural, uv, game-engine, unreal-export, advanced]
extraction_status: complete
frames_dir: tutorials/frames/create-trim-sheets-in-substance-3d-painter---part2-adobe-substance-3d/
frame_count: 8
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Create Trim Sheets in Substance 3D Painter - Part2 | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=QoVWM-IKmFw)
**Author:** Adobe Substance 3D
**Duration:** 18m50s | 15 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### <Untitled Chapter 1> [0:00]
**Transcript (timestamped):**
[0:00] In our last video, we went over on what trimsheets are and we went ahead and created our initial
[0:14] ID mask and our non-map details.
[0:17] And now in this chapter, we will go ahead and we will finish off our trim sheet over
[0:21] here and I will show you how it is actually used in a 3D environment.
[0:26] Now at this point, we can turn off our color ID, we no longer need it.
[0:31] And we are going to go ahead and create our base colors in a few stages.


### Base Colors [0:32]
**Transcript (timestamped):**
[0:35] First of all, our base colors, the second one is going to be polished on our base colors
[0:40] and the third one is going to be improving our overall textures.
[0:44] So for our base colors, we are going to keep this nice and simple because I want to go
[0:47] ahead and get quite a clean effect.
[0:50] So it's mostly just going to be metal with some slight roughness variation to it.
[0:56] I want to go ahead and I want to go to my smart materials over here.


### Smart Materials [0:57]
**Transcript (timestamped):**
[1:01] And then if you scroll down, you will very often see a bunch of steel materials.


### Steel Materials [1:04]
**Transcript (timestamped):**
[1:06] Now the one that I want to use is I think some clear coat materials, which are nice and shiny,
[1:11] will work quite well.
[1:12] I'm just going to go ahead and drag this one above our non-map details over here.
[1:18] And I will call this base steel.


### Steel [1:19]
**Transcript (timestamped):**
[1:21] Now we are first just going to focus on having one overall steel that works well.
[1:25] And then we will go ahead and add some color variations.
[1:29] The one that you want is you want to go into your coating over here.
[1:32] And right now the coating has like a metal edge where, but I'm just going to go ahead
[1:36] and turn this off.
[1:38] And I'm going to set my coating mask over here to a white mask so that we are only using our coating.
[1:44] We still want to keep the metal below it because it does have some effects.
[1:48] Now you want to go to your under paint and we can basically just say, let's go for like a
[1:55] little bit of like a lighter metallic paint.
[1:59] Let's start with something quite light, something like this, and maybe make it a little bit of
[2:03] like a bluish tone over here, something like this.
[2:07] Now next what I want to do is I'm now going to switch to my 3D view.
[2:10] And you can already see that I have some pretty interesting roughness over here.


### Roughness [2:11]
**Transcript (timestamped):**
[2:14] We can control this roughness one by going into our finish rough under our metal.
[2:19] And in here we can play around with our brushing intensity as you can see over here.
[2:24] And we can also play around with the overall scale of our roughness.
[2:27] I want to set my scale quite low and my brushing intensity also quite low.
[2:32] Next I'm just going to go to my clear coat and your clear coat actually controls most


### Clear Coat [2:33]
**Transcript (timestamped):**
[2:36] of your roughness.
[2:38] What I'm going to do is I'm going to tone this a little bit down over here.
[2:41] And I think that this is already like a pretty solid base for our mesh.
[2:46] Now what we can do is we can actually use the mask in our clear coat to create different colors.
[2:52] Because of course some of this metal is really light, some of this metal is darker.
[2:57] So I just want to create a few different color variations of this.
[3:02] I can do this and first of all what you can do is we can actually get rid of the dust
[3:05] because it is a plane.
[3:07] When we have a plane many of these generators will not work.
[3:10] But then in our coating I can go ahead and call this gray metal over here.
[3:18] And now we can go ahead and get started by masking over here which pieces we want to have
[3:23] this gray metal on.
[3:24] So I'm just going to add a simple fill layer.
[3:27] Go to my gray scale and anchor points and now we can select the anchor points just like we
[3:32] did before.
[3:33] So our base metal I want to go ahead and have this base.
[3:36] I want to go ahead and now add another fill layer.
[3:39] And this time for this one I want to select for example my random details over here.
[3:44] And then all you need to do is you need to go and set the mode from normal to art,
[3:49] linear dutch art.
[3:50] And that will just add these pieces together.
[3:52] Now let's say that I also want to go ahead and add another fill.
[3:56] And this one is going to be our floor panel.
[3:59] I think that one we can also use as a base and just add it.
[4:04] And yeah so we do have quite a bit of fill layers but it does make everything nice and
[4:08] non-destructive.
[4:09] Now I want to have my wall panels to be a different color.
[4:13] So all I want to do now is I just want to have my line over here.
[4:17] And that is probably the last one that I want to art.
[4:20] So we can go ahead and set this to art and there we go.
[4:23] Then next I can simply go ahead and duplicate our clear coat and I can call this light
[4:30] metal.
[4:32] And then for example just go ahead and get rid of these fill layers except for maybe the last one.
[4:36] Go to your under paint and let's set this one to be a little bit lighter.
[4:41] And then finally in your fill layer you just want to go ahead and select for example this
[4:46] is going to be our wall panel mask.
[4:48] So we want to make this one a bit lighter and let's add another fill layer.
[4:52] And this one is going to be our console mask over here.
[4:57] And once again we can add this.
[5:01] Next this I actually also in my gray metal want to add my decals.
[5:05] So let's add one more fill anchor points, decals and let's art over here.
[5:12] And then now that this is done what we can do is we can go ahead and grab for example some steel.
[5:17] So we can just drag this steel in over here.
[5:20] And then we can once again add a black mask to this.
[5:25] Add a fill layer and I want to use my floor for the steel just like that.
[5:31] And then we also need a little bit of a rubber.
[5:33] So we can just type in rubber and then we can often find maybe some plastic or some
[5:38] rubber or something like that.
[5:39] Let's do plastic armor simple just to keep things nice and easy.
[5:45] Add another black mask.
[5:47] Add another fill and then you can go ahead and in your anchor points I'm going to use the
[5:52] cable for this one.
[5:54] And by the way in my steel I want to make sure that my steel is also including
[5:59] the gears that I have.
[6:01] So add a fill anchor point gears and art just like that.
[6:07] Okay so now we have like a few base metals.
[6:09] Now of course what you want to do is you want to go ahead and in your base steel
[6:14] we want to make sure that all of these fills that we used are included in here.
[6:21] So that we can mask them out.
[6:22] This is as simple as just adding a quick anchor point to these two metals over here.
[6:28] And then in our base steel we can add a simple black mask and just the same thing over again
[6:33] we add a fill and sorry not the base metal mask.
[6:37] This one is going to be our gray metal over here and then we can go ahead and we can add
[6:45] another fill and this one we can set to art and this is going to be our light metal over here.
[6:53] And then over here in our steel I accidentally set this to the wrong mask so I want to set this to
[6:57] my event mask over here.
[7:00] Okay so we now have everything properly divided up in the way that we wanted to.
[7:04] And now that we have our base colors to keep things nice and organized and also to fix our
[7:08] normals we can create a folder called base colors and then when we add these maps over here
[7:15] because now it is reading the folder it will no longer overwrite the normals because the
[7:20] folder settings are set to basically combine all of the normals.
[7:24] So we now have our base colors over here.
[7:26] The only problem that we have now is that we are missing our cutout as you can see over here.
[7:32] We can fix this by going into our steel which is the one that has the cutout
[7:36] and if we just go to our base we just want to turn off the opacity setting so that now we have a cutout.
[7:42] Next to this I would also like to create a cutout on this mesh over here because I do not


### Create a Cut Out [7:43]
**Transcript (timestamped):**
[7:48] want to have a background when I add these details to my plane as if they were decals.
[7:54] This is once again not too difficult all we need to do is go down to our norm map details
[7:59] and then if we have our normal details over here we can add a nice anchor point
[8:05] and then let's you know what throw this all into a folder.
[8:09] Normal details which allows us to also immediately mask the anchor point.
[8:14] So let's go ahead and add a black mask to this along with a fill layer and this fill layer you
[8:21] want to select the actual random details not the normal details but like just the color that we
[8:27] assigned to this section because then all we need to do is we need to throw a fill layer inside of
[8:33] our normal details turn everything off except for the opacity and let's set the opacity to black
[8:40] call this cutout and then you guessed it black mask fill layer and assign your normal details in here.
[8:49] It can be a little bit confusing because we work so much with different fill layers
[8:54] but you will get used to it. Make sure that if you're doing this in your reference channel set this
[9:00] to your opacity press invert and then you just want to set the alpha behavior to extract alpha
[9:07] and now as you can see it has nicely cut out these shapes so we can use them on our decals.
[9:13] Okay awesome so we got this stuff done I would say that the last one that I want to do is I
[9:19] probably want to give like a darker metal to this area over here and once again this is something
[9:25] that I can just very quickly do so let me just very quickly time lapse it.
[9:37] Okay here we go now I would say one last thing that I'm going to do is I'm already going to
[9:53] quickly balance out my steel and I'm going to get rid of the surface details over here
[9:58] and maybe in my base steel I'm going to set my roughness a little bit lower and maybe the color
[10:03] a little bit lighter. I'm not going to go over like the actual polishing too much because that would
[10:09] feel a little bit overkill but just in general you can go ahead and play around with things
[10:14] however you want to get exactly the materials that you want. Now what we can do is we can go
[10:19] ahead and we can add some very simple decals we can simply go up here create a folder that's called


### Decals [10:25]
**Transcript (timestamped):**
[10:25] decals and when I say decals I mostly mean text. For this one what you want to do is it's mostly
[10:31] fill layers let's call this one text let's make the color a little bit whiter let's make the roughness
[10:38] quite dull and make sure that metallic is set to black and with this text what we can do is we can
[10:44] go ahead and we can add a black mask and then in this black mask you can do this even easier like
[10:51] instead of doing like a projection you can even go in here and there are a bunch of text decals as
[10:56] you can see here that I can use so let's say that I want to use for example artrized personnel only
[11:04] I can set my brush quite large and then you can see that it will already show
[11:08] my mask so there are many ways that you can do this or you can go ahead and do this
[11:12] or you can and then just simply oh it's auto saving and then you can simply stamp it as you can see
[11:19] or what you can do is you can still use your projection and then it is just a matter of
[11:23] scrolling down and let's say that we want to go ahead and grab the word danger we can go in here
[11:29] and you basically just like nicely want to add these so I will just go ahead and like add a few
[11:34] of these here we go so I added two versions I added some orange text which has this one
[11:40] and I just went ahead and added some normal text over here now of course this is all very perfect
[11:46] so let's break it up a bit that's going to be quite easy just in our decals folder let's go
[11:51] add an art a black mask to this let's add a fill layer and then you can find like a nice crunch
[11:57] map in your textures that you can use for example up here we have like a lot of them so let's say
[12:02] that we are going to use for example this one the crunch charcoal we want to add this one in here
[12:09] and then you can see that already adds like a little bit of damage over here if you want you
[12:14] can also combine these crunches so you can play around with your balance here to add more or less
[12:19] and then let's say that you want to add another fill layer and for this one I'm going to grab for


### Fill Layer [12:20]
**Transcript (timestamped):**
[12:24] example my crunch concrete over here or maybe want to go ahead and crunch concrete like dirty or old
[12:33] you can do various ones here let's do old and then just play around with your balance and contrast
[12:39] to get some slight damaged areas on your text okay so now that this is done what I want to do
[12:50] is I want to go ahead and start adding some dirt and some edge highlights to improve our material
[12:55] even more now for this what we need to do is we need to create a special anchor point and this


### Anchor Point [12:58]
**Transcript (timestamped):**
[13:00] anchor point will basically combine all of our norm map details and all of our height map details
[13:04] into one anchor point and then what we can do is we can reference this later on in our dirt now
[13:11] for this we want to go ahead and go to our norm map details over here in the folder and this is why
[13:16] it is so important to have this folder below our base colors and now there is a little trick that
[13:22] you can use so if you go ahead you can go up here to filters if you just add any filter doesn't matter
[13:29] what it will do is it will create a filter that is already set to pass through and then you can
[13:34] just close this so instead of going over here and adding a paint layer setting this to pass through
[13:39] on every single channel that is quite annoying so adding a filter is a shortcut and we can call this
[13:46] one uh let's call this one master anchor now all you need to do here is you need to go ahead and
[13:54] add a anchor point to this very base just like that and now it will reference everything that is
[13:59] below it which is all of these norm map details finally if we just go ahead and let's place this
[14:07] in our base steel because i do not want dirt to be affecting our clean steel i can go up here and
[14:13] let's create a nice folder that we will call dirt and in here i'm going to start with like a fill layer
[14:20] and call this occ underscore dirt so let's add some occlusion dirt let's set our roughness
[14:26] quite low let's give it like a little bit of like a brownish color over here just like that and then
[14:33] if you want you can turn off the height normal and opacity now next what we can do is we can add a


### Black Mask [14:38]
**Transcript (timestamped):**
[14:39] black mask this and we can use a smart material for example let's go ahead and scroll down and
[14:44] let's use this sharp dirt over here submit a bit and now what we can do is if we go into our dirt
[14:53] we need to scroll down to our micro normal and micro height and in here you want to reference
[14:59] your master anchor now after you've done this make sure that on your normal you set your referenced
[15:06] channel to be your normal channel and on your height for it to be your height channel next if
[15:12] you scroll up to the micro details tab all you have to do is turn this one on and then you can see


### Micro Details [15:13]
**Transcript (timestamped):**
[15:17] that it will generate our dirt in here you can play around a bit with for example your AO radius
[15:24] to get more or less dirt and also your height detail intensity and next this you can of course
[15:30] also play around with for example your dirt levels and let's tone down our contrast a little bit
[15:36] like this and now let's just go ahead and say i want to make like my dirt a little bit lighter
[15:42] and a little bit more subtle something like this and the same works for edge highlights let's say


### Edge Highlights [15:46]
**Transcript (timestamped):**
[15:47] that we want to go ahead and add another fill layer edge highlights over here what we can do
[15:54] is we can make this for example like quite bright and then in our roughness we probably want to go
[16:02] ahead and tone this down a little bit and for the rest we can turn off everything else we only
[16:07] will need these two versions over here now we can go ahead and we can add a black mask and this
[16:13] time instead of a spark material i'm just going to add a generator up here and i just want to add
[16:19] a curvature generator because i just want to get some soft highlights we go ahead and zoom in again
[16:25] you want to go ahead and turn on your micro details micro normal reference your master anchor and
[16:32] micro height reference your master anchor and don't forget to set the correct reference channel
[16:38] normal and height over here and now you can immediately see that we get some nice highlights
[16:44] you can go ahead and of course play around with your global balance to get more or less out of it
[16:49] and what i like to do is i often like to go up here to the opacity of my curvature and use that
[16:55] to basically control everything a little bit and just like that we now have some extra dirt added
[17:01] now there's a bunch more polishing that you can do you can balance out the metal and everything
[17:05] you can add some roughness variation add some more specific dirt and details and all that kind of
[17:10] stuff but this is something that i will simply do off camera because else this tutorial would be very
[17:16] long so what i want to do now is i'm going to show you how that we actually use this trim sheet how


### Uv Unwrap [17:22]
**Transcript (timestamped):**
[17:22] we UV unwrap the models and how that we use it in our level it's just going to be a nice little bonus
[17:28] okay so here we are in 3s max now as you can see here i have the pillar you can see that the pillar
[17:33] is mostly made out of metal and then i simply added planes that have for example those norm
[17:39] map details on here now if we would go ahead and open up the UVs of our pillar you can see that it
[17:45] has just been strategically broken up in a way that it all fits in our metal sometimes literally
[17:51] sometimes literally by adding extra lines in between here and then what we do is we use these
[17:56] construction lines which you cannot see right now but those are the construction lines that we created
[18:02] to basically hide some of these seams and we have used these same techniques also on our other assets
[18:09] so if we would for example go ahead and go to unveil and as you can see here is our scene it is
[18:14] a fully real time scene here is our pillar and you can see that it works great when we actually
[18:19] cut out these meshes using our material inside of a wheel we use the exact same material also
[18:24] over here on our window pieces we used it on our floor here you can see our floor details it's a
[18:30] little bit dark but you can see it and over here you can also see it on our wall details and all
[18:36] with all it will create a nice scene so that was it for this quick tutorial series i hope that you
[18:42] learned something from it and i hope to see you next time



---

## Captured Frames

- [1:12] tutorials/frames/create-trim-sheets-in-substance-3d-painter---part2-adobe-substance-3d/frame_000.jpg
- [2:20] tutorials/frames/create-trim-sheets-in-substance-3d-painter---part2-adobe-substance-3d/frame_001.jpg
- [5:20] tutorials/frames/create-trim-sheets-in-substance-3d-painter---part2-adobe-substance-3d/frame_002.jpg
- [7:50] tutorials/frames/create-trim-sheets-in-substance-3d-painter---part2-adobe-substance-3d/frame_003.jpg
- [10:56] tutorials/frames/create-trim-sheets-in-substance-3d-painter---part2-adobe-substance-3d/frame_004.jpg
- [13:46] tutorials/frames/create-trim-sheets-in-substance-3d-painter---part2-adobe-substance-3d/frame_005.jpg
- [15:17] tutorials/frames/create-trim-sheets-in-substance-3d-painter---part2-adobe-substance-3d/frame_006.jpg
- [18:14] tutorials/frames/create-trim-sheets-in-substance-3d-painter---part2-adobe-substance-3d/frame_007.jpg

---

## Structured Notes

### Core Technique
Finishing the trim sheet's base-color pass entirely with anchor-point-referenced fill layers (every color zone masked by referencing the Part 1 Color-ID anchor points, never repainted by hand), building a proper alpha cutout for decal-style reuse, adding text decals and procedural dirt/edge-wear via a single "master anchor" that combines all normal/height detail into one reusable reference, then showing the finished trim sheet applied across a full sci-fi corridor level in Unreal Engine (UVs unwrapped in 3ds Max).

### Summary
Part 2/2 of Adobe's Create Trim Sheets series, picking up immediately after Part 1's Color ID map and normal/height detail work. Base color construction: starts from a Smart Material (a Steel/Clear Coat material family) dragged above the normal-detail layers and renamed "Base Steel" — disables the coating's built-in metal-edge-wear mask (set to plain white so only the coating shows), tunes the underpaint to a light bluish metallic tone, and controls roughness via both the metal's "Finish Rough" (brushing intensity + scale) and the Clear Coat amount (which drives most of the perceived roughness). Color variation zones are built as separate materials (e.g. "Gray Metal", "Light Metal") each masked by one-or-more fill layers whose masks reference specific Part-1 Color-ID Anchor Points (Base Metal, random details, floor panel, wall line, console, decals, gears, cable, etc.), combined with the **Add (Linear Dodge)** blend mode so multiple anchor-referenced fills stack into one mask; a duplicate anchor point is added to each new base-color material so that a later "Base Steel" layer can itself reference and exclude those zones via its own black mask. All these are organized into a **Base Colors** folder set to combine/pass-through normals so the folder doesn't overwrite the normal-detail layers below it. Cutout/decal-readiness: enabling the shader's built-in Opacity-based cutout on the steel material, then building a dedicated cutout pass in the Normal Details folder — an anchor point on the relevant Color-ID zone, a fill layer with only Opacity enabled (set to black) named "Cutout", masked by a fill layer referencing the normal-detail anchor with its reference channel set to Opacity, Invert checked, and Alpha Behavior set to **Extract Alpha** — producing a clean per-shape cutout so the normal-detail panels can be placed on a plane and used as real decal geometry, matching Part 1's stated Unreal Engine decal use case. Decals: a **Decals** folder with a "Text" fill layer (white-ish, dull roughness, black metallic) masked either by stamping Painter's built-in text-decal alphas (warning/caution words like AUTHORIZED PERSONNEL ONLY, DANGER, KEEP OUT, OPEN, LOCK SECTION, CONTROL ROOM AREA) directly with a large brush, or by projecting them; then breaking up the decals' crispness with grunge-map fill layers (Crunch Charcoal, Crunch Concrete Dirty/Old) for wear variation. Dirt/edge-highlight finishing: creates a **Master Anchor** by adding any filter (set to pass-through) at the base of the Normal Details folder and dropping an anchor point on it — a shortcut vs. manually pass-through-ing a paint layer on every channel — which then combines every normal-map and height-map detail layer below it into one referenceable anchor. Placed inside Base Steel (so dirt doesn't affect the clean steel elsewhere), a new **Dirt** folder holds: an Occlusion Dirt fill layer (low roughness, brownish tint, Height/Normal/Opacity off) masked by the **Sharp Dirt** Smart Material, whose Micro Normal and Micro Height reference channels are pointed at the Master Anchor (Normal reference channel = Normal, Height reference channel = Height) with Micro Details enabled — exposing AO Radius and Height Detail Intensity controls, plus a Levels adjustment to tone down dirt contrast/opacity for subtlety; and an Edge Highlights fill layer (bright color, lowered roughness, only Base Color + Roughness on) masked by a **Curvature** generator with the same Master-Anchor Micro Normal/Micro Height referencing, whose own Opacity slider is used as the primary intensity control. Final section switches to 3ds Max to show the trim sheet's UV unwrap on a pillar asset (strategically split so segments map onto matching trim regions, sometimes adding extra geometry cuts purely to align UVs, with Part 1's construction lines used to visually hide seams) and then to Unreal Engine, where the same single trim-sheet material is shown driving pillars, cutout window/decal meshes, floor, and wall details across a fully real-time corridor scene.

### Key Steps
1. Turn off/hide the Color ID folder from Part 1 — no longer needed once base-color work begins.
2. Base steel: open the Smart Materials shelf, find a Steel/Clear Coat family material, drag it in above the Normal Details layers, rename to **Base Steel**.
3. In the Coating sub-layer: disable the built-in metal-edge-wear effect and set its mask to plain white so only the coating renders; keep the underlying Metal layer active for its contribution.
4. In Under Paint: pick a light, slightly bluish metallic base tone.
5. Tune roughness in two places: **Finish Rough** under Metal (Brushing Intensity + Scale, both set low here) and the **Clear Coat** amount (which dominates overall perceived roughness) — reduce Clear Coat somewhat for a cleaner base.
6. Build color-variation materials (e.g. "Gray Metal", "Light Metal") the same way — duplicate/adjust Base Steel, then mask each with one or more fill layers whose masks are set via **Anchor Points → [Color-ID zone]** (Base Metal, random details, floor panel, wall line/console/decals/gears/cable, etc.); when combining multiple anchor-referenced masks into one, set additional fill layers' blend mode to **Add (Linear Dodge)** so they union together instead of replacing.
7. Add a fresh Anchor Point to each new color-variation material (Gray Metal, Light Metal) so the top-level Base Steel layer can later mask them out of its own coverage.
8. On Base Steel itself, add a black mask, then add fill layers referencing the Gray Metal and Light Metal anchors (Add blend mode) to exclude those zones from the plain base steel, plus fix any zone accidentally masked to the wrong anchor (video catches and corrects a vent-mask mistake this way).
9. Organize into a **Base Colors** folder; set the folder's blend/pass settings so normals combine rather than get overwritten by the folder — keeps normal-detail layers underneath intact.
10. Fix the missing cutout: on the Steel material's Base sub-layer, disable the Opacity toggle so the shader's Alpha-Test cutout actually takes effect.
11. Build the decal-ready cutout: in Normal Details, add an Anchor Point to the relevant Color-ID zone; wrap Normal Details in its own folder (enables immediate anchor+mask referencing); add a black mask + fill layer referencing the raw color-zone anchor (not the normal-detail anchor); inside that, add another fill layer with every channel off except Opacity (set to black), name it **Cutout**; mask it with a fill layer referencing the Normal Details anchor, with **Reference Channel = Opacity**, **Invert** checked, and **Alpha Behavior = Extract Alpha** — this cleanly cuts the shape so it can be used as decal geometry on a plane.
12. Decals folder: new "Text" fill layer — near-white Base Color, dull Roughness, Metallic = black. Mask it either by directly stamping Painter's built-in text/warning-sign decal library brushes (large brush size) or by projecting them, placing multiple decal words/labels around the trim sheet.
13. Break up decal crispness: add a black mask + fill layer using a Grunge map (e.g. Crunch Charcoal, Crunch Concrete Dirty/Old) over the decals, tuning Balance/Contrast for partial wear.
14. Build the **Master Anchor**: at the base of the Normal Details folder, add any filter (its default is pass-through) purely as a shortcut to avoid manually setting a paint layer to pass-through on every channel; add an Anchor Point to this filter layer and name it (e.g. "Master Anchor") — it now represents the combined result of every normal-map and height-map detail layer beneath it in the stack.
15. Place a new **Dirt** folder inside Base Steel (so dirt only affects the base steel zones, not other color-variant materials) containing: an **Occlusion Dirt** fill layer (low Roughness, brownish tint, Height/Normal/Opacity channels off) masked by the **Sharp Dirt** Smart Material.
16. On the Sharp Dirt mask's generator settings, scroll to **Micro Normal** and **Micro Height**: reference the Master Anchor for both, and set Reference Channel = Normal (for Micro Normal) and Reference Channel = Height (for Micro Height); enable **Micro Details** to activate the effect — exposes AO Radius and Height Detail Intensity sliders to tune how much dirt appears and where. Use a Levels adjustment on the dirt layer to tone down contrast/opacity for subtlety.
17. Add an **Edge Highlights** fill layer (bright Base Color, reduced Roughness, only Base Color + Roughness channels on) masked by a **Curvature** generator, again referencing the Master Anchor for Micro Normal/Micro Height with the same Normal/Height reference-channel settings — produces soft edge-wear highlights. Use the Curvature layer's own Opacity slider as the main intensity control for the whole effect.
18. Further polishing (metal balance, extra roughness variation, more localized dirt/detail) is left as an off-camera exercise — not shown step by step.
19. Switch to 3ds Max: inspect the UV layout of a corridor pillar asset built mostly from the trim-sheet metal, showing the mesh strategically segmented (sometimes with extra geometry cuts purely for UV alignment) so each piece maps onto the correct trim region; Part 1's construction lines are used specifically to visually disguise these UV seams.
20. Switch to Unreal Engine: shows the same single trim-sheet material driving the pillar, cutout window/decal meshes (using the Extract-Alpha cutout built above), floor details, and wall details across one fully real-time sci-fi corridor scene — the payoff of building everything from one shared texture.

### Layers / Tools / Settings
- **Smart Materials shelf**: Steel/Clear Coat family material as the Base Steel starting point.
- **Base Steel material sublayers**: Coating (metal-edge-wear disabled, white mask), Metal/Under Paint (light bluish tone), Finish Rough (Brushing Intensity, Scale), Clear Coat (roughness-dominant amount slider).
- **Anchor-Point-referenced fill layers**: the core masking mechanism throughout — every color-variation zone is masked by one or more fill layers set to a specific Part-1 Color-ID Anchor Point, several combined via **Add (Linear Dodge)** blend mode.
- **Base Colors folder**: groups all base-color layers; configured so normals combine/pass through rather than being overwritten.
- **Cutout construction**: Opacity channel toggle on the Steel base sublayer; dedicated "Cutout" fill layer (Opacity-only, black) masked via a fill layer with Reference Channel = Opacity, Invert on, Alpha Behavior = **Extract Alpha**.
- **Decals folder**: Text fill layer (Base Color near-white, Roughness dull, Metallic black) masked by built-in text/warning decal brushes or projection; Grunge-map fill layers (Crunch Charcoal, Crunch Concrete Dirty/Old) for wear breakup.
- **Master Anchor**: a pass-through filter (any filter, default pass-through behavior) at the base of the Normal Details folder, carrying an Anchor Point that represents the combined normal+height result of every layer beneath it — the key reusable reference for downstream dirt/wear effects.
- **Dirt folder** (inside Base Steel): Occlusion Dirt fill layer masked by the **Sharp Dirt** Smart Material, whose generator exposes **Micro Normal** / **Micro Height** reference-channel fields (both pointed at Master Anchor, Reference Channel = Normal / Height respectively) and a **Micro Details** enable toggle (AO Radius, Height Detail Intensity sliders); Levels adjustment for contrast/opacity taming.
- **Edge Highlights fill layer**: masked by a **Curvature** generator, same Master-Anchor Micro Normal/Micro Height referencing pattern; layer/generator Opacity slider used as the master intensity dial.
- **3ds Max**: UV unwrap inspection of a trim-sheet-driven pillar asset.
- **Unreal Engine**: final real-time corridor scene using the finished trim-sheet material across pillars, cutout decal meshes, floor, and wall assets.

### Difficulty
Advanced/Expert (deep anchor-point-referencing masking system, Micro Normal/Micro Height generator referencing, cutout/Extract-Alpha decal construction, cross-app UV+engine payoff).

### App & Version
Substance 3D Painter (texturing), 3ds Max (UV unwrap inspection), Unreal Engine (final real-time scene, confirmed as Unreal Engine 5 per Part 1's closing note and this video's visible modern Unreal editor UI). No Painter version number is stated on screen; the feature set (Smart Materials, Micro Normal/Micro Height reference-channel fields in generator settings, Extract Alpha behavior, pass-through filter trick) is consistent with a modern Painter release but not precisely pinnable to a single point version.

### Tags
`layers`, `fill-layer`, `masks`, `generator`, `anchor-point`, `smart-material`, `blend-mode`, `curvature`, `ambient-occlusion`, `pbr`, `metal-rough`, `basecolor`, `roughness`, `metallic`, `height`, `normal-map`, `opacity`, `alpha`, `procedural`, `uv`, `game-engine`, `unreal-export`, `advanced`

---

## Related Tutorials
- **Create Trim Sheets in Substance 3D Painter - Part 1** (`tutorials/create-trim-sheets-in-substance-3d-painter---part-1-adobe-substance-3d.md`) — direct prerequisite: builds the Color ID map, per-mask Anchor Points, and normal/height detail layers this video's base-color and dirt/wear passes reference throughout.
- **Creating Trim Sheet UVs for Substance 3D Painter** (`tutorials/creating-trim-sheet-uvs-for-substance-3d-painter-adobe-substance-3d.md`) — same broader Adobe trim-sheet series; covers the same 3ds Max UV-unwrap process shown briefly at the end of this video, in much greater depth.
