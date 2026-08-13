---
title: How to use UDIMs properly!
source: YouTube
url: https://www.youtube.com/watch?v=yf9CPHE5BYg
author: 3DRedBox
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/how-to-use-udims-properly/
frame_count: 0
frame_status: pending-selection
---

# How to use UDIMs properly!

**Source:** [YouTube](https://www.youtube.com/watch?v=yf9CPHE5BYg)
**Author:** 3DRedBox
**Duration:** 17m19s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py how-to-use-udims-properly <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] UDIM and keep the text density same per tile is a problem for you.
[0:16] I'm Mehdi from 2D Red Box Channel and today in this video we want to talk about how to
[0:21] keep the same text density across multi-tiles in UV.
[0:27] So, be with me in this video, we are going to explore this.
[0:31] But before that, let me introduce you the brand new course that we release for Substance
[0:37] Painter.
[0:39] Learning Substance Painter is easier than ever.
[0:42] Hey all Substance Lovers, Tech Change Seekers and awesome future artists, welcome to ultimate
[0:48] course for learning Substance Painter from Zero to Hero.
[0:58] Ready to learn how to texture with different projects, Substance Master released a brand
[1:02] new course for those who want to learn to texture with Substance Painter.
[1:08] In this course we cover from preparing the model to rendering different projects, different
[1:13] challenges.
[1:14] If you want to level up your skill in texturing, come and check the Substance Master Ultimate
[1:19] course for learning Substance Painter.
[1:22] Ok, now we are here and we have this model and we want to texture this inside Substance
[1:28] Painter.
[1:29] But there is one problem here.
[1:32] This model is so big.
[1:34] It contains so many small pieces.
[1:38] And how we are going to manage the quality inside UV and the final texture.
[1:46] And in here the first solution is to pack all the UV island inside one UV tile.
[1:54] And let's do that and compare it to the other option that we have.
[1:58] Ok, let's copy this model and I'm going to rename it UV1.
[2:05] And for sending this model to the RISOM UV, I use the bridge that's very easy and fast
[2:13] and you can use it in 3ds Max and you can find the link of this script inside the description.
[2:21] So let's put it on edits and click on send to RISOM UV.
[2:26] And when we use the RISOM bridge, it's automatically open the RISOM UV and import our model with
[2:34] the UV.
[2:36] And now I'm going to pack this UV inside the RISOM.
[2:41] And how we can achieve the best result inside the RISOM?
[2:46] We just need to go to the packing properties and change accuracy to ultra and iteration
[2:53] to something like 4 or 8 and after that we can set initial orientation to V and change
[3:03] orientation optimization to 90.
[3:07] And now I can go and click on pack.
[3:10] And as you can see, we have a perfect packing of UV inside one UV tie.
[3:18] And for bring it back to 3ds Max, we just need to press CTRL S and now we have the model
[3:25] inside 3ds Max.
[3:28] And let's add some material to this model because we want to compare this with another
[3:35] option that we are going to create.
[3:38] For this purpose, I just use a simple 1K texture and tile it 4 times because we want
[3:48] to represent the 4K texture.
[3:53] So let's apply to this model and this is the final quality that we are going to get from
[4:01] 4K texture on this model.
[4:05] Compare this pixelate issue that we have here and I'm going to copy this model again and
[4:15] rename it UDEMS 1 and let's bring it to RISOM.
[4:22] And we are in RISOM again and for increasing the quality when we want to use something
[4:30] like texturing in substance painter and create unique texture, we need to extend our UV
[4:38] tile to 2, 3 or 4 or more.
[4:42] And we call it this technique UDEMS and in RISOM we can increase UV tile spaces with
[4:52] this window, little window here.
[4:55] And let's increase it to something like 4 and I'm going to change accuracy to ultra,
[5:03] iteration 4 and initial orientation to V and orientation optimization to 90.
[5:13] And now I'm going to pack it again and now we have 4 UV tiles as you can see and let's
[5:20] save it and bring it back to 3ds Max.
[5:24] And let's give the same material to this model and now you can see we have more quality
[5:34] on this texture.
[5:36] And the reason is we have more UV tile, it means we have more UV space and when we have
[5:44] more UV space we can increase the UV island size so we have more pixel on each UV island
[5:54] and it means we have better quality compared to one UV tile.
[6:03] But the problem here is when we increase our UV tile number we may get different size of
[6:12] each UV island in different UV tile.
[6:17] So how we can solve this problem and for solving this problem we need to keep same
[6:24] pixel density when we are going to pack all the UV island in UDEMS or multiple UV tile.
[6:36] So let me bring another version here and let's call it UDEMS 2 and send it to RISO.
[6:49] Okay now we are here in RISO and the packing properties it's same that we discussed before
[6:58] and now I'm going to increase again the UDEMS to 4 tile and let's pack all the UV island
[7:10] across these tiles.
[7:12] Okay this is the final pack but it's not correct I just changed it for demonstration purpose.
[7:21] We don't get this kind of effect when we pack inside RISO UV because we use initial scale
[7:30] keep average pixel density option but in here I just want to show you what happen if we
[7:37] have different scale on each UV island.
[7:43] And the translation of this matter is we have the lower quality here and higher quality
[7:52] in here and this is the problem okay and it happens all the time when we want to use UDEMS
[8:02] in complex object okay and how we are going to solve this.
[8:08] For solving this issue we need to understand how toxial density works but it's kind of
[8:17] complex matter so let's keep it away and stick to the simple way that I'm going to show you.
[8:25] So we have map res and texial density target option here and for the map res we need to
[8:36] find out what is the final dimension that we are going to export for example from Substance
[8:42] Painter or even what is the size of the final texture that we are going to use in our material
[8:49] inside our project okay and in here it's 4k so let's put 4096 here and if we are going
[9:01] to use 2k let's put it 2048 and what's about the texial density target for this matter
[9:09] let me show you easy way okay so let's pick biggest UV island that you have okay for example
[9:19] this one this is the biggest UV island that I have and let's isolate it and just press
[9:28] on back okay and select this and pick okay as you can see we have 43 texial density target here
[9:43] okay it means we have the quality near to 4k and it's good it's good but what happened if I use
[9:57] this texial density target let's select all this UV island and press rescale and as you can see
[10:09] maybe we need more than four tiles here so let's give it eight okay and now we need to change
[10:21] texial density target to something like this I just use the map res and divide it by 100
[10:33] because I just use centimeter here okay for modeling and now it times to change some setting
[10:43] in packing properties the first one is changing initial scale to texial density and after that
[10:54] turn off scale optimization range from full to off and now it's time to use
[11:04] packing here and let's wait and see what's happening okay now after packing all the UV island in eight
[11:15] UV tile as you can see we have the great quality here but we have some space here
[11:23] and for solving this issue we can go here and select some of the UV island and bring down
[11:33] the scale of them so in this way we can save some space for these icons and pack it up all the UV islands
[11:47] in seven UV tile okay not eight but it's okay for me right now and let's save it and explore another
[11:57] option here okay now we can understand how we can keep the same size or same texial density
[12:07] when we want to pack all the UV island with udim's method okay but this is the method based on
[12:18] texial density what happened if we have some limitation for example we can just use four
[12:27] UV tile how we can keep the same size in four or three UV tile let's do that now I'm in the
[12:36] RISO and we have three tile with the udim's and I just pack all the UV island with the same packing
[12:46] properties that we discussed before and let's check the scale or texial density of each UV island
[12:55] inside each UV tile and the map res here is 4k so I need to change map res and just select
[13:06] this one and use this checker and the texial density is 24 and for this one it's 24 but we have some
[13:19] small difference in the number after dot okay and this is 23 so we have the same texial density
[13:35] almost the same but what's happened if we want to keep the same texial density when we want to have
[13:44] the three udim's okay so we have 23 and 24 okay so let's pick 22 here and I just turn off the
[14:00] scale optimization range and change initial scale to texial density and now when we
[14:08] click on the pack the texial density of each UV island should be 23 and as you can see we have 23 here
[14:20] 23 here and here so in this way we can keep the same texial density or same scale of
[14:32] UV islands in different UV tile and for the last part let me show you how we can check the texial
[14:41] density quality inside substance painter okay now we are in substance painter and whenever we import
[14:49] something like a complex model and we don't sure the UV is okay and at the end we can get
[14:58] a good quality of that we have a generator inside substance painter that we can use
[15:06] and check the quality of the UV so in here I just add generator on the paint layer go to the generator
[15:18] and just use UV texial density and let's just keep the color and whenever we have the red color
[15:30] or something like red it means we don't have enough quality inside the UV okay and for the green it
[15:41] means it's okay and we can continue but we couldn't use the lower size like 2k or 1k and we just need
[15:52] to export higher quality like 4k or 8k and when we have the blue color it means we are in a good
[16:01] position and we could use for example 2k as a final export and we get a good quality okay so in here
[16:13] for this UV we get the green color okay and now let's go I'm going to copy this layer and let's go
[16:26] to the next model and in the next model we have 8 UV tile okay and let's copy that and as you can see
[16:39] we get the blue color here so we are good and we can start our process and texture this model
[16:49] and that's it this is for this video I hope you learned something new and I can answer your
[16:56] question because we have a lot of questions about the UV u-dims and keep the same texial density
[17:03] across multi tile and this kind of question if you learned something new or like this video
[17:11] please hit the like button subscribe our channel be creative bye



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
