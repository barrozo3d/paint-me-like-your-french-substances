---
title: SUBSURFACE SCATTERING: Subsurface Scattering in SUBSTANCE PAINTER for UNREAL ENGINE 5
source: YouTube
url: https://www.youtube.com/watch?v=mjLiJ5yjto0
author: Jared Chavez
ingested: 2026-08-13
app: "Substance 3D Painter"
version: "not specified"
tags: [thickness, masks, generator, curvature, blend-mode, layers, fill-layer, paint-layer, game-engine, unreal-export, export, advanced]
extraction_status: complete
frames_dir: tutorials/frames/subsurface-scattering-subsurface-scattering-in-substance-painter-for-unreal-engi/
frame_count: 10
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# SUBSURFACE SCATTERING: Subsurface Scattering in SUBSTANCE PAINTER for UNREAL ENGINE 5

**Source:** [YouTube](https://www.youtube.com/watch?v=mjLiJ5yjto0)
**Author:** Jared Chavez
**Duration:** 8m22s | 17 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


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

## Captured Frames

- [0:05] tutorials/frames/subsurface-scattering-subsurface-scattering-in-substance-painter-for-unreal-engi/frame_000.jpg
- [1:14] tutorials/frames/subsurface-scattering-subsurface-scattering-in-substance-painter-for-unreal-engi/frame_001.jpg
- [1:38] tutorials/frames/subsurface-scattering-subsurface-scattering-in-substance-painter-for-unreal-engi/frame_002.jpg
- [2:00] tutorials/frames/subsurface-scattering-subsurface-scattering-in-substance-painter-for-unreal-engi/frame_003.jpg
- [2:45] tutorials/frames/subsurface-scattering-subsurface-scattering-in-substance-painter-for-unreal-engi/frame_004.jpg
- [4:03] tutorials/frames/subsurface-scattering-subsurface-scattering-in-substance-painter-for-unreal-engi/frame_005.jpg
- [4:50] tutorials/frames/subsurface-scattering-subsurface-scattering-in-substance-painter-for-unreal-engi/frame_006.jpg
- [5:30] tutorials/frames/subsurface-scattering-subsurface-scattering-in-substance-painter-for-unreal-engi/frame_007.jpg
- [6:08] tutorials/frames/subsurface-scattering-subsurface-scattering-in-substance-painter-for-unreal-engi/frame_008.jpg
- [7:17] tutorials/frames/subsurface-scattering-subsurface-scattering-in-substance-painter-for-unreal-engi/frame_009.jpg

---

## Structured Notes

### Core Technique
Hand-painting a custom **Scattering** user/material channel in Painter (starting from a baked Thickness map as a rough guide, not a literal driver) to art-direct exactly where subsurface light transmission should read as bone-blocked vs. thin/fleshy, then exporting that channel into an Unreal Engine 5 `SubsurfaceProfile` asset for the final render look.

### Summary
Direct follow-up to Chavez's Neomorph creature texturing videos — this one isolates just the subsurface-scattering (SSS) map process he skipped over previously. The creature's Texture Set is named "Neomorph" with a dedicated **Scattering** channel visible in the Texture Set list (frame_002/006/008), painted with a grayscale value system: pure white = maximum light transmission (the top of the skull, his chosen "hero" scattering zone), pure/near black = fully blocked (bony landmarks: ribcage, spine, joints), with grays in between for partial transmission (arms/legs/tail — "more bone than flesh," so darker but not fully black). The workflow deliberately starts from the baked Thickness map as a loose starting point/sanity check (used to preview in Unreal early), then is almost entirely hand-repainted on top because thickness alone produces an undirected, gelatin/candle-like glow with no readable anatomy. The layer stack (visible in frame_002/006/008) is built from multiple named Paint layers per body region (`Stomach`, `Feet`, `Hands`, a spine/ribcage layer, etc.) interleaved with `Levels - Scattering` adjustment layers per region and a `Blur` filter to soften the on/off transitions at region boundaries. Later passes add: a second refinement pass for finer landmarks (tendons), a Curvature-generator layer to concentrate scattering control into edge/detail areas, and localized "fake mass" tricks — e.g. darkening the belly center to suggest solid organs blocking light even though nothing physically exists there to do so ("not 100% physically accurate... but it was able to get the point across"). The final step is iterating the actual `SubsurfaceProfile` asset in Unreal (frame_009: `Neomorph_SSProfile`) — Surface Albedo, Mean Free Path Color/Distance, World Unit Scale, Tint, Boundary Color Bleed, Extinction Scale, Normal Scale, Scattering Distribution, Transmission Tint Color, Dual Specular Roughness 0/1, Lobe Mix — dialing the shader itself to exaggerate scattering further than the painted map alone would produce, described as partly a "lucky" outcome from experimentation rather than a fully deterministic recipe.

### Key Steps
1. Bake/inspect a **Thickness map** as the starting reference for the subsurface layer — accept it will have baking errors in complex areas (this asset had incorrect thickness at the feet); manually paint-fix small baking artifacts directly rather than chasing a perfect bake.
2. Create the initial subsurface layer(s) set to **black** as the base (no scattering by default), then hand-paint value into it — this "secondary subsurface layers" approach treats the SSS map as fully authored, not thickness-derived.
3. Paint black/near-black directly over **bony landmarks** — any area where bone sits close to the surface (ribcage, spine) — to block light transmission there and create a visible bone-vs-flesh read.
4. Do a fast, rough first pass (e.g. just the ribcage) and preview it — validate early that the contrast between "bone" and "skin" areas is reading before investing more painting time.
5. Add a **Blur** filter on top of the painted layer to soften the transition edges between scattering/non-scattering zones — prevents harsh on/off banding artifacts.
6. Export the in-progress bake/paint to **Unreal Engine 5** early and iterate by eye against the real shader response — treat the engine's live material preview as the actual feedback loop, not the Painter viewport alone.
7. Decide on one "hero" maximum-transmission zone per character (here: the top of the skull) and paint that area **pure white** — establishes the top of the value range; everything else is graded down from there in variations of gray/black.
8. Paint **arms, legs, and tail** as a partial-transmission mid-tone (not pure black) — "more bone than flesh" areas get a darker gray that still allows a little light through, distinct from the pure-black bone landmarks.
9. Do a **second refinement pass** adding finer-grained landmarks like tendons — areas that should read as slightly less scattering than surrounding flesh, adding nuance beyond the broad first pass.
10. Layer a **Curvature-generator** on top of the hand-painted base to pull additional scattering detail control into edge/crevice areas, making fine details "pop" in the final SSS read.
11. Add dedicated **custom paint layers for flake/damage skin areas** — retained separately so damaged/thin skin patches can be independently tuned to not read as fully thin/scattering, preserving the flake detail's visual identity in the SSS channel too.
12. Use a **"fake mass" trick** for organs: paint extra black into the center of the belly (and a few other spots) purely to imply something solid is blocking light behind the skin, even though there's no actual geometry driving it — a pure illusion/read-improvement move, explicitly non-physically-accurate but visually convincing from multiple angles.
13. Final step happens outside Painter: dial in the Unreal **SubsurfaceProfile** asset parameters (Surface Albedo, Mean Free Path Color/Distance, World Unit Scale, Tint, Boundary Color Bleed, Extinction Scale, Normal Scale, Scattering Distribution, Transmission Tint Color, Dual Specular Roughness 0/1, Lobe Mix) to push the shader's own scattering response further — the painted map and the shader profile work together, and some of the final look came from experimentally pushing the shader beyond what the map alone implies.

### Layers / Tools / Settings
- Baked **Thickness map** — starting reference only, not the final driver.
- Custom/user **Scattering** channel (Texture Set: "Neomorph") — the channel all subsurface layers paint into.
- Multiple named **Paint layers**, one per body region (seen in frames: `Stomach`, `Feet`, `Hands`, a ribcage/spine layer, plus others for arms/legs) — hand-painted grayscale values, white = max transmission, black = fully blocked.
- `Levels - Scattering` adjustment layers — one per region, refining the black/white/gray range per painted area (`Affected channel: Scattering` visible in frame_004).
- `Blur` filter — softens hard transmission/no-transmission transition edges.
- **Curvature generator** — layered on top for edge/detail-driven scattering control.
- Separate custom paint layers for **flake/damaged-skin** areas — kept independent so damage detail isn't washed out by the broader scattering pass.
- Unreal Engine 5 **SubsurfaceProfile asset** (`Neomorph_SSProfile`) — Surface Albedo, Mean Free Path Color, Mean Free Path Distance, World Unit Scale, Tint, Boundary Color Bleed, Extinction Scale, Normal Scale, Scattering Distribution, Transmission Tint Color, Dual Specular Roughness 0 / Roughness 1, Lobe Mix.

### Difficulty
Advanced — assumes comfort with custom/user channels, multi-layer value painting, and round-tripping a texture between Painter and a live Unreal shader for iterative tuning; not a beginner "toggle Subsurface on" workflow.

### App & Version
Substance 3D Painter (paired with Unreal Engine 5) — version not specified on screen or in narration.

### Tags
thickness, masks, generator, curvature, blend-mode, layers, fill-layer, paint-layer, game-engine, unreal-export, export, advanced

---

## Related Tutorials
- [REALISTIC CREATURES: HAND PAINTED TEXTURES in SUSTANCE PAINTER](realistic-creatures-hand-painted-textures-in-sustance-painter.md) — same creator, same Neomorph creature; this video is the direct SSS-map follow-up the base texturing video explicitly deferred ("I left out the subsurface scattering portion").
- [How to TEXTURE in SUBSTANCE PAINTER | Creature TEXTURING](how-to-texture-in-substance-painter-creature-texturing.md) — same creator; shares the same hand-painted-value-zones-over-anatomy methodology (there: color zones for bone/fat/cavities; here: grayscale zones for light transmission).
- [How to TEXTURE in SUBSTANCE PAINTER | ORC TEXTURES](how-to-texture-in-substance-painter-orc-textures.md) — same creator; shares the same subdermal-first skin methodology and multi-frequency detail-layering approach, applied there to color/discoloration rather than a light-transmission channel.
- [How to make HAND PAINTED SKIN Textures in SUBSTANCE PAINTER](how-to-make-hand-painted-skin-textures-in-substance-painter.md) — same creator; the Subdermal-group-first mental model there (blood/bone color beneath the surface) is the direct color-channel counterpart to this video's grayscale light-transmission channel — both built on "author what's happening underneath the skin first."
- [HOW TO MASTER TEXTURing in SUBSTANCE PAINTER](how-to-master-texturing-in-substance-painter.md) — same creator; conceptual companion — the "fake mass" belly trick here is a concrete example of that video's Phase 3 "embellishing reality for readability" philosophy applied to a non-color channel.
- [Substance Painter Beginner Tutorial for Unreal Engine 5](substance-painter-beginner-tutorial-for-unreal-engine-5.md) (Unreal Sensei) — different creator; broader Painter-to-UE5 pipeline coverage including multi-texture-set blending and Nanite export, useful context for the export side of this video's Unreal round-trip.
- [Optimizing Textures - How to Pack Masks Like a Pro](optimizing-textures---how-to-pack-masks-like-a-pro.md) (Abe Leal 3D) — different creator; shares the "author a custom User Channel in Painter, then reconstruct/consume it via a dedicated Unreal material asset" pattern (there: a packed "blood" channel driving a Material Instance parameter; here: a "Scattering" channel driving a SubsurfaceProfile asset).
