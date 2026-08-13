---
title: Realistic Texturing Tips in Substance Painter
source: YouTube
url: https://www.youtube.com/watch?v=_qirDRMN1WI
author: FastTrack Tutorials
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/realistic-texturing-tips-in-substance-painter/
frame_count: 0
frame_status: pending-selection
---

# Realistic Texturing Tips in Substance Painter

**Source:** [YouTube](https://www.youtube.com/watch?v=_qirDRMN1WI)
**Author:** FastTrack Tutorials
**Duration:** 20m39s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py realistic-texturing-tips-in-substance-painter <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hi everybody, thank you for watching Fast Track Tutorials, my name is Sam. Today we're
[0:06] going to be going over five quick tips as far as texturing goes that I used to texture
[0:13] this pot. We're going to be using Substance Painter. Tip one is going to be creating a
[0:21] metal base material. So I've gone ahead and hidden all the other layers and the ones,
[0:31] the layers in red are the ones we want to focus on. Firstly, noise roughness, this is
[0:39] the kind of look we want to achieve. If we go into the roughness map we can see the small
[0:45] dots which are really going to, as you can see here, give the material a nice pop that
[0:54] you really want to have in your materials. So this is really simple. All I did was add
[1:02] a dirt three map. I tiled it up to about 14. These are rough measurements by the way.
[1:08] So any, you can really just go by eye at this point in whatever looks good to your eye.
[1:17] You should go with. The next thing I did was adjust the roughness. So I brought it down
[1:27] to 0.21. Again, it's just a per eye basis. You know, each person's opinion is different.
[1:37] But one thing you want to make sure you do is go to the roughness tab here and it starts
[1:46] off at normal and you want to change the blend mode to overlay. What this is going to do
[1:53] is just make it more visible throughout each layer you stack on top. The more layers you
[2:00] put on, the more you will notice whether or not you have overlay on. The next layer we're
[2:07] going to want to add to our base material is basically the same thing, but we want to
[2:13] just hit seed so it's not exactly over hovering over your roughness and we are going to change
[2:22] to color. So it is basically the color equivalent to what I just added to that noise. If we
[2:28] go to roughness, you can see this is what we did previously. And then base color, it
[2:35] is basically the same thing. So you put it on instead of going into the roughness tab,
[2:40] go into overlay. It doesn't really matter what you have here. We just want base color
[2:47] overlay, same type of thing. And you adjust it just until you can kind of see it. You
[2:54] know, it's a case by case basis. If you're texturing this for close ups, you know, maybe
[2:59] you want it to be a little bit more subtle as opposed to if you're putting this into
[3:07] say Unreal Engine and it's going to sit on a shelf and you're only going to be able to
[3:11] see it from, you know, 20 feet away. In that case, scaling this up is going to add that
[3:18] detail that you'll be able to see from a bit further away. The next layer we're going
[3:24] to add is the directional height. So this is what it looks like. This is a pretty simple
[3:32] layer. Basically, the way I achieved this was if I'm going to hide all these right here,
[3:39] we start out with directional scratches here. So you can find this right in the search bar
[3:46] here. All these maps I've used, by the way, are just base substance painter maps. So they're
[3:51] easy to find. And you can really achieve a lot with just using substance painter default
[4:00] maps. So directional scratches. I'm going to throw this in here. As you can see, I've
[4:06] tweaked the parameters a little bit, so feel free to copy exactly. But this is another,
[4:12] you know, it's never, real world stuff is never, you know, one certain parameter. It's
[4:18] just kind of a variation. So don't feel like you have to copy exactly what I'm doing. Dirt
[4:25] scratchy grunge layer has been added here. And we've put it onto a subtraction method.
[4:33] So if we change it, this is kind of what it's looking like. I've tiled it up to about four.
[4:43] And we want to change it back to subtract right here, subtract. So as you can see, all
[4:52] it's done is taken this map and subtracted this map from it. It just gives it that real
[5:00] world variation that we look for when we texture. And to add even more variation to
[5:09] this, all I did was duplicate twice this map and simply rotated it. So as you can see,
[5:19] it's quite exactly the same, but it has a slight slant to it, as opposed to being perfectly
[5:27] straight like this one. It's been rotated, rotated, and it gives a nice look, a nice
[5:36] brushed metal look. Tip number two is adding heat distortion, heat discoloration. If I
[5:44] apply all these layers, you can see there's a nice gradient of colors that you can see
[5:51] kind of fading into one another, starting from, as you can see, yellow up to this emerald green
[5:58] teal type color. So to get this effect, I'm going to hide these layers and we're going to start on
[6:06] yellow base. So I'm going to hide these layers and we're going to start here with black and white
[6:13] spots. Again, this is a default map you can find in the search bar. So this texture map,
[6:19] we're going to put from back to normal. As you can see, it's covering the whole thing. We don't
[6:24] want that. We just want it on the bottom. So in order to do that, I put it to a normal blend
[6:33] mode you change it to. And then you simply paint in where you want to see the spots appear. So
[6:41] I've painted in these areas. If I go to the mask, these are the areas I've painted in. And I've added
[6:51] a blur on top of it, giving it a one intensity just to fade in those colors and make it seem
[7:00] pretty natural. I multiplied, as you can see, it's still called yellow base. Let's change it to red.
[7:08] Okay, and the only thing I did here, I kept the tiling exactly the same. That's important. And
[7:14] if I toggle between, you can see all I did was decrease the balance. So we're at point three
[7:24] right now. This is where we were with point five for the yellow. And we just bring it in a little
[7:31] bit back to point three. And you're now able to see both. I did this exact same method when adding
[7:44] these two. Feel free to tweak your contrast as well. Tip number three is going to be adding grime.
[7:55] Right here in black edge color, I added a dirt generator. And all I did here was, if we go into
[8:06] the mask, this is what it ended up looking like. All I did here was add a grunge concrete tile or
[8:13] texture, rather, and set the blend mode here to subtract. So all it did was just add that little
[8:27] bit of variation that we look for. Very subtle, just to break it up. This is pretty difficult to see
[8:37] as I'm going to show you my parameters here. I've used color roughness, and I have the metal
[8:44] activated. So 100% metal is this. And we want to just take it off a little bit. And I found it tends
[8:54] to look a bit more like dirt, of course, as you take off dielectric, you just feel feel out this
[9:01] type of thing. So if this is your metal map, you start to see dirt here. It's we don't want it
[9:06] caked on there. We just want to see subtle signs of it kind of like this. And this is even a little
[9:12] too much. I'm going to go back to okay. Again, I started out with a dirt generator. I'm going to
[9:20] hide this one just to make looking at this a bit easier. I'm going to hide the first one. So to go
[9:27] into this, we have this type of caked on dirt look that we want to achieve. You get your dirt
[9:39] generator. These are the settings I used. It's pretty contrasted. It's just pretty heavy in general.
[9:48] You set it to multiply. Okay, you set it to multiply. And I used a moisture node ironically
[10:02] enough to make dirt. I've set it to eight. These are my parameters. And yeah, it's just it's pretty
[10:13] simple. It fills in the multiply hides and this fills it in. So what I did after that was I went
[10:20] around with my paintbrush and I just the specific brush I used was artistic heavy sponge. So you
[10:32] just go around paint out the subtleties you want. You know, we're going to add some layers here. So
[10:40] if it looks a bit sparse right now, don't don't worry. Yeah, and I added another subtract
[10:46] to give that directional look here. So the next map we're going to add here, the same concept it's
[10:56] going to follow. So this looks insane right now, as you can see. So we're going to do the same type
[11:05] of thing. Hide this for the sake of looking at this. So we have it set to normal. Let's go ahead,
[11:13] bring it down to multiply galvanic large is the map I decided to go with, because it has very
[11:20] distinct sharp cutoffs, you know, it's a contrast texture. That's why I went for it. And these are
[11:29] my parameters for that. So the next thing I did, I went around, painted it out. What I didn't want.
[11:39] Same type of brush I use same process. You paint out what you don't want. It's pretty
[11:46] straightforward. One thing I did here that's worth noting. This is 100% subtraction. I still
[11:53] wanted a little bit of residual dirt there. So I went ahead and just kind of erased some of that
[11:59] subtraction work that I did with this brush, brought it back, but in a very subtle way. It's not
[12:06] aggressive. And then from there, I added another fill layer set to subtract. It's the same concept
[12:16] as this noise here. Same noise. Just to add that extra cool look to kind of go with the brushed
[12:26] look that I have going here. And then these here, these, these, what do you call them, paint brushes,
[12:35] there to take out what's on the inside. It's just a subtract, subtract. That's all. And then lastly,
[12:47] for this grime tip, the last thing we wanted to add is just another color variation type thing. This
[12:56] is very simple. As you can see, there's even tiling here. It's a, it can be kind of, so the last
[13:03] thing I wanted to add here was color variation. All I did here was a grunge concrete map. Didn't
[13:11] even tile it, kept it at one. It depends on your resolution, how you want it to look. But just to
[13:17] kind of go with, if I, if I here, I can quickly look at it's just color. And then I set it to overlay.
[13:26] That is all I did. And now we can go ahead and bring out all these. And as you can see, they kind of go
[13:34] with each other. So as individual layers, you know, they do not look convincing at all. But when you
[13:41] go ahead and, you know, add them all together, they compliment each other. They really do. And they
[13:48] make it look as one cohesive texture. We have some nice color variation in there, a little bit of
[13:56] roughness variation. It looks nice. The fourth tip is adding dense to our material. The first layer
[14:06] I'm going to add, I'm going to start with cells. Cells one, yes, cells one. As you can see, cells one.
[14:18] Right here, it looks like this. If we go into this view mode, I'm going to take out all this. Okay. So what I did
[14:31] here, it's currently inverted to go back. This is kind of, it's at point six, eight. We go boom, point six, eight.
[14:39] Inverted. And it gives this obscure look that we kind of want to change right away. But the next thing I
[14:49] did was I added another fill layer. I set it to subtract. And this is just a simple black and white
[14:55] spots tiled up pretty high. Again, it doesn't really matter what your tiling is. As long as you're
[15:02] happy with the result. These are my parameters. I set it to subtract. And I cut the subtract in half,
[15:13] basically. I still wanted a little bit of the dent to be there, but I didn't, I wanted to create some
[15:23] nice variation within the dent itself. So as you can see, this still isn't really what a realistic
[15:30] dent would look like on a pot. So we go ahead and add our blur to kind of finish it off. And yeah, as you
[15:38] can see, you get kind of like a very subtle, but nice dent generator that you can, you can play with.
[15:50] So we're going to add more of these layers to dense to. So what we did here was add clouds to these
[16:06] are my parameters tiling. And to go back on our, I didn't show you the previous parameters for dent
[16:15] one, but they're basically the same. Okay, our height is a little bit different. But these dents, we want
[16:22] to be more severe. So clouds to from there, we duplicate it. And we set it to subtract. So it
[16:33] thins it out a bit, thins it out, goes from this to this. And we have offset this, which is what
[16:41] makes this worth offset and tiling has changed. Okay, now we're going to go add our blur. And then our
[16:53] paintbrush. Yeah, like, great. You can see this is very, this is a very broad breakup. Just so we can
[17:04] properly see three here. So it doesn't look like much in the mask. But our height is very severe. So
[17:14] you're able to see it pretty clearly. Alright, not that severe. So we basically it's just a
[17:22] duplicate duplication of the same process. My parameters for each one here, pretty much the
[17:29] same. And then you add a blur. So I point point two seven five is my intensity for the blur. And then
[17:36] this is just another subtract for the the bottom that we do not want. Okay. So this is kind of what
[17:46] you get. There's the nice, you get that nice variation. The fifth tip is going to be adding this
[17:54] kind of dried water drip look to your pot. The first thing we want to do, luckily painter has
[18:05] basically an exact texture that you would need to use for this. It's called leek small. It does
[18:15] exactly what it has. It serves one purpose is to make make this detail. So we're going to add this
[18:21] in. These are my parameters. We're going to add a fill layer here, set it to subtract a simple black
[18:30] and white spots. My parameters are here. And again, this is just to break up some repeating factors
[18:42] and to make it look a bit more unique. And then what I do here is paint out whatever details I do
[18:54] not like. So if I notice something is not maybe where I want it to be, as opposed to trying to
[19:04] tile this and you just create sometimes more more work than you want, you can just kind of finish
[19:11] it off via a subtract paintbrush and just go around to clean up the areas you don't want. And it
[19:18] looks like I have duplicated. I've made two, but you really only need one. So that's detail five.
[19:27] Another thing you want to notice is these. These are my these are my material parameters. So I've
[19:39] set the base color. My roughness is pretty high. And my metallic is more towards the dirt value.
[19:47] It's gone away from pure metal. So as you can see the base color here drips, you can see it very
[19:55] lately. It's as if dirt had been attracted had gotten stuck in a line of water and it's dried.
[20:07] That's basically the concept I was looking to achieve. So it's rougher than its base material of
[20:13] the pot. And yeah, metallic, it's more towards this is more towards the dirt side. It's less pure
[20:25] white. It's more on the black side. Thanks again for watching fast track tutorials. These were five
[20:34] tips on improving your texturing in Substance Painter. Thank you.



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
