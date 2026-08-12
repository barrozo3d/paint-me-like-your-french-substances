---
title: How to TEXTURE EVERYTHING in Substance Painter
source: YouTube
url: https://www.youtube.com/watch?v=GvjfkhCW3aM
author: J Hill
ingested: 2026-08-12
app: "Adobe Substance 3D Painter"
version: "not stated on screen; Bevel Smooth filter usage places it at 11.0.0+ (see App & Version note), estimated 11.0.x-11.1.x"
tags: [layers, fill-layer, paint-layer, masks, smart-mask, smart-material, generator, anchor-point, blend-mode, curvature, ambient-occlusion, tri-planar, procedural, MatFX, udim, texture-set, pbr, metal-rough, basecolor, roughness, metallic, height, normal-map, emissive, opacity, alpha, iray-render, export, export-preset, channel-packing, game-engine, unreal-export, advanced]
extraction_status: complete
frames_dir: tutorials/frames/how-to-texture-everything-in-substance-painter/
frame_count: 22
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# How to TEXTURE EVERYTHING in Substance Painter

**Source:** [YouTube](https://www.youtube.com/watch?v=GvjfkhCW3aM)
**Author:** J Hill
**Duration:** 199m28s | 16 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Hey, I'm Jay and four years ago I made this video about texturing skin with Substance Painter
[0:27] and people still let me know that tutorial was helpful, so this is the sequel to that video.
[0:33] But instead of focusing on texturing skin, it's about everything else. I've tried to cram as
[0:38] much useful info and techniques and tools for texturing some of the most common materials
[0:44] with Substance Painter. So this is my super duper big texturing tutorial. I've also made the project
[0:50] files for this available to anyone, the links down below, so you can download these and you can
[0:56] texture this helmet project yourself or you can take a look at my scene, my completed scene,
[1:02] for reference. And I've also included some decals that I've made and samples by Jonas
[1:08] Runagord. So you can use those and I've also included my export presets for Unreal Engine.
[1:12] The full seven hour raw version of this demo is already available and at my course at Character
[1:19] Class.com and it's available for all the students there already. And I've also uploaded that same
[1:25] unedited version to this channel for members and my patrons. So if you really want the unedited
[1:33] real time version of this demo, you can watch it for as little as seven bucks. Lastly shout out to
[1:39] the homie Brecky Thor BT from the servers who made this initial helmet model for me to use in this
[1:46] demo. And also shout out to Hazel Brown. She made the hair model that I used in the final presentation
[1:53] at the end. First, I want to start off by showing you my references for the project that I'm going
[1:58] to be showing and also just a quick word about my texturing philosophy. And then we'll jump right
[2:04] into the demo. Enjoy and I hope you learned something. Okay, so here in puref, we can see


### References [2:07]
**Transcript (timestamped):**
[2:11] some references and here are helmets. This is very much the vibe. And then here's this idea of the
[2:17] Hollywood texturing. So when doing texturing, I think there are two kinds of parallel things
[2:24] going on. There is the storytelling side of things, the cause and effect, you know, the very
[2:31] kind of mathematical way to look at things. What are things made out of? How are they put together?
[2:36] How do they interact? Where have they been? What's been happening? And again, we're drawing on those
[2:41] so that we can do the creative part. That's the parallel thing going on is that in addition to
[2:47] what things are made out of and where they're from is the overall kind of aesthetic look of what
[2:54] we're doing. And we're going to be balancing and using those two things together. So the way
[2:59] something looks, you want it to be appealing, you want it to be readable, all right, you can think of
[3:04] your work, your assets and having like a first, second and third read that first read needs to
[3:10] make a nice impact, be clear, legible and make a nice first impression, right? Somebody needs to
[3:15] look at it and go, oh, cool. And then the second read starts to be more the storytelling aspects.
[3:20] And the third read is like the details. And if those keep holding up, you have something that's
[3:24] really great. And we can see that in some of these Hollywood things, you know, so things aren't
[3:29] perfectly clean. Here's an example from this, the coolest show, Knights of the Seven Kingdoms,
[3:33] that's going on right now. We hear you have people in white armor. And so the white you still have
[3:37] like, you know, here's like, it looks like maybe rain or something, right? So you have some rust
[3:41] dripping down dirt around here. So you have different whites, different shades. Okay, and you
[3:46] have different kind of types of grime. We'll show it again. Right here's a good example. Okay, some
[3:51] work from Weta. Here's something that is meant to be new and clean. Nothing will ever be actually
[3:58] perfectly clean. So you see some some kind of subtle, you know, looks like just dirt in some
[4:03] ABS plastic bumps or whatever you get some cloudiness on the surface. So that's the cleanest
[4:07] it's going to be. And if you look closely here, do you see how there's kind of like grime inside
[4:12] the insets and in the corners? And you see the little edge wear on the on the edges. This is
[4:18] the fundamental thing I'm talking about is at a base level, you always are still going to be trying
[4:24] to emphasize certain shapes that you want, making something graphic and readable. And that's how
[4:32] we're balancing it, right? If we can kind of make this seem like believable, maybe dirt would go
[4:37] in there, maybe it would get some edge wear, okay? And we're walking that line because we don't want
[4:41] it to be too procedural. But this is a common technique, you know, in the Hollywood prop stuff
[4:46] that they do washes of different kinds of thin paint, and they'll rub it away so that the cavities
[4:51] and recesses get darker, they'll rub and buff the edges to pop them out. And so we're doing that sort
[4:56] of thing too when we're texturing. Okay, so this is the kind of curated look we're going for that
[5:01] doesn't look necessarily like a found object. It looks like, you know, a nice cool prop. That's
[5:07] the first read, very simple, easy, boom, got it, graphic. And then we're holding it up with the
[5:11] details we go through. Let's talk about the scene setup. Okay, so when you open this scene or any
[5:17] new scene when you're starting some things that you might want to change at least I change every
[5:21] time. If we come over here to the display settings, you'll see if I if I increase the
[5:27] environmental opacity, and I turn down the blur, this is the default, which is like a sunny field.
[5:33] I still think this is a mistake that they do this. And it looks kind of even hidden because
[5:38] people may not know we'll do the number one dude, Tomoko bro studio Tomoko this is where it's at.
[5:44] If you know you know this is the this is the best HGRI that's out there. So yeah, we need just team
[5:49] Tomoko guys. All right, this is all you need to know. You can blur it a little bit if you want,
[5:53] but I'm slower the opacity to we can just be in a black void. Honestly, or we can you know a little
[5:56] bit of a little bit of something if you want but all right so this is the one change I would make
[6:00] and then the camera settings I like to change the focal length I don't know what it starts out maybe
[6:05] 30 or something but looks all kind of warped or whatever. So 50 is a good little rule of thumb
[6:10] this is the this would be the lens that's somewhat similar to the human eye. Okay, and then if you're
[6:17] doing a portrait sometimes I change this to 85 but those are just a couple things do right off the
[6:21] right off the bat. Just an overview of the scene you can see we have four texture sets and you
[6:27] don't really need lights in here but yeah really three texture sets we're going to texture the helmet
[6:32] the cables and the visor and you can see the helmet is four udims we're going to jump over to the
[6:37] helmet we're going to do that we're going to spend most of our time here on helmet if I hit f1 on
[6:42] the keyboard you can see the layout so here it is this is the bake and the the layout for now
[6:48] you can see both at the same time check that out. All right so that should be good now we got neutral
[6:53] light that's why we changed our HRI by the way we don't want color cast so when you're in a sunny
[6:57] field it's gonna it's gonna cast a color so you want a desaturated environment you want something
[7:02] that looks a little bit believable. The first thing I do at the start of any texturing project


### Blockout [7:03]
**Transcript (timestamped):**
[7:07] similar in 3D is to block out your scene okay blocking out your scene is super important because
[7:12] it gives us our first run it's our first draft and we get to think about it in terms of what
[7:17] materials do I need and we'll set up the scene by using folders for each material we'll make our
[7:23] masks and it's really our first pass at outlining what we need to do the texturing so we're going
[7:29] to front in some of that stuff and so we're just gonna set ourselves up for success so let's do
[7:32] that we're gonna block out this scene and we'll start making materials with folders we'll name them
[7:37] and then we'll start making fill layers and masks and really outline everything we think we need
[7:42] right now for this helmet project. Alright first thing I'll do is I'm gonna delete this
[7:46] default layer or whatever and I'm gonna make fill layers and I'm gonna put those fill layers in
[7:52] folders. The first fill layer I make at the start of everything is I just call it base if you see
[7:58] here on the left we're gonna add every channel and we're gonna set the defaults because the way that
[8:03] substance painter works is that it goes bottom up all right and because of certain things we're
[8:09] gonna do later if we don't set defaults then it'll just inherit something later so this might make
[8:15] sense as we add more things but it's really good practice to set your base your bottom kind of anchor
[8:19] layer at the bottom that just have all your defaults okay so for height we'll keep zero for roughness
[8:25] that's fine metallic zero normal zero so this is fine for now so this is our base layer you can
[8:30] even by the way like sometimes I'll make this a bright color so that you can see the areas that
[8:35] don't have a material yet but maybe for now we'll we'll keep this white so you should still see it
[8:42] but it won't be so obnoxious okay so now we're gonna create a folder let's start with metal and then
[8:48] for organization I'm gonna keep my materials capital letters all right and then inside we're
[8:55] gonna create a base so I'll do another fill layer we'll call this base we just call it base metal I
[9:00] guess we want to be organized and then the base color we can keep this roughness we'll do point
[9:07] three is fine and metallic one all right so already we got metal going look at that all right and then
[9:13] let's do paint all right and then for that we'll just do a reddish color and then roughness we'll do
[9:25] that's fine for now metallic zero so now we have a nice red paint all right and then we can even do
[9:32] a height while we do we'll just have a height layer on here for right now so we can already start
[9:36] masking some stuff why don't we start with this paint mask so we have the metal right and the way
[9:42] we're gonna think of this is we're gonna build our materials up and you can see in the layer
[9:49] outliner stack here we're gonna do it in the order that it would be in the real world so the
[9:54] whole thing is metal for now later we'll replace it with some plastic parts but you can imagine
[9:59] almost like the whole thing is metal and then we're gonna do paint on top of that dirt on top of
[10:04] that right it'd be paint or a metal paint stickers dirt you know what I mean so we're gonna layer it
[10:11] up you want your layer stack on the right here to always be that you know emulating the layer
[10:17] order that it would be in the real world so we'll start by doing some paint right now so we can
[10:21] overlay it on top of the metal we'll right click and add a black mask and then we can add a paint
[10:28] layer here now this is the first thing to know I add a paint layer for everything I don't as you
[10:34] can see like if I was just in this mask I can I can paint directly in this mask okay because I have
[10:40] a paintbrush right here right I can just choose a paintbrush and I can paint in this mask now I
[10:46] don't do that because one of the great things about substance painter is that it can be non-destructive
[10:53] or you know very non-destructive maybe not a hundred percent but that means that you can go back and
[10:57] edit and change things you can split things out and that's what we want we want to be able to go
[11:02] backwards and forwards so I never do anything directly in the mask everything I'll do I'll add
[11:09] little modifier thing here so instead of painting I'll add a paint layer okay because then I can
[11:15] add more paint layers and you can name these so super super great you can be organized and again
[11:21] you can just go back and change anything at any time that's what we want so I'm going to come over
[11:25] here you can see this polygon fill and this gives me some options so we'll go over a few different
[11:30] ways that you can do masks so a lot of these meshes are separate make our lives easier so I can just
[11:36] start clicking and I'll add paint right so I'll just add paint to this stuff there you go adding
[11:43] paint here okay how are we looking shift them right clicks how I'm moving the light around
[11:48] all right uh there's some paint right here there's some paint right here I won't spend too much on
[11:54] this side just for the demo as long as it looks good from this side I'll be good so here's our first
[11:58] example of like we might want to wear this away but maybe I'll come back and I'll just wear this away
[12:03] you know like maybe the heat's messing it up but still we'll keep it simple in the beginning
[12:07] all right so we've got our paint masked on there great now let's do
[12:15] plastic then we'll add our fill layer and we'll call this base plastic okay and then
[12:23] for base plastic we'll do kind of a darkish color height we'll just turn that on for now
[12:29] so it can be at zero still roughness why don't we do 0.45 a little bit rough not too much
[12:35] and then metallic zero so now we've got a dark plastic now we'll add a black mask to that folder
[12:40] and again we'll do a paint layer and we'll start layering this up all right uh we make this plastic
[12:47] this whole hose plastic could also do the inside okay so that was our first hey uh oh we don't want
[12:55] to do the whole mesh right we just want to do the inside okay well we can come over here you can see
[12:59] you can do uv chunk fill instead and then I can do this because I separated the uvs there so that
[13:06] I could do this very thing come back to the polygon or object fill mesh fill and then we'll do most
[13:13] of this stuff so why don't we fill this and this this pretty much everything but the hardware and
[13:19] then we'll fill everything in here maybe yeah when I just fill all this stuff and then we'll make these
[13:26] inserts here plastic actually we'll do this could be plastic too that would make sense
[13:33] just while we're working why don't we do something um nice soft lighting about this
[13:39] there we go that way we can see let's turn the lights on so we can see okay looks pretty good
[13:45] also uh you see this wireframe like I don't really need that to be that crazy so why don't we change
[13:50] that too come in here let's turn down the wireframe opacity I don't think we needed that much so now we
[13:56] got some plastic bits is everything else this could be plastic too so I think we're pretty good with
[14:00] that now let's do leather and then just come in here we'll do base leather and we'll choose a brownish
[14:11] color and then we'll do roughness 0.3 height metal zero we'll come back to this leather is a whole
[14:18] thing but let's just mask it where we think we'll need it got our mesh fill here's a leather strap
[14:24] here's a leather strap here's a leather strap all right we good there and I think that's all the
[14:29] leather we got on this one okie doke mr plastic okay now let's do a fabric we've got a couple
[14:39] fabric elements here so fabric now instead of creating a fill layer why don't we type in
[14:45] fabric and I actually know that there's one I can use right here fabric cotton jersey I think it's
[14:51] going yeah fabric cotton jersey and then I'll just drag and drop it in there there you go
[14:58] gonna want to change some of things here let's see well we'll just change the tiling why don't we
[15:03] make it eight there we go it's better okay and then the fabric color will make it more just an off
[15:12] white kind of feeling and then fabric color variation make that higher there we go nice
[15:19] it looks a little pilling there and then let's see weft distortion we can even mess around with this
[15:23] how about we do point well just do point one there we go get a little bit of things there and then
[15:29] the height range we don't need it to be that that big so we'll make it a little bit softer
[15:35] there we go so it's softer but there you go so you got some tooth to it see and there we
[15:39] used one of these base materials that comes with the program all right so now add a black mask paint
[15:45] and then we'll select that fabric that fabric there we go so now I've got our fabric things
[15:51] chosen great okay looking good all right well there you go so far done no not really but there so
[15:58] now we've outlined the materials that at least we think we need right now metal paint plastic
[16:04] leather fabric looks good we have our masks now we can start adding more nuance and detail to try to
[16:11] make these materials feel more like the materials and then you can start layering adding more detail
[16:18] all right so next we're gonna do metal we're gonna focus on doing the metal base now we're gonna be


### Metal [16:24]
**Transcript (timestamped):**
[16:24] focusing on texturing metal all right we're gonna add some more fill layers some more nuance and
[16:31] roughness and things like that and we're gonna build up our base metal try to make this helmet
[16:36] at least the base metal look good and we'll go over some different techniques and filters and
[16:40] stuff like that right so let's jump into that closed up these other folders we don't need these
[16:45] and we can even start assigning these some colors so we can separate this even better
[16:51] so let's add our first wear level we'll add another fill layer we'll call this wear and then over
[16:59] for the base color make it a little bit darker make this 55 and then for roughness we're also
[17:06] gonna increase the roughness go something around 0.8 okay and then we're gonna add a black mask to this
[17:14] and then we are going to add a fill layer and then in here we're gonna use some grunge grunge
[17:22] gonna use this a lot so we'll type in grunge paint scratched and see what we got here so we got
[17:28] grunge right here paint scratch i'll always love this one now you could drop this right here
[17:33] you could drop it right you could drop it in there you could come over here to the fill layer
[17:38] and type in here you could go grunge paint scratch same thing okay three different ways to do it
[17:43] all right now we are gonna do some editing of this so why don't we turn these off so you can see
[17:50] here's our metal for now okay here's what we're here's what we're cooking with now we need this to
[17:55] be nice and sharp so let's do tiling we're gonna set this instead of one to ten and then balance
[18:02] um let's drop it down a little bit and then contrast let's up this all right and then we'll add a
[18:09] filter so right click add filter and we'll come over here and we'll do these are here's all your
[18:15] filters you can filter just for filters but if i type in sharp you'll see little triangle guy
[18:21] i'll click that oh oh so nice defaults to a little bit a little bit too much let's drop it down to 0.15
[18:28] but you can see if i turn it on and off better okay so here's our first wear layer for our metal
[18:34] just so it doesn't look too perfect right now let's do another one we're gonna add another fill layer
[18:39] and we'll call that noise and then for noise i'll do a little brighter color okay maybe 0.85 and then
[18:47] for roughness we'll do 0.85 we'll add a black mask to this black mask and now some more common
[18:53] fills that you'll use noise so if i just search for noise in my assets we can look for how about a
[19:00] 3d perlin right here is this fractal yeah 3d perlin noise fractal let's do that right there
[19:07] and then for projection we're gonna switch it to match per uv tile uh because it's udms that way
[19:13] goes across the udms and then for position for this one we'll go 0.36 we'll drop it a little bit
[19:20] contrast let's do 0.45 now if i hold alt and click the mask you can see it okay so why don't we do
[19:28] that so you can see what we're doing and then for scale let's do 10 so it's getting bigger
[19:34] and then in here it has it has something called roughness that's just for the actual pattern
[19:39] and we'll we'll up that too here's our noise breaking it up but a little bit too procedural
[19:45] a little bit too perfect so we're gonna add another we're gonna right click here and we're gonna add
[19:51] a new one fill and we'll do let's do a 3d perlin noise fractal again why don't we do that again
[20:00] and then we're gonna set this to multiply so here let's isolate this so you can see again
[20:04] so this is what we made adding a new one but if we set it to multiply just like in photoshop it's
[20:09] gonna be removing from it so for position you know we can leave this you know generally right here
[20:14] and then for contrast we'll go up quite a bit and for scale we'll make it even so yeah so now
[20:20] we're removing it from some places you see if i make it really strong you can see so hit m there
[20:25] you go so now we have our our noise which is breaking up the light all right and this is the
[20:30] kind of this is the kind of nuance we just keep adding and adding and adding and adding and it's
[20:33] gonna feel better all right now let's add edge wear to this we're gonna add a new fill layer
[20:39] we're gonna type in edge wear and then let's make the base color white and then roughness we'll just
[20:47] do 0.5 we'll add a black mask to this and then we'll add another common thing edge wear generator
[20:55] so let's do a generator go over here and we'll type in metal edge wear you see right there metal
[21:02] edge wear doink so we'll load this nice all right let's jump into this mask you see what's going on
[21:10] looking cool but you know we're gonna edit some stuff so wear level we're gonna make this come up
[21:15] a little bit wear contrast we're gonna go down a little bit and then for the grunge amount go down
[21:22] a little bit because we don't want too much grunge for this we're gonna add our own grunge you know
[21:28] and then edge smoothness 1.7 there you go that really softens it okay now we'll add a sharpened
[21:36] to this too so right click filter and then we'll make this 0.25 doesn't need to be all right so again
[21:45] you can see what the sharpening is doing looking good and then you can see what this edge wear is
[21:51] doing yeah i think i'll just turn off the roughness for the edge wear and just leave it the base color
[21:55] for now okay all right cool so we got this we got some edges popping out and we've got some grungy
[22:01] stuff let's add scratches so add another fill layer and we'll call it scratches and then we'll add a
[22:09] black mask and then we'll right click and we'll add scratches generator it's going over here to
[22:17] generator we'll type in scratches so there should be a scratches generator all right so we're gonna
[22:23] add that as our fill layer there you go scratches generator all right now we're gonna make a bunch
[22:28] of changes to this again let's isolate the mask you see what we're doing all right for spline number
[22:35] we're gonna lower that down a bunch make it like 200 spline scale maybe 0.75 something like that
[22:42] spline width make it thinner and then spline scale random a little bit and then width random a little
[22:51] bit all right and then spline distortion that's good spline distortion frequency maybe a little
[22:58] bit more okay and then fade length yeah we're gonna do both ends we want to fade in and out
[23:05] and then the length you know maybe a little bit like that okay so that is our scratches now what we
[23:11] could do is we can make this white we want to or maybe just a little bit brighter and then for roughness
[23:20] we could go really rough or we could go really smooth depends on what you want really even in
[23:25] the height we could do a little bit in the in the height that we wanted to like really you know
[23:32] mess with the lighting but now we've got scratches too and you can again because it's
[23:37] non-destructive you can even balance all this stuff okay so let's just keep adding stuff all
[23:41] right we're gonna do screws we're gonna make a layer just for our screws just because they're
[23:46] inheriting a lot of the big wear and we want to kind of curate that you could actually make your own
[23:51] folder just for screws if you wanted to or you know separate multiple things out but we'll keep it all
[23:55] in metal folder but you can do whatever you want so like we'll make a fill layer now just for screws
[24:00] and then we'll do roughness and metallic so let's do roughness 0.5 metallics obviously gonna be one
[24:08] and then for the base color we're gonna we're gonna do something a little different for the
[24:12] base color we're gonna add a generator so we'll come in here and we'll do a curvature so we're
[24:18] gonna use this curvature for our base color i'm gonna hold alt now i'm gonna click color just so
[24:23] it only is on the color and then we'll mess around with this so we got color only balance we'll do
[24:29] 0.45 and then we'll add oh let's go and change this yeah so then for the mode yeah we want edges
[24:38] sharp we're gonna leave it one fine we'll drop down 0.66 if you haven't used this before this
[24:43] use this curvature all the time and then big we'll leave big 0.25 i guess there so now it kind of
[24:52] looks nicer for our screws you see what i mean okay cool now because now we get like darker holes
[24:58] and everything so we're gonna add a black mask to this and we're gonna select our screws see this
[25:03] looks better for our screws can actually click whatever you want because you could use this now
[25:08] you have like a second you could just name this something else you know like old metal or whatever
[25:12] so you can just click random stuff that you want with this kind of dark darker look you know maybe
[25:19] even that's cool right i don't know all right again i'm not gonna spend too much time over there but
[25:22] let's just get these in case they're in view so it's kind of like a darker anodized look for the
[25:27] screws all righty we got some screws let's add another one another fill layer we'll call this one
[25:34] surface imperfections and then let's add some stuff for our base uh here let's see height 0.03
[25:43] and then we're gonna do this is more like form stuff and then we'll add black mask we'll add
[25:50] clouds so let's just look for clouds we'll do clouds one and then we'll set the scale to three
[25:58] and then layer opacity we're gonna drop it down so you can you see the light moving across this
[26:04] so the difference makes it bumpier and we're gonna lower this now you need to lower the opacity here's
[26:11] here's your first uh brain teaser if you're new to substance at all and you're not used to this so
[26:17] here's our entire layer stack right we have uh blend modes and we have opacity and all that if i
[26:24] i have to switch it to each channel to control that stuff per channel so you actually have
[26:30] you know however many channels you have that's how many you have to manage and this will come up
[26:34] time and time again but i'll just show you now right so we're gonna come in here we're gonna go to
[26:37] height and we're gonna change you can see the blend mode is linear dodge let's add and we're gonna
[26:42] change the opacity we'll change the opacity to something like 40 so now if i go on and off
[26:47] subtle okay can you see that let's get a glancing angle here there you see the light coming okay so
[26:53] that's again subtle but just making things more imperfect that's why we call it surface
[26:59] imperfections okay go back to base color that's usually where we hang out let's add some more stuff
[27:04] we'll go fill there and then we'll do grunge plaster paint yes check this out grunge plaster paint
[27:13] all right balance we'll do 0.9 and then tiling amount okay so now we've got some
[27:21] kind of chunks missing too but now as you see the light rolled you see that that's the whole
[27:26] point of this is to see the light rolling around and then getting caught on stuff glancing angles
[27:32] it looks more like a rough surface now and that's the idea all right maybe our first opportunity to
[27:38] check out ira so that's this camera button if i click this camera button it's going to open up the
[27:43] ira renderer this is an actual ray trace renderer and so you'll get you know actual like bounce
[27:48] lighting and ray-trace shadows and stuff and this is a good way to check materials this is
[27:52] like the ground truth real time will be different but you can just see does it feel like metal
[27:56] interacting so you see you get these little damages and stuff like that so i'll change the opacity
[28:01] so that's not so deep and just make them like little chunks missing like maybe there's a little
[28:05] bit more like rock so here it will come in and we'll change this to 50 so yeah now subtle but
[28:13] it's okay that's what it's all about all right so here is our nice base metal cool and ready to
[28:20] layer up more and more stuff if you were gonna have something be kind of pure a big piece of this
[28:27] that's metal that's how i always i would think about it like if there's a part of your asset that's
[28:31] a big part then you want to bring interest you're gonna treat that differently but this is our
[28:35] underlying material and what we're gonna end up doing is revealing it here and there so you can
[28:40] be a little bit more heavy-handed you can scatter things a little bit more that's what we're doing
[28:43] here but if you wanted to have an an entire exposed metal piece then you probably come in and add
[28:48] some more you know hand curated nuance or things here and they're a breakup thing so it's not so
[28:53] procedural but for our base metal for what we're doing is a good start let's see let's add before
[28:58] we're done let's add one last thing and that's some shiny metal maybe we can wrap up our surface
[29:05] imperfections with a sharpen first and then we'll just make this like 0.33 i guess just so it's not
[29:11] too crazy all right so we got some little dings and let's finish with with shiny metal shiny metal
[29:18] and then we're gonna do base color value 0.7 through 5 that's fine and then height we're gonna
[29:25] do this and then roughness we're gonna do shiny now here is your next lesson in managing layer
[29:32] blends if i come over to height okay you see it's on linear dodge add by default we can actually go
[29:37] to height and i'll show you in height we're gonna set it to replace and you see what that did it
[29:42] replaced all of the height below it with zero now that's gonna let us add these polished pockets
[29:50] all right so now we could add a black mask and then we could add fill layer here and then maybe
[29:59] we want yeah maybe we want to do the metal here metal edge wear okay and then we'll make smaller
[30:07] and then we'll do the smoothness for sure our contrast and then do a lot more grunge and
[30:13] i'll make it bigger there we go so now we've got some shine coming through too so again if you
[30:20] wanted to show an individual panel or you want an entire metal helmet you might go about it a
[30:25] little differently or at least in the way it looks but this is an example of adding lots of
[30:30] fill layers that have different elements that are mixing together and you can create a nuanced
[30:34] look so it's you can see the difference between these layers isn't so big at least not between
[30:39] all of them but by layering them and mixing them having that variety it can give you a nice base
[30:44] look and we haven't even used our brush yet that's gonna come later gotta be careful not to because
[30:48] i tend to do this not to go too long and just never use your brush and it's just everything's
[30:54] procedural that has a look to it too so adding paint masks to these coming in wiping away again
[31:01] you can do that at the end when you see it in context but that's the kind of thing that really
[31:05] makes it you know the hand the manual you know finessing at the end let's start texturing our


### Plastic [31:10]
**Transcript (timestamped):**
[31:12] plastics all right we're gonna set up our our base for plastics and we're gonna have a couple
[31:16] different colors we'll add some nuance so that you know there's a little bit more life and
[31:20] the plastics of our helmet okay so here's some some techniques on how i do that all right so
[31:25] why don't we turn on our plastic fill layer this is what we had before just basic right so start
[31:30] adding some more nuance to this now we want to get a little bit more detailed here right now this
[31:37] is our base plastic so let's start adding some different types of plastics that's really what
[31:43] we need we need variety and so let's start with um let's just change this to rubber so we'll call
[31:52] this rubber is it really rubber i don't know but it's going to be uh actually let's see if we can
[31:57] use that material rubber raw there you go we're using actual material here rubber raw and then
[32:03] we'll make this uh black for later all right rubber raw here we go pretty cool right already
[32:10] getting a lot of stuff for free okay we need to change this from UV able to do triplanar uh so
[32:14] that goes across seams and then for tiling uh we can change that to 10 all right and then roughness
[32:22] variation i'm gonna drop that down a little bit here and then the height range we're gonna drop
[32:28] that down quite a bit so the height range it's at 0.2 now we'll do 0.05 so it's like a fraction of it
[32:35] there you go and then the roughness variation maybe it's still too much that's the roughness variation
[32:41] at zero already getting into a little bit more tricky stuff i don't like this uh roughness variation
[32:46] so i'm gonna add a levels and i'm gonna do just the roughness and then i'm gonna i'm gonna bring up
[32:51] we're gonna bring these in so there's like less variation because i'm gonna add my own variation
[32:56] you know what i mean all right so already looking better right guys look at that already looking
[33:00] better wow you know i love these little things that happen on there i love little happy accidents
[33:04] like that okay so there we go let's add a new thing well maybe we'll mask this where should this go
[33:10] yeah maybe up there would be good too so why don't we go to our plastic let's add some more stuff here
[33:15] all right we got our plastics here let's do this too actually we're gonna use our uv selection for
[33:22] this mask oh no we're not we're going to we have to use our where is that one i have to use our
[33:29] polygon selection i guess all right so i want plastic all the way around but not the actual
[33:36] center so we're gonna do this i should have just split this in the uvs but i didn't and here we are
[33:43] and this can be a lot of what texturing is so we're we're growing our mask our overall plastic
[33:49] material mask okay so we've got some plastics cooking here uh all right let's add a a new one
[33:55] let's go black shiny let's do this one and call it black shiny all right and then for black shiny
[34:04] let's do this height we'll make it zero i don't think we need metalness anymore because we have
[34:10] the base below right so we're gonna make this pretty dark let's say uh for the base color 0.15
[34:16] and then for roughness we want to be shiny don't we so how about 0.15 pretty shiny huh and then
[34:23] height for zero and then we're gonna want to replace that so remember if we're in our height
[34:28] normally you know you default to the base color but we want to change this to height and instead of
[34:33] letting our dodge we're gonna go replace and that didn't do anything i did something but i think um
[34:40] i think our rubber on the topic of layer blends okay just to recap because i don't know people might
[34:46] skip or skip around right this is just an important thing to understand with substance painter that's
[34:50] unique to substance painter okay that's why i want to harp on this you have the different
[34:56] channels base color height roughness those are different layers stacks here that have different
[35:02] parameters right here on the right the blend mode the opacities and you have to jump around
[35:08] okay to edit those now what's happening here is the metal down below look at that the metal
[35:16] height information down below is still there and that's because folders by default are not set to
[35:25] pass through they're just set to normal pass through means it's affecting everything below it so
[35:31] i'm on base color now right so if i change this to pass through then it sets the folders blend mode
[35:38] to pass through just for base color but we want it for height that'd be kind of a pain in the butt
[35:43] to go to each of these right so here's something that took me way too long to learn that you're
[35:47] gonna know right now if you right click on it you can apply to all channels and look at that
[35:53] we just replaced the height and why did that work because first of all that right click apply to all
[35:57] channels you're i'm gonna use that a lot more in this demo but you just use that all the time so
[36:01] that's because in here we have our black shiny height zero replace so now if i jump over to height
[36:07] you can see it's on passive it's on pass through now in all channels so now my height is set to
[36:11] replace you can see now i can actually see there's the metal now my rubber is on top now my black
[36:18] shiny is on top of that so that's the only way to get this stuff to work you have to make sure you
[36:22] understand how these things interact and again we're gonna do this over and over again that way
[36:26] in case you're into that and i'm sorry for the people that already know all that stuff because
[36:29] it's probably boring boring to death but this is super crucial i think this trips a lot of people
[36:32] up okay so there's black and shiny all righty uh so let's make some shiny stuff do a black mask
[36:39] and then add paint and this is fun now that everything's set up we can just go do you know so
[36:44] i think making the little tubes shiny is cool and then maybe this thing all right it's good enough
[36:53] this thing's a little bit distracting this background i know it's brighter better or not i don't
[36:57] know i'm gonna say no all right now it's nice and shiny cool okay good enough for now let's add a
[37:05] new plastic we're gonna do gray all right let's set up our gray plastic base color i'm gonna set it to
[37:13] if i don't know what to do i either do 755 3 3 2 5 something like that roughness 0.55 remember
[37:20] this stuff's all non-destructive right that's why it's so cool okay and then um all right let's
[37:26] set a mask to this black mask paint let's start clicking stuff this will be gray plastic um
[37:34] this will be gray plastic that'll be great plastic this will be great plastic like we're
[37:38] making two-tone stuff now guys okay a little more interesting now and then this little strip up here
[37:44] can be gray for now so there you go now we got a little gray plastic going on looking cool
[37:50] looking cool and then we do need our little button here we need red plastic um why don't i just
[37:58] duplicate black shiny because it already has the replace on there let's call it red and then for
[38:05] this we need roughness we'll make it less shiny because it's not as shiny as it and then we'll do
[38:12] red and then we'll delete that one and we'll add our new paint layer and we'll choose our button
[38:17] there we go so now we have our button there you go now before we dip out we did some more
[38:24] materials with like you know we probably want some scratches don't we so let's see here let's do um
[38:31] you're we'll zoom in here so we could see so let's add a new fill layer we'll call it scratches
[38:36] and then we're gonna set we're gonna go to base color and we're gonna set the blend mode to overlay
[38:43] oh can't see anything because of this value we need to go white and then let's do roughness add
[38:50] point seven so it's getting rough too okay because that's how we're saying the the plastic gets worn
[38:55] it gets more rough then we're gonna add a smart mask all right there's a new thing too so these
[39:01] things you can see smart masks now we'll search for paint subtle paint subtle scratch is a good one
[39:08] we can just drag this right on the mask thing and boom smart masks are like uh smart layers
[39:14] smart materials where it just saves all the stuff we've been adding we've been adding these
[39:18] manually one by one right and you can save whatever you want as your own smart mask but
[39:22] substance comes with some so there you go now you can see so we're already cooking with something
[39:26] which is cool it is the inverse of what we want so we can we can flip that we'll do global invert
[39:33] true and then we're gonna add a sharpen to this too and now you can come in here and you can change
[39:39] whatever you want you know if you want it to be less and then you can also set the uh value instead
[39:44] of one you know you could do point nine five or point nine two or something like that so it's just
[39:48] more subtle right there you go now at least it doesn't look like brand new plastic it's got some
[39:54] some life there and then even the uh you have some things in here too that are like subtracting
[39:59] those just scratches okay what about this so now i'm just editing what's already there but that way
[40:04] i'm getting less of the the worn uh plastic everywhere right it's kind of like making a
[40:09] little bit more subtle all right as you can see i can i could literally just do this all day long
[40:13] so we'll stop right there there you go here's some plastic why don't we go jump into ira
[40:18] see what it looks like with some actual rendering got a few different plastics cooking we've got some
[40:22] wear you know so we've got some interest in here good thing to start with because then from here
[40:27] we can add more and more handmade stuff and then you know we can curate it you know more from here
[40:32] we're gonna add dirt and all that kind of stuff but just flushing out our plastic material layer
[40:36] it's looking good and so next we're gonna talk about paint we're gonna do some of the similar


### Paint [40:38]
**Transcript (timestamped):**
[40:42] techniques essentially we've we've covered the essentials now fill layers filters generators
[40:47] smart masks blend modes folders that kind of stuff right you're gonna use time and time again
[40:51] now we're gonna introduce anchors for the first time and powerful and it's really cool and we're
[40:56] gonna do some tricky stuff with that so next let's talk about paint all right so now inside our
[41:03] paint folder we're gonna create another folder inception dude so we're gonna go paint colors now
[41:12] and then inside of our paint colors we're gonna do all the colors we think we want for our again
[41:18] this is gonna be different for you so we're definitely gonna want a red we'll come back to that
[41:23] but we're gonna want orange and we can just set that real quick let's do orange and then we'll do
[41:31] a roughness at 0.25 seems like okay for paint maybe it's a little bit polished but should be okay
[41:40] and then we can duplicate this we can do blue there you go so we have red blue and orange
[41:50] okay red blue and orange cool all right so we'll call this red okay so let's do blue let's make our
[41:56] blue color and that's gonna be like a baby blue kind of okay cool now let's set our masks so for
[42:04] orange we're just gonna have probably just one little panel I guess there's our orange for now
[42:10] and then for blue we're gonna want a couple different things so we're gonna do this I'm adding
[42:19] more blue now all right and then yeah so blue's gonna come here too so we've been adding layers like
[42:26] this now I'm gonna add a little something different we're gonna add some detail so that it looks like
[42:35] it's paint and I'll set that up before I do the painting so you can kind of see or maybe I'll just
[42:42] do a little bit first okay cool so now I'm gonna actually like paint this as if I'm spray painting
[42:48] I'll turn mirror on so that's on both sides as you can see and then I'm actually just gonna like
[42:52] as if I'm airbrushing this okay so I'm gonna do this I'm gonna come in here and I won't finish
[42:58] so you can see but so I'm painting all this and then this and I'll do some more in a sec so let's
[43:03] say I do this okay so here's my little my little paint job I'm gonna add some stuff to this to help
[43:08] me make this look like a spray paint look so check it out we'll do a fill layer and I'll do
[43:14] Gaussian spots I mean sorry Gaussian spots Gaussian spots two probably good is that this one no two
[43:22] yeah so more speckles right and then UV projections probably fine for this wait we want this to be
[43:29] tiny though balance is gonna be like nine five scale there we go see this tiny spots everywhere
[43:36] it's gonna look like you know like spray paint on the edges now if I set this blend mode to soft light
[43:42] see what you see the gradients become speckled see and now that this is set up though I can like
[43:49] you can literally just come in here and spray paint more it's pretty cool right see it's pretty cool
[43:53] I like doing that all right and then you can even clamp this so like if I set a levels you
[43:59] kind of improve the look a little bit even so if I brought in the white I could bring it to uh I don't
[44:05] know .9 see I mean it gets a little bit more full feels a little bit more opaque and then you know you
[44:12] could do um there's a brush early like called smooth noisy that's what I use when I actually
[44:16] just want to fade stuff so then it's got it just is like just dots you know now because of the because
[44:22] of how it's set up it just looks like dots I was trying to make it look a little interesting you
[44:25] know next what I'm going to talk about is this sort of advanced anchor setup advanced I'm just
[44:31] saying that because it's going to get a little tricky but this is probably not that advanced
[44:33] you're going to see some after this you're going to see this a lot so when I when I'm texturing I
[44:38] use anchors a lot and I use this new filter called bevel smooth a lot and so we're going to be using
[44:43] that quite a bit so what I want to do I want to create a single layer that lets me with my brush
[44:50] paint where paint chips happen and then I can add even a filter on there and then that's going to
[44:55] cause paint chips okay essentially a simple black and white mask that is creating complex paint
[45:03] chipping effects that have like an uneven height that have primer that has in a regular chipped
[45:12] edge but all I'm doing is just with gradients and with a brush and with generators saying where that
[45:18] stuff goes okay and so to do that we can use anchors that's going to drive things and use it as
[45:22] references that we're going to create that layer that's meant to drive that effect okay and you'll
[45:27] see as we if you're new to this you'll see as we set it up and I'll try to name everything accordingly
[45:31] so that you can follow along and you set this up really fun there's a million ways to use this kind
[45:35] of thing but I think this is a great way to show it okay so now I'm going to create a new paint layer
[45:41] we want that to be in the folder which is always very confusing there you go in the folder and we'll
[45:46] name this new paint layer because we usually use fill layers this is just going to be called our paint
[45:52] mask control all right now this layer is just going to be used to drive everything above because
[45:57] we're going to use anchors now instead for this paint mask control what I'm going to do is I'm
[46:02] going to add a black mask and now I'm going to move this paint layer to below remember this paint
[46:08] layer we made before we put it on the folder up here to show where paint goes right but we want
[46:14] to drive this with an anchor so we can do all kinds of effects and the way the anchors work
[46:18] is they have to be below everything that references it I can only reference things that are layered
[46:23] below me that's why I'm putting this paint mask control at the bottom now I'm going to add an
[46:28] anchor point and that makes this new paint mask control mask okay that's confusing but it's okay
[46:34] so now I'm going to add a fill layer you know back to that paint folder because it doesn't have one
[46:38] anymore but if I go in here and I and I select my newly created anchor point I'll have the same
[46:43] results as before but the difference is this mask is now being driven by this as you can see right
[46:51] if I remove if I paint down here it removes it from up there okay so now we have a working
[46:57] anchor point setup so let's start removing the paint now which again right I'm I'm I'm actually
[47:04] editing the full right here the folder of paint because this is my anchor so uh anchor result
[47:12] so now let's add some more cool stuff to this everything has to be underneath this anchor this
[47:17] so let's add it let's add a curvature drag that down below and then we're going to set this then
[47:21] to multiply and why don't we highlight this so we can see all right global invert true
[47:29] because we're just want to remove the edges don't we and then mode open this up mode edges that's good
[47:36] global balance point and it's getting way up there yeah and then sharp one always one love some sharp
[47:43] point five two something like that and then soft maybe point three something like that and then
[47:50] let's get rid of these all get rid of these guys there you go all right and then let's add some more
[47:57] break up let's use a texture we get learn some more about our curvature generator which again I
[48:02] use it all the time with all kinds of stuff so get used to this here we use it we'll use a texture
[48:07] texture opacity want that to be one and then let's do the image input right here let's do
[48:15] a grunge concrete yeah grunge concrete burnt and then contrast let's get that up there and then
[48:26] yeah so that's before and that's after and then how we looking back this off a little bit we don't
[48:32] want the the face is gone yet but here you go yeah and then let's get some more let's do more
[48:38] let's add a metal edge where that'd be good yeah metal edge where metal edge where there you go
[48:47] we'll drag that right into our stack right above curvature and we're going to set that to multiply
[48:53] two and then let's do some stuff here so global invert true again and then wear level a little bit
[49:00] more wear contrast fine grunge amount 0.3 fine grunge scale for good smoothness one that's all
[49:09] right a o masking 0.5 okay okay good it's got a little bit more crispiness there I got some
[49:16] more detail now so we're good for now let's keep going okay now we're gonna add some complexity
[49:24] here instead of our anchor just driving one folder we're gonna use that anchor we're gonna drive a
[49:29] couple different things now so and so that we can offset them and mix them together so let's
[49:34] follow here we're gonna make our primer that we just made we'll have that be driven by our mask
[49:40] here's our new primer right so let's add a mask here and then we're gonna add a fill
[49:45] and we're gonna choose our anchor and we're gonna add a mask to our colors i'm gonna add a fill
[49:51] and we use our our mask so if we turn i wonder if we can just remove the whole folder so now if we
[49:57] remove the mask from the folder what do we got here we go so now if you see what we got here
[50:05] i think i'll just set this to pass through on all channels so now our folder for paint is literally
[50:10] a container now we have colors and primer being driven by this paint mask control make sense here
[50:17] i'll make this red so you can see like or maybe can i make it orange again so it's like yeah look at
[50:21] that looks like an anchor look at that oh such organization such color coding so now we have
[50:26] similar result right but now we can start getting freaky with it we can start getting
[50:29] jiggy with it now okay so let's offset some stuff with the paint color so you can actually see
[50:36] the primer because right now they're the exact same mask right so just want you to to know what this
[50:42] is all right so for the paint colors here we're gonna add my favorite new filter bevel smooth
[50:49] if we just filter everything you can see here right here bevel smooth looks like that
[50:53] i use this a lot and this is somewhat new so i don't know what i was doing before but anyways
[50:58] i use this all the time now so i'll do 0.0095 sure and then smoothing we'll make that zero
[51:05] curve offsets we're gonna do negative 0.15 curve shape i'll do negative one mask threshold
[51:13] will be 2.17 and now look at that what's happening now we're offsetting it and now we're seeing the
[51:18] primer poke through you know all right so there's that then let's do a warp filter so we can so it's
[51:25] not just a you know like an extrude it's actually different so we'll add a filter and then we'll do
[51:32] a warp there you go warp all right uh intensity we'll do pretty low and then blur pretty high
[51:43] see now we're getting thicks and thins you see that before it's like uniform and now it's a
[51:48] little different and then let's do a sharpen on this all right so we've got our edge where now
[51:55] let's add more more now we're gonna do another primer because because it's cool that's why we'll
[52:03] add a new fill layer called light primer we're so smart light primer so this one gonna be lighter
[52:11] let's do uh and then let's see here let's see here uh roughness 0.6 again same dealio
[52:22] all right and then i guess both of these just to be safe i'm gonna do metal zero just because they
[52:27] might be probably fine but just in case um we need to override the the metal below why not
[52:33] okay so let's create a black mask on this one and then we're gonna fill it with the anchor again
[52:39] and then we're gonna start doing some some stuff again so let's do our let's go back to our our
[52:44] stash here good old bevel smooth and then we'll do out we'll do distance 0.01 that's good smoothing
[52:52] 1.75 uh let's offset the curve that away negative 0.78 it's what i'm doing curve shape negative one
[53:00] and then mask threshold we'll do 0.43 all right and then we'll do a warp filter on this one too
[53:07] so we'll do a warp filter here on this and then intensity let's do 0.25 and then see source blur
[53:17] one let's go crazy uh source balance 0.75 and tiling five uh distance 0.01 oh 0.01 so look at
[53:27] that we got some pretty cool interest now don't we i don't know pretty cool all right and then what
[53:32] we're gonna do here we got some warping and now we're gonna do um the light primer we're gonna
[53:36] introduce a new another new node that's uh pretty useful and that's quantize that's gonna let you set
[53:43] it's kind of like uh whatever they call it in photoshop can't remember but essentially you know
[53:49] you turn it into like right now i've set this to three and it'll just turn it into three colors
[53:55] so there you go let's see what's this looking like i need to put a filter uh sharpen on there too but
[54:00] looks like paint that's worn away cool and then now what's cool though is we got some complicated
[54:07] edges and we can we can edit this stuff watch so i can come in here and then this is the paint mask
[54:13] control layer remember so i can um i'll say this is like i don't know regions okay and then i can add
[54:20] a paint to this and then just freestyle right i can say you know what storytelling hat on right i can
[54:29] say well it's not gonna get worn too bad so we can like come in here and just say you know what it's
[54:34] gonna be okay right here and it'll be uh okay right here so i'm picking and choosing where the where
[54:43] i want the where to be and come back and go away and stuff like that so these two like maybe these
[54:48] two little things that's each other they don't wear that much all right like around here it doesn't
[54:53] wear that much around here it doesn't wear that much and then i can also i should be able to
[54:59] so you can see i can actually come in here and remove the paint i'm gonna say it burns in here
[55:05] you know so just i'm gonna remove all the paint from there but if you see like it keeps my edits
[55:10] so that i don't ever have just a you know a stroke it still kind of looks like paint chipping see
[55:16] what i mean and if i get in the more gradients i get the better i'll come in here and i'll do
[55:21] my smooth noisy brush which i use a lot i can add some paint back so i'm just getting primer now
[55:27] and i keep going because of the gradients now i'm getting the paint back see that and i'm getting
[55:31] that nuance and then i can say maybe um here i'll just bring back some so i can actually like watch
[55:39] this line get thinner it'll start filling in with primer same thing right here like maybe
[55:44] don't want that all right so you can just do this till the cows come home as they say
[55:50] and then also um is this separate i don't like that uh part coming back so
[55:59] all right anyways so that's our that's our paint layer on top right and then um again like with the
[56:04] metal edge where we could get some more stuff maybe get some more random things like this
[56:11] you know little pops here and there all right okay cool so that's how this paint control thing
[56:17] works now let's keep adding more nuance to our paint texturing let's add dirt and wear at the top
[56:26] okay let's start adding dirt and we're gonna add dirt to our paint colors we're actually just gonna
[56:31] add more dirt we're gonna add stuff in here so let's do a new one called dirt and then we'll do
[56:38] kind of a yellowish brownish color roughness more roughness 0.7 all right and then we'll
[56:46] create a black mask on the dirt and then let's check this out let's do kind of generator that's
[56:52] that's cool that you can use in your stuff called tile generator there you go it looks like this with
[56:57] the grids and then with this you can do all kinds of custom stuff so i can say um we're gonna do type
[57:06] type custom image input we're gonna tile a custom image and right here for the image pattern
[57:14] we're gonna use an image that we have called dirt stain large okay so there you go you can see it's
[57:20] tiling now and then we have all kinds of controls so i'm gonna change this resolution i don't know
[57:26] if this really does anything but that would suck if it does so i'm just doing it and then let's see
[57:31] we'll do over here let's do hardness are we good this hardness shape that's fine maybe maybe less
[57:38] hard i don't know all right so let's do a bunch of random stuff that's why this is cool so we'll
[57:43] do random rotation we'll do symmetry random rotation random again and then scale it's our scale here
[57:56] it's going to size i can just type in six even though i can't scale it i can type it in see what
[58:03] i mean so yeah now we use this image you can do whatever image you want you can imagine a ton of
[58:07] ways you could use this thing but like you know by using this source now we're getting all this so
[58:12] yeah we got a bunch of random stuff on here here you go and then we'll add a filter at our sharpen
[58:17] trusty sharpen make it look nicer and then we might need to make this or we could make it just
[58:24] not that opaque if we made it kind of maybe we make it less hard it should be down here in the image
[58:33] input so we definitely get a little muddy now and then i'm thinking um all right we're gonna over
[58:41] crank this call it a day and move on let's go to eight all right we'll say that's good for now we're
[58:48] gonna add more and more dirt to this too so we're just trying to make the paint look a little messed
[58:52] up all right uh so yeah that's that now let's do let's add another one and see how they mix together
[58:58] let's do one called stains okay so that was tile generator uh now let's do
[59:05] another kind of warmish middle tone and this one we'll call well this one will actually do multiply
[59:13] for sure do base color multiply and then we'll set the roughness to 0.5 again roughness variation
[59:21] you always want a bunch of detail in your roughness okay and then we'll add a black mask let's do
[59:26] another smart mask let's do smart mask and we've got something called dust stain drag that on there
[59:32] all right and then texture scale we're gonna want to change that uh let's do texture scale
[59:40] we're gonna change this uh we're gonna make this one that is our stains let's see what's it looking
[59:48] like and then always by the way you know you can come in here um for your seed you know for whatever
[59:54] is driving your thing i'm not sure what maybe it's this one whichever one you can click it and it'll
[59:59] it'll update the random thing so if you don't like the random shapes that are coming out you can
[60:04] click it a few times until it just re-rolls the dice if if you know what i mean let's do more we'll
[60:10] do shiny stains now so this one's gonna be a lot more targeted for the roughness let's do shiny
[60:14] stains you can see similar to the other materials we've been doing layering things up right over and
[60:20] over and over again here we're gonna do up there and then we're gonna do base color multiply again
[60:27] and then we're gonna do roughness here's where this one happens this is where the magic happens on
[60:31] this one it's point one so pretty shiny all right and then we're gonna add a black mask to this one
[60:37] because these same things over and over right this is it all right then now we'll do a fill and
[60:41] we'll add a grunge map over here we'll type in this one's called runge map 07 007 okay again
[60:49] let's take a look at the mask as we build it so this is that tiling we're gonna do four and that's
[60:55] on each piece um you know you could do the fit match per tile you could do triplanar and it would
[61:02] go across everything so yeah it's whatever you prefer i could keep triplanar for now it'll look
[61:08] more like it's on the whole helmet all right so then uh balance we'll do point four one and then
[61:16] it's looking a little sweatier a little grimeier right what happened here oh we need to we need to
[61:21] turn these other things on dude so it doesn't look crazy and then maybe the inside of the helmet
[61:26] i'll make just plastic just so we don't have to stare at this thing the whole time back to our
[61:32] paint so that was our shiny stains okay so we got some stains and they're shiny now we're gonna do
[61:38] more actual just roughness variation let's just call that roughness variation okay and then roughness
[61:45] we're just gonna crank it to one don't normally do this folks here i'll just do it i'll just do
[61:49] 2.9 just to not break my own rule you don't really nothing's ever fully won and then we'll
[61:54] add a black mask and then we'll do some more noise let's go fill and then purlin noise uh let's do
[62:02] the 3d purlin noise and then we'll do fit match for tile and then for contrast we'll do point one
[62:09] six scale with the 30 and then distortion intensity we'll do point three five for that and then
[62:18] layer opacity and that's going to be in the roughness don't you know so in the actual roughness
[62:25] channel why don't we do it in the mask we'll do it in the mask in the mask we'll lower this opacity
[62:31] a little bit and then we're gonna add more stuff let's do fingerprints that's fun we'll do fill
[62:37] we'll use it again on on glass probably but we'll do fingerprints smeared is a good one right and
[62:43] there's a bunch of these grunge fingerprints smear sure okay and then we'll do um triplanar
[62:50] projection for this one and for tiling maybe four balance go a little bit up but then we'll make this
[62:59] overlay so now we're doing blend modes on the freaking blend modes do you know look at that now
[63:04] there's blend modes in the mask assignment you know it's crazy and then for this uh we could also change
[63:12] the the opacity for this one if we want to so we want to just mix a little bit again this is for
[63:19] roughness so so can you even see it as the question a little bit right so here we'll jump in to our
[63:26] renderer so we can take a look in fact let's do uh you know we've been using this soft white so we
[63:33] could see but let's let's get an actual a-stri in here with some nuance okay so here you go so now
[63:39] you can see with the glancing eels and stuff we've got a lot more stuff going on okay so things are
[63:44] are um feeling less flat and they got more dimension stuff and that's good now let's let's create a new
[63:53] layer just to add some edge discoloration on our paint now again this is in that category of like
[63:59] looking fancy you know just to separate the elements more make it more readable almost like a burnt
[64:05] paper edge so that's not necessarily uh realistic depends on how the wear is happening but it's
[64:12] another way we can emphasize the shape so let's let's do that now we're going to create a new fill
[64:15] layer for our paint and we're going to call it edges and then we're going to do multiply here
[64:23] what are we at here supply oops that's supposed to be in the base color we gotta do that multiply
[64:31] all right and then we're going to do i guess a little bit less opacity let's add our black
[64:37] mask to this and then we'll do curvature and let's do some of these things so global blur i don't
[64:45] know we'll see balance 0.3 contrast a little bit and then we're going to do mode as edges sharp one
[64:55] always soft that's good medium that's fine so now we have these edges getting darker okay so kind of
[65:04] like gets darker as it gets closer to the metal and helps pop it out a little bit okay little nuance
[65:10] okay let's do another layer this one we'll call dust and then we'll add a black mask and then we'll
[65:18] just do grunge grunge dusty scratch yeah i'm gonna just i'm gonna just call that a day what do you
[65:27] think about that it's a little blurry though i guess it's a little blurry i guess uh match
[65:34] uh that didn't really help did it i'm tiling them out and then probably should sharpen it too
[65:39] it's kind of low low res get ready to just flip this random seed a little bit till we like it this
[65:45] seems better all right there we go now we're cooking this up pretty good what do you think pretty
[65:50] good looking like a dirty helmet all right now the finishing touch some edge detail all right this
[65:59] is going to help this look more like paint and uh once we get this to i'll play i'll show you can
[66:03] play around you can do a million things with this but uh here's kind of last piece of the puzzle here
[66:07] and this is a pretty cool thing too so check this out we're going to do our edge detail now so we
[66:12] need to create a new fill layer uh at the very top of the folder of our uh yeah of our thing called
[66:20] paint edges all right so probably in paint colors right let's do it let's do the very top here we'll
[66:25] do we'll just call this paint edges all right we'll keep the bc like that and then the height
[66:33] we'll do point one or point oh we'll do point o2 so we can see for now and then the opacity
[66:42] we'll keep and then here we go out of black mask let's get our anchor our magic anchor and then
[66:50] let's see what we're let's see what we're doing now we're going to do a mask outline so we're going to
[66:56] go filter mask outline and we're going to change it to got outside threshold we're going to go zero
[67:05] width we'll do point oh three blur zero curve shape and like negative six five or something like that
[67:13] all right let's keep this like this for now this paint layer below is is uh too harsh so maybe we'll
[67:20] maybe we need to do our corrections later let's get this set up so we can see what it looks like
[67:24] all right so we got negative there and then let's see what's looking like right now
[67:28] we'll probably set this to replace on everything and then choose this one paint colors mask now we
[67:35] got to do something else to make this work right um so we're going to do let's see so we need to do
[67:42] what's this doing okay like that okay that's not too bad okay so we need to width width like that
[67:49] okay like that maybe do a little blur I suppose and then we need to make this cleaner we need to add
[67:56] another fill layer and choose that same anchor point get my anchor again can I set it to multiply
[68:04] okay so that that's gonna remove it does that make sense here watch I'll show you the mask
[68:10] so here's my paint colors anchor I just grab right an anchor here on all my paint colors
[68:18] so that's everything except my uh primer because I just want to peel the paint up right so then I'm
[68:25] with this layer that's just going to be the edges the height I have in my fill layer my paint colors
[68:30] anchor so now it's just gonna be the same as this mask right now I'm gonna use this mask
[68:34] outline to create this shape and we can even blur it some more and you know we could do some some
[68:39] interesting stuff I suppose and this threshold is gonna let me like move it here is the same same
[68:45] thing again you see paint colors mask and I'm setting it to multiply that stamps out the middle
[68:51] so now you just have this in between see what I mean now we're just gonna have this kind of
[68:57] edge so I'm gonna do a warp we'll play with this some more I might just use bevel smooth honestly
[69:05] I love bevel smooth but let's do warp just to get this all set up we're just wanting like an
[69:09] irregular edge here so we're just gonna do something kind of subtle we'll do a source blur and then
[69:16] we'll do some tiling and then the intensity and then we'll do a little blur here these are both
[69:21] gonna go above whatever that ends up being not having the best luck with the outline so we'll see
[69:28] and then the blur we'll just do point one just take the edge off of it and then this doesn't have
[69:32] to be that okay so here is it with the mask outline so now again without the punch out on top right
[69:38] the negative it doesn't it loses the sharpness which is okay because we're blurring the edge we're
[69:43] trying to get to curl up then we punch it back out it should look like it's uh kind of peeling
[69:48] up that makes sense and then the warp is what gets us to like lose it you know so that matches
[69:55] it perfect but now with with our little warp we can kind of have it just be a little bit different
[69:59] kind of looks like it's curling up at different places you know I'm saying give it some more
[70:02] unevenness okay and then maybe like what if we blurted a lot yeah see that's like no blur at all
[70:08] and we can kind of just kind of fading a little bit let's see if I can get this just to come more
[70:13] so width is point one can I yeah it's the most I can do okay probably something like this and then
[70:19] I'm gonna lower the height to be pretty subtle or maybe maybe make it if I keep it big and then
[70:24] with the threshold I make it so it's just the big shapes that's probably the best way to do it get
[70:30] a little bit of the holes and then yeah we'll do point oh three I guess or something like that
[70:35] all right so let's see what we got cooking here and then and then now we have like everything
[70:41] open to us too we can go back on the shiny parts and everything I won't now because I will just keep
[70:45] adding stuff but yeah we're getting we're cooking now let's see with the render okay so we're getting
[70:49] some nuance in these areas there you go and then we can mess around with adding paint back in there
[70:55] and stuff maybe we even make this the edge is more rough if we want I know we have in our metal we
[71:01] have our shiny metal I wonder if we invert that let's do curvature weight here we go that way
[71:09] that way our shininess not so much contrast we have contrast with the paint already so just
[71:13] want a regularity with the metal so I think that feels better we're cooking now okay so now we have
[71:20] our paint set up we've got our paint edges and colors and primer we'll keep going but you could
[71:29] you know paint in and out of all these different layers you could add paint back here maybe I could
[71:34] show that so everything's being driven by this right here's that paint layer back if we add it
[71:39] okay so I can say like in this area you know you can like very much with like a spot fix it
[71:45] say like you know where doesn't happen right here so we should get rid of it and then maybe
[71:51] maybe there's even a way to show so like yeah maybe I think it'd be cooler too with some
[71:56] something with like more opacity and and then I'll do with my flow here come in here we'll add
[72:03] nuance just by coming and adding some more back in here right like we'll just say it doesn't get
[72:10] worn here as much you know in the corner okay so we're getting some some stuff back there here
[72:16] we'll just say okay it gets worn there sure catch some edges you know and then but maybe right here
[72:23] it doesn't so much just by painting in and out you can have a little bit more control
[72:30] maybe we wear it a lot right there but then maybe right here we'll bring it back in the middle
[72:35] so I'm just using the sandpaper brush because I can vary the pressure and also it's got a pattern
[72:40] to it so just it's adding just more detail for this thing to pick up because we have all those layers
[72:45] on top you know we've got some bevel smooths and some because everything's picking up from this
[72:50] anchor point so it's a little laggy to paint but all that complicated stuff is happening with the
[72:55] primer offsets and everything too so as I paint primer starts to come back the more I paint the
[73:01] other primer and then and then the paint and everything has these irregular edges and warps
[73:05] and stuff like that so I can really just control where you know I think the where should be and
[73:10] then I could bring it back in some other areas and yeah there you go so I'm you know getting a real
[73:16] complexity here like I don't think it should wear here so I'll just come in here and I'll just add
[73:21] a bunch back here and then we still have that global control remember we this you know underneath
[73:26] this paint layer is a generator and a curvature and we could reduce the balance so there's like
[73:34] these few knobs if you know where to look where you can just make these big global changes and
[73:38] that's ultimately why you know this workflow is so powerful all right so there you go with the paint
[73:45] now I want to talk about texturing kind of metal coatings you know there's times where you're doing


### Metal Coating [73:47]
**Transcript (timestamped):**
[73:52] certain kind of sci-fi weapons or armor and stuff and you want to do these black things that are
[73:58] hard surface metallic type things so we're going to do sort of a fake coating and to do that we're
[74:03] going to take a look and use an example this little flashlight piece on this helmet all right so to
[74:10] start we're going to create a new folder for a material we don't have yet and we'll call this
[74:15] coating and we'll keep uh we'll keep the little uh system we have going on by choosing a new color
[74:23] okay and then inside our coating folder we'll make a new fill layer we'll just call it base coating
[74:31] keep it going and then let's see we'll do something dark like this and now with the coating we're
[74:39] going to break pbr a little bit we're going to do some roughness and then for metallic I'm actually
[74:44] not going to do full black or full metallic I'm going to do kind of in the middle so I'm going to
[74:47] do something like 0.6 so this isn't true pbr but this is a way that we can make things look like
[74:53] there's like metallic in the flakes or metallic paint or something you know that it's not 100
[74:57] percent there and it could keep this looking hard surface all right so now we're going to make a mask
[75:04] for our coating layer and uh actually we should probably set our folder remember we're doing our
[75:10] layer blending you know our good good practice here the way I'm using folders and everything I know
[75:15] that I want my folder to be passed through for everything all right we're going to keep it for
[75:19] our base we're going to keep this we'll keep it passed through uh let's do a paint layer so do black
[75:25] mask on our coating folder we'll go to paint and then we're going to select some of this stuff so
[75:31] we're going to do the whole light piece for sure we'll do this thing and then maybe uh while we're
[75:37] at it we'll do this and then uh this guy that the little maybe the uv there we go we'll do that maybe
[75:43] this guy we can do and then I don't know anything in here maybe I'll just do this for now so we've
[75:50] got three things going on right now then this because this could be kind of metallic and maybe
[75:53] this one so I got even more stuff going on okay let's work on this now all right so we are going to
[76:00] do uh curvature yeah let's do a curvature on the coating so on our mask we're going to do
[76:10] curvature all right and we're going to set that to multiply and then let's open up our
[76:15] curvature settings here we go again global invert true because again let's just check a look at the
[76:20] mask right we're just gonna we're just gonna wear away the edges right global blur blur zero
[76:25] balance of point five is fine contrast point five and then for the curvature stuff we want sharp
[76:34] yeah we're gonna do edges uh fine we're gonna do point four something soft let's go less than that
[76:40] and then medium even less than that it's often like a stair step usually okay we'll get rid of this
[76:46] stuff there you go so it's a little tighter okay and then maybe we'll add a little blur to this
[76:52] try to integrate it a little bit more and then we'll do a grunge let's add fill and we'll do grunge
[77:02] dirt scratchy that's a that's a good one right here scratchy yeah like this one yeah yeah yeah
[77:07] all right and then for tiling we'll get it tinier something like that's pretty good balance maybe
[77:14] down here we go and then contrast and then we'll set this to overlay this is gonna help give us some
[77:21] detail in those gradients there you go and then we'll do even more stuff let's do you'll see this is
[77:28] how i build a bottom mask you can see the the repeated patterns here right let's do uh grunge
[77:34] scratches rough where's this this one grunge scratch it grunge scratches okay and then again
[77:42] multiply and then we need to change this to be a lot smaller obviously right so tiling two
[77:50] a global invert and then cerebellum contrast give it a little bit of contrast
[77:57] scratches tiling we want tiling more scratches dirtiness let's see for our dirtiness we'll go
[78:05] all the way one double scratch we'll go one scratch spots intensity well i don't like that that much
[78:12] that's kind of like the noisiness in there and then dust intensity no so there you go now we got some
[78:17] chips so if i show you here here we go so it was still um a little blurry and that's where we can
[78:24] we can do something else but let's keep going right now so we're gonna create a new okay so this
[78:29] is blurry right so to get us the look we want let's let's use threshold you guys might be familiar
[78:36] threshold photoshop but it's gonna crunch it makes it more binary you see and then we'll just do
[78:41] point uh i mean you can just see what you want really see this helps it look like it's a coating
[78:46] that just got messed up and then maybe this i like the blur a little bit much though but okay and
[78:51] then threshold really lets us like say how much is dinged up or not you know and then for scratches
[78:58] i wonder if we can just add a lot more that's pretty good like that just little dings here in
[79:03] there cool i think it's okay all right now in our folder let's add some more detail to this
[79:09] coating okay so we've got something probably seen things like that they get worn okay now in our
[79:13] coating later we have our base coating let's add some more stuff let's add a fill layer and we'll
[79:18] call this flakes all right and then now let's do some height in here we'll do .02 and then let's add
[79:25] a black mask on here and then we'll just view this mask we're gonna do a fill called gradient flakes
[79:34] okay gradient flakes there we go and then let's see we'll do this a tri-planar projection is so
[79:39] that it's the same size across these different panels or else it wouldn't because the UVs aren't
[79:44] uniform tiling you can make that really really tiny here and then even the pattern amount we're
[79:51] gonna go a lot a lot a lot a lot and then the range i don't know .02 all right and then a sharpen
[79:57] filter filter sharpen all right now we got it nice and noisy so let's add some more stuff let's do
[80:09] it's kind of a lot let's do let's lower this height thinking whether or not i want this
[80:16] paint stuff to come through or not i'm guessing not although i could like lower the opacity a little
[80:21] bit you'd get a little bit of something maybe so we've got that and then we'll do a new fill layer
[80:28] called grunge all right and then for the bc that's fine opacity we're gonna do pretty low opacity
[80:37] and then roughness .6 cool and then we'll add a black mask and then we'll do our grunge painted
[80:44] let's go like that all right grunge sorry grunge paint scratched isn't it yeah this is an awesome
[80:52] one all right tiling let's do let's do a tri-planar again and then do tiling that's good and then
[81:00] let's see contrast let's bring that up and then we'll do a sharpen too really ties the room together
[81:06] doesn't it always always all right so there you go and then you can add or remove any of the wear
[81:12] here we can take a look at our other we added this in a couple places then we we added it right here
[81:17] we added it right here maybe i should scale it more because it's getting a little blurry in some
[81:21] areas but i liked it on the light that's fine so there you go jump into our renderer so we can see
[81:27] some nice rendering i do think uh we lost some of the height so maybe we've got to bump that up a
[81:33] little bit let's go to our flakes and then maybe we just jump this to 50 i mean the overall i feel
[81:39] like the overall height should even there we go because i should even get an edge for the for
[81:45] the wear you know see the little dings there i think it was a little better when it's more
[81:49] complicated than just those smooth lines so yeah there we go now i think this is looking better
[81:53] all right there we go so we've got a new material on here for our coating all right
[81:59] thing is coming along now so yeah we got this new coating material you can put that on whatever you
[82:04] want all right so that's pretty good so far with these man-made materials let's continue with
[82:11] leather so leather really common material and used on a lot of characters both fantasy and sci-fi


### Leather [82:12]
**Transcript (timestamped):**
[82:17] it's uh organic and in this helmet it's our first maybe only organic material because it is skin
[82:24] and so i'm gonna show you a way that you can make leather and again you can go so many different
[82:29] places from here and i could honestly talk for like an hour about leather so we're gonna do a
[82:34] simple leather setup just want to outline the pieces right it's gonna be similar to the paint
[82:40] in that i'm gonna do a bottom base layer of raw leather so we'll build a raw leather that's essentially
[82:46] just like a you know noisy rough surface then we'll do the leather skin topping and then we
[82:52] can punch holes and do wear and tear that way to reveal the raw leather you know in between
[82:56] on top of that we'll do some like some kind of wear and dirt you know roughness variations and
[83:01] everything leather skin pattern will be a part of that and then we'll do kind of stitching at the top
[83:05] okay so those are the basic components and i'll show you some more blend modes and layer effects
[83:10] and we'll use a we'll use one of the materials and substance too okay so let's build it and make some
[83:16] leather all right so this is where we were left before it's our paint we've got our coatings
[83:21] let's close everything up and let's open our leather all right so for our leather let's start
[83:28] we need to make our our leather raw so we're gonna start to make this a little bit more complicated
[83:32] as we do because it's just our block out so we actually want a folder in there called raw okay
[83:40] so let's in here let's make a folder called leather raw and inside there we're gonna do a base and
[83:50] now in this base we'll set it to something like that let's see something like this that's pretty
[83:58] good a little bit brighter maybe okay and then for the roughness it's gonna be kind of rough kind of a
[84:03] rough grain leather you know and now we'll do a here we'll take a look why don't we take a we'll
[84:08] do most of our demo on here why don't we and then we'll do a new fill layer on here and we'll call it
[84:15] grain and then is this good it's pretty good and then we'll take this light gray and then we'll
[84:22] set it for the blend mode and base color we'll set it to divide kind of makes it brighter more
[84:28] saturated and then for height we'll add some height to this grain too okay now we'll add a black mask
[84:34] and then we'll add a new fill we'll search for more assets i'll show you we'll do uh black and
[84:41] white what do they call it b and w spots okay b and w spots too that's what we use for our grain
[84:48] we'll strike that in there there we go let's see contrast bring that up a bit uh scale and uh we'll
[84:57] do a sharpen on that too sharpen okay so that's pretty uh it's pretty raw anything uh that height's
[85:04] kind of crazy though uh you know let's just eyeball this let me get something like that and then for
[85:10] our b and w spots okay there's our raw leather okay it's fine again you can do this stuff forever
[85:18] now outside of this raw leather we're gonna make a new fill layer and we're gonna add actually we're
[85:27] gonna add one of the materials they have here they call it leather skin don't we look at that perfect
[85:31] so we're gonna add our leather skin above raw all right we'll let this guy load there you go
[85:36] and uh i like using these materials whenever i can because you get a lot of uh detail for free
[85:41] we have three colors here they're not exactly what i want you could do a hue saturation but why don't
[85:44] we just choose three different colors so we'll go a little bit more yellow warm for me and then for
[85:51] the tip color we're gonna make that darker again just more yellow let's do like this and then for
[86:00] the patina color this might be a little bit too different from each other i don't want that much
[86:05] contrast you know three subtly different things i think would be good fine i suppose okay leather
[86:12] skin okay let's change the height range now it's a little bit too too uh much height detail i think
[86:18] so we're gonna go way lower it's at 0.05 now we're gonna go to 0.01 now and then we do need to set
[86:24] the the blend in the height mode to replace there we go now you can see look pretty nice right you
[86:30] get this detail let's go to it let's go to it still i feel like the is it the tipped color is that
[86:36] what's the dark spots yeah all right now let's add a black mask to this leather skin and we'll use
[86:45] we'll use metal edge wear one of our favorites generator metal edge wear okay uh invert true
[86:53] and you can see the we want more contrast in here now you saw like in this case doing all three
[87:00] i'll just show you how you can add a filter and i did that to the layer itself and i'll come in here
[87:05] and there's huge saturation levels or is it hls uh hsl yeah so i typed silly okay and then you see
[87:14] i have only color selected and so now i can darken this and i can change the temperature too although
[87:20] i like the color temperature so i'm gonna leave it but you see i i'm just affecting all the whole
[87:24] base color now with that all right back to my metal edge wear mask so grunge amount we're gonna do
[87:31] point four all right and then let me show you this too so this is a generator right but let's add a
[87:36] paint layer here and i'll just grab the leather brush right here you can see right here right
[87:42] so now i've got this leather brush and i'll just you know i'll just try to paint some uh some cracks
[87:48] here i don't think the size would be a good to have right here there you go maybe that's a little bit
[87:53] big there we go so now i'm just see now i'm just painting it maybe flow would be better to have
[87:58] let's let's try it with flow here we go yeah see that so now i'm wearing where i want it but i'm
[88:04] using a leather brush so now it looks all leathery right wow all right we'll leave it there we'll
[88:10] leave it there like that we did it on the bend point so that's that paint layer and then we'll
[88:16] do a threshold which will help that sharpness here we go and then the threshold it's good
[88:23] get it up there so that's it with that oh you can see here the raw is actually looks like it's poking
[88:29] out more doesn't it so i think for the leather skin to fix that because we have height on the raw too
[88:34] we've got height here so this will come up sometime so this is your height range i lowered the height
[88:39] range right still i can bring it back though because i'm cool like that you see it's popping up right
[88:43] but height position is what we can use to raise where the base level is so if i pop it out more
[88:51] i can i can have it start at a higher position than leather raw okay so height position something
[88:57] like that's it's kind of what's gonna right now dictate kind of how thick this leather skin is
[89:02] so gotta be careful with that but i think that looks pretty good so we'll leave this for now
[89:06] you'll see we can come back to these layers remember non-destructive let's continue on
[89:09] we'll get all the pieces set up so that's that uh let's do some staining let's create a new fill layer
[89:15] and we'll just call that stain and then the base color will be set to multiply
[89:24] and let's get a color here let's do something with a little bit of color all right and then roughness
[89:30] we'll do point three that's good okay black mask let's get some clouds clouds too and then balance
[89:36] we'll do three three and then uh contrast get some contrast going show you the mask all right and then
[89:43] scale we'll leave at one okay let's get some more stuff going let's do grunge grunge dirt um
[89:52] scratchy always okay and then we'll do that needs to be set to multiply on our mask it's
[90:01] going to remove some stuff here uh we're going to set the invert to true that way we just got
[90:05] these little flecks in there balance we'll do six four something like that a little bit more
[90:10] and then contrast we'll do a little bit too back on our leather skin we're going to add an anchor
[90:17] so now we've got an anchor for our leather skin remember we have our wear on there don't we because
[90:22] it's it's showing the raw beneath but we have our paint we have our metal edge wear procedural thing
[90:27] our little threshold so that's going to be our leather skin mask so now on the stain we can
[90:32] fill and we can add that anchor and then we can set it to multiply and so now the staining is
[90:39] only on the skin part that just one of the other many ways to use so now we've got color variation
[90:45] and everything going on things are looking a little bit more complicated that's good all those
[90:49] metal edge wear i feel like it's a lot but anyways okay let's continue on so let's do some more cracks
[90:57] all right let's create another fill layer um called cracks all right cracks and then we're
[91:05] set the uh base color blend mode to soft light this time it's too soft light where you at
[91:13] and then for the color do a little color again something like that will go all the way right
[91:19] and then height we're actually going to go negative and then roughness we're going to go pretty high
[91:24] okay we're going to do black mask and then we're going to fill this with leather damage that's called
[91:30] this one okay so you can see we're getting something okay and then let's see we need to tile this a
[91:37] little bit less we need this to be big all right and then balance it's going to be 0.34 we're going
[91:42] to drop it a little bit and then we're going to blur it a little bit add a blur and then the blur is
[91:46] going to be small though 0.3 all right and then now our handy dandy my favorite the bevel smooth
[91:54] bevel smooth all right now what i'm going to do here we're going to see we're going to get some
[92:01] nice like soft cracking so there's just more ways you can use all these filters and stuff so if I
[92:07] change my distance to something low and then smoothing offset my curve and then my shape and
[92:16] mass thresholds to 4 okay then we can add a sharpen make this more crispy and I'm going to crank this
[92:28] I'm going to do sharpen 4 you've ever seen that before look at that oh it looks like rivers dude
[92:33] look at some real cracks but it doesn't really look how we want yet huh we need to we need to invert
[92:42] so let's do it and then invert and then with our bevel smooth you know with the smoothing
[92:51] well it changes the shape everything's getting laggy now and then curve shape too that's like
[92:58] kind of the gap that fills it up yeah this makes it soft curves upping the curve shape
[93:05] gotta drop this down maybe maybe four is a little too hardcore anyways you see some cracks right
[93:09] looks more like leathery stuff you can see there all right here's something you can do again you
[93:15] can like mask it and out there's a million ways to do it okay so let's do a new fill layer we're
[93:23] going to do some edge stuff again so out of fill layer and we'll call it um and then height
[93:31] I'll just just need height don't need that let's do 0.65 add a black mask and then we'll fill it
[93:39] with that anchor right where's that well still let's just do this let's see what the fill layer
[93:46] and leather skin mask okay then we're gonna do a bevel told you I use bevel smooth a lot
[93:53] and it's new what was I doing before I don't know okay bevel smooth and then direction we want in
[94:00] here why don't you see what's going on here I'll show you we want the edges to curl up again remember
[94:03] this time we're using bevel smooth all right so that's bevel in distance something like 825
[94:10] this works for me you know experiment zero and then 0.03 and then 0.24 all right let's see
[94:17] 4.3.0.8 oh 0.08 smoothing feels like kind of a lot honestly uh let's see what it looks like
[94:27] all right now warp filter to make it irregular that's why we use warp all right um intensity
[94:35] yeah 0.1 is fine uh we're gonna blur it a little bit or a lot of it again before and after right
[94:40] just to get some irregularity then we're gonna blur this a little bit and this uh blur I don't
[94:46] know a little bit something like this and then we're gonna do the same trick we did before right
[94:51] so now we're gonna add a fill we're gonna add that anchor again and it's gonna be multiply
[94:57] let's try to make this feel good now let's see there we go so this the bevel smooth we gotta
[95:02] leave we gotta leave some of that you know but because of that I wonder yeah I think we're just
[95:07] gonna end up lowering this height that's probably just gonna be how it is we got some detail but
[95:14] not a ton but it's okay here we go cool all right that's set up and you can wear this stuff
[95:20] more and more right like if I came down here now we have this it's all predicated on this so um you
[95:26] know if I came in here and I just started wearing this away you get that crispy detail and if we
[95:31] didn't have the threshold you know it would you know I don't know it just feels a little bit more
[95:36] fake right so if you made it smaller you can kind of add some noise back in so it depends you can
[95:42] edit all this stuff depending on how like noisy or not you want it to be you know you're gonna just add
[95:47] some of that back in there so yeah you can just add add or remove as you see fit and instead of if
[95:53] you didn't want to be too harsh by the way right just to show you so if I took the threshold off
[95:59] and I did a levels instead it's not as brutal thresholds pretty much binary right you could
[96:05] you could come in here and still add but have a little bit more of a gradient you know if you
[96:11] wanted to come in here with and then wear and tear the stuff up you know with with some uh
[96:16] some level of gradients so up to you you have full creative control that's why a painter's awesome
[96:23] yep again million ways to do everything all right last part of this we're gonna do stitches
[96:30] so to do that we're gonna add a new paint layer uh we're actually just gonna use the one of the
[96:36] tools here too so I'll add a new paint layer at the top here we'll just call it stitches and then
[96:41] if we search down here for stitches it's this one top stitch so the way this will work this is a
[96:46] curved tool uh this is pretty cool come in here and what you'll do is you're gonna start in the
[96:54] corner and then we're gonna edit the brush settings and it saves it so like here let's just do one
[96:58] side right here actually maybe we need to so I'm just clicking a few times again non-destructive
[97:03] pretty cool I can move it okay now while I have it I'm gonna change some settings okay so if you
[97:09] come down here we'll look at some stitching parameters there's um spacing you can see they're
[97:15] touching don't like that so here's spacing uh if we set this to 0.25 see we're getting some spacing
[97:22] now 0.3 okay cool and then I can select the color probably don't want to be white you know probably
[97:31] like uh dark brown you know or just maybe just an off white if it's dirty or whatever and then also
[97:37] you would pick your size I think this is kind of okay for this but um let's see if we want to pick
[97:43] the size of our of our stitches stroke width I don't think that's it stitches stitches vertical
[97:51] stitches horizontal imperfections which is really cool okay I'm gonna say all right again I feel like
[97:57] it's too close together so I'm just gonna make the gap there we go all right and that's just cool
[98:01] curves you know non-destructive I can move them around really really great okay so now that we've
[98:07] got this set up I can come back in here and just select this ribbon thing again and it'll be it the
[98:17] same thing as the brush thing like double clicking these things just sets all the parameters all right
[98:22] there's those two we'll come over here we'll do some more get those in the right position a little
[98:28] more towards the edge I guess so at any time I can select this tool and I can hover over curve
[98:33] and I can come back and change it that's what's cool about this the downside is if I wanted to
[98:38] change the color of these at least I don't know a way I mean it'd be cool if they were like somehow
[98:42] smart about it I don't know but if I wanted to change any of those parameters I have to come in
[98:47] here select the path tool select the path and then make changes here also a new paths thing shows up
[98:54] so I can select every path that I did here you can see highlights in blue and then I'll have to
[98:58] so really make sure your first stroke has all the settings that you want really that's the key
[99:03] there but yeah there you go so now you've got your your stuff and then I assume we can hit replace
[99:12] on all of these right no we can't I wonder if uh base color should not be replaced all right yeah
[99:18] well that's stitches then really cool these things right here these these are kind of new additions
[99:22] to down here at the bottom definitely recommend playing with them but yeah there you go so let's
[99:26] see what we got here now with our leather that we made okay again could go crazy from here but we
[99:32] got the you know we got the makings of some leather looks like leather from over here so there you
[99:37] go we're gonna talk about model details all right so this is details this is texturing that's not


### Model Details [99:38]
**Transcript (timestamped):**
[99:44] just color roughness this is stuff in the normal and the height to give it form so these are some
[99:49] things that maybe could have been modeled in a lot of cases or maybe it's easier to do in texturing
[99:55] so there's several reasons why you do things like this one is sometimes you're just texturing and
[99:59] you're like hey that'd be nice to have some detail here you know you just didn't think of it or or
[100:04] you're texturing another asset or whatever and so it's good to be able to add little details here
[100:08] and there without having to go all the way back to the high poly and then some cases it's just easier
[100:13] more straightforward non-destructive as we've been seeing right to add model details in texturing so
[100:18] I'm going to show you some of that stuff I think it's awesome to do and I'm going to do it with
[100:22] kind of three categories of doing this the first one we're going to do is stamping down normals
[100:28] normal stamps super fun I'll show you how it works in substance painter and then at the end
[100:33] too I'll even show you how you can pick that stuff up in the generators we've been doing like curvature
[100:37] and getting dirt in the cracks and stuff so it'll be just as if you modeled it and baked it that way
[100:42] all right so here's how we left our helmets so what I'm going to do is I'm going to add a new
[100:49] layer now and the first thing to understand about what we're going to be doing is we're going to be
[100:55] using anchors so we've been using anchors in other ways right with masks and if you remember
[101:02] think about anchors is it goes bottom up the best place to put normal stamps is at the bottom
[101:09] because it has to live at the bottom because that way you can pick it up all the way through
[101:14] okay so let's start stamping down some normals okay so we'll just get any brush here and uh
[101:23] whatever we'll do we'll just do a basic hard brush and then we can just look for normal stamps
[101:29] and then we're going to put it in the normal channel here so if I just type in normal you
[101:35] see substance painter comes with some of these things and now you can go online and buy like
[101:40] you know packs of this stuff which is super cool you know you can see it comes with these
[101:44] things right here so we'll just use some of these that are you know just free examples
[101:49] but like you could buy hundreds of these things you know and make your own obviously so why don't
[101:53] we start with this little uh doohickey this seems cool so we'll drag it in the normal channel
[101:58] all right so we can see it and then we'll stamp it now you may not be able to see this okay obviously
[102:05] I can see it makes your life easy right but this sometimes in your you know check your painter but
[102:11] if you're you know maybe you have brush outline cursor by default I don't know right then you
[102:16] can't see it so you have to come up here in the upper left this little uh oh man that looked like
[102:20] that move flubber dude it looks like flubber anyway sorry if you do full preview it just straight
[102:25] up shows you which is fantastic you know because then you can see what you're doing and then if I
[102:30] hold control and then I right click move back and forth it's scale and then if I hold control and
[102:38] left click up and down it's rotate so we can really see uh what's going on here right so we're just
[102:44] gonna do this and then look at that wow it's like I'm a great modeler so why don't we just stamp down
[102:49] a few of these for funsies uh let's see what we got we could use one of these little vent things I
[102:56] suppose oh another good thing would be like screws right so it's what's like a good screw thing here
[103:03] is there any kind of like sci-fi looking screw I don't know what all this what's this gonna look like
[103:07] uh that's the fading up and down is fading I guess that looks kind of crazy looks kind of like a
[103:12] button now huh it's kind of cool look now our screws are crazier like a ball bearing I don't know is
[103:18] that good I don't know let's do some more let's do panels and stuff um oh there's another one that's
[103:23] useful is uh I'll show you this watch so I'm gonna put this over here got this little button don't
[103:28] we need those little uh those little thumb things don't like that it's cropping alpha get out of here
[103:35] there we go no alpha for you all right let's get this big enough here we go boom wait what
[103:43] this goes twice I'll get it one of these days you know here we go looks pretty good right
[103:49] and then you could also like you know come in here and then just uh erase gotta make sure your eraser
[103:55] also has a normal channel to erase these channel things are complicated let's keep doing some
[103:59] stuff let's do some more stuff a couple more vents this can be addicting so I won't go forever but
[104:05] you know it's cool kind of would be better if I could actually see though that works looks
[104:10] like there another thing now all right I guess that's good maybe we'll just do I'll end with
[104:15] one of these like panels you know this is a good sci-fi panel thing here it's a door right here
[104:21] service panel okay to get in there to change the batteries for the helmet okay cool all right that's
[104:27] that's uh that's good there you go there's some normal stamping detail all right so that's normal
[104:33] stamps so now um I'll show you one other little thing that thinks fun that I did while messing around
[104:39] and just to show you kind of some ideas on how you can use height and some other things to just
[104:44] add detail you know just as an example so it's a simple thing and then we'll get into specific
[104:49] things just for this asset all right so that's normal stamps those lived lives down there right so
[104:54] now I think it's time that we actually make our model detail uh folder so where could we put it
[105:00] we could probably put it at the top but um yeah I suppose we could put it at the top for now we
[105:06] can always move it later all right so I'm just gonna add like this edge extrude over everything so
[105:11] so I'm gonna get our model detail folder cook in here my model or I'm sorry I'm gonna set my folder
[105:16] to pass through on everything I'll make a base color in here and we'll call it edges extrude all
[105:25] right and then height we're gonna go down for this example doesn't really matter because you're just
[105:31] gonna just gonna end up being a normal map so we're gonna add a black mask all right and remember
[105:36] now we're gonna push down here so I'm gonna go in here I'm gonna add a generator I'm gonna add
[105:40] our curvature and then we're gonna mess with some of these settings so we're still gonna do edges
[105:45] for global blur we'll blur it a little bit balance we'll up it a little bit and then contrast
[105:52] we'll uh up that too and then we're gonna do an invert so let's see what we're cooking with here
[105:57] so for edges we're gonna do sharp uh something like this and then we're gonna zero all this other
[106:02] stuff out okay so with our curvature I played I just using sharp again in edges and I'm just trying
[106:09] to get the edges to peek for me out a little bit right so I can pick it up and then maybe even
[106:14] need some contrast to tighten it but there you go something like this okay so if we take a look
[106:19] at what it looks like right now the edges are popping out which is kind of a cool look already
[106:24] so with bevel it just softens it and then we can do the smoothing to round it you know um which
[106:29] makes it a little bit more purposeful and then we can um we can get in there and just remove the
[106:34] bits that we don't don't like you know so I don't know something like this see what smoothing
[106:39] does oh that's kind of cool makes a little bit simpler and so that's cranked way too high probably
[106:45] something like this might be okay I wonder actually let me see if we can get this looking good too
[106:50] that'd be pretty sweet let's see curve offset do we need that all right we don't need it everywhere
[106:55] why don't we here let's do this that's using some stuff to mess around again this is kind of cool
[107:00] don't you think like look at that it's kind of cool popping your edges but anyways trying to make
[107:04] some like extra panel detail especially for this black part because it looks it's looking a little
[107:08] simple I think it looks pretty good the black part that's what I'm looking at so what we could do now
[107:13] is we could say we can make a folder edges extrude layer it's good to not have the same
[107:20] name it you know and everything so we're gonna call this because then now we could do a black mask
[107:26] and we could just pick where we want this you know it wasn't looking so good here right I was like
[107:31] oh but the settings so you know to make the settings look good here doesn't look good here but
[107:35] you know the point is like we could just make this area look a little cooler get a little notch in
[107:39] there you know yeah maybe we add it there so it's extra extra thingy if we want to up here it looked
[107:46] pretty good you know it kind of goes around the screw very star warsy here let's get our mirror
[107:50] back on all right cue the oh so that worked out pretty good let's see if i can add it anywhere
[107:56] else i'm gonna do something a little bit more curated now okay so we're messing around with
[108:00] this black part on the side of the helmet and there's this kind of ear cup and again what I was
[108:06] feeling while texturing is this thing's kind of especially if i'm showing the side view this is
[108:10] a big element didn't have that much interest going on in the model I don't want to just do
[108:15] paint chips everywhere for the for the detail or to get some interest there so I was just playing
[108:20] around with some ideas to add more materials and stuff so we have this single model right here
[108:25] on the ear cup right and right now it's just both red and so what I want to do is get some of this
[108:30] black plastic in here get some metal in here and then I'll have paint so we'll have three different
[108:34] things going on and I'll I'll show you how we can use some of the selection tools and some of the
[108:38] other things we've been doing already to add a model detail here so it's a little bit more complex
[108:44] interesting okay so let's set that up all right let's do new fold uh new folder let's just start
[108:51] with a fill layer and we'll call it ear trim and then we'll have a bc here that's fine and then height
[109:01] we're gonna do uh point one fine and then we'll set to replace on everything here so we're gonna
[109:10] place the height and then uh roughness we'll make it point three and then metallic all right
[109:17] we're gonna have a shiny disc here we'll do some star wars stuff okay so let's add a black mask to
[109:22] here add a paint and then what we're gonna do is we're gonna select polygons this time we're gonna
[109:28] do a polygon select I might need to bring my wireframe back up shouldn't I all right so I'll get
[109:34] started here um now I already know what I wanted the kind of shape I want right so I'm gonna do
[109:40] this I'm gonna cut a notch out of it so I'm gonna do so you see these two rows here so I'm gonna
[109:46] I'm gonna count these I'm gonna say ooh something like that would that be good and then we'll do it
[109:51] on the other side something like this right that feel weird yeah like it's turned a little bit that's
[109:56] pretty cool let's jump into the flat view so we can finish a little easier okay so yeah it comes in
[110:02] here comes back up here I think that's right one two three four one two three four that's good okay
[110:08] and then we're just gonna start filling this up and I think we'll even do one more row inside
[110:14] so now it's just about getting all these selected cool let's see what this looks like how we're
[110:19] looking now yeah boy okay now a little bit crunchy that's okay uh but you know you can leave it like
[110:24] this but you know we'll just why don't we use our trusty uh why don't we use our
[110:28] but uh yeah so yeah you can leave it like this but we could use our trusty bevel smooth again
[110:36] so we're gonna go filter bevel smooth and then distance we're gonna do something pretty small
[110:43] smoothing something a little bigger see the rounded edges now pretty cool right looks better
[110:49] all right and then we'll do some more anchor points too stuff uh too so we're gonna you know
[110:54] we're gonna putting all this stuff together so there's the air trim shape let's add an anchor
[110:57] point to that we want to get this edge looking it's a little bit clean right a little bit weird
[111:02] look it's sitting on top let's get this more separated we'll call this ear shape outline
[111:09] and then for this one we're gonna make it darker and then for height we're gonna go down because
[111:15] we're gonna we're gonna make a little trench around this and the roughness we're gonna do one
[111:20] remember i told you never to do this so i guess i won't um but you can also put a o in there
[111:25] to be continued black fill layer and then you guessed it we're gonna get our anchor that's not
[111:31] the right one is it oh it is uh but we need just the outline so we're gonna do an outline filter
[111:37] mask outline it looks like the the guy again who did i say it looked like flubber okay mask
[111:45] outline all right threshold uh zero uh width 0.01 blur 0.01 just a little little guy look at that
[111:53] though now it looks like it's seated in there look at that are we cooking with gas or what no
[111:59] what do you think and uh now i think if we go down here to the paint um for the paint i think i want
[112:07] to get rid of this region so how can i do that can i do it with the uvs it's loading all the anchor
[112:13] stuff let's see did i get it right did i win did i not i guess i didn't split that yikes dude okay well
[112:20] what we could do i we're gonna make it black plastic won't aren't we let's do that let's go
[112:24] into black plastic we have it set to replace don't we so what if i just came in here and just did
[112:28] some dirty brushing what i just did a little bit of dirty brushing you know i mean that'll do it
[112:33] that'll do it uh little tip to since we're in here since we're in here i want to i want to
[112:37] show you something here the painting in the uv view it's good okay obviously us old-timers just
[112:43] used to do this uh it's the only thing we did but there's a setting i want to show you just any time
[112:47] you're painting in the uv view i want you to do this because you're actually still in the 3d if that
[112:52] makes sense and you can do these weird projections and stuff so if you look over um you see where it
[112:58] says alignment tangent wrap you can change that to uv and that's better so now it's just straight up
[113:05] this is just straight up painting in the uv view now just like just like back in the day
[113:09] you might not feel a difference and that's okay but it's gonna cut down to mistakes because you'll
[113:12] see the brush actually like changing size and doing weird angles and stuff when it's not like that
[113:16] because it's actually like doing a weird uh 3d thing but anyways i digress all right now is this
[113:21] the right plastic yeah that looks better right guys look at that oh freaking oh a little bit of
[113:28] sith action now am i right or what am i right or am i right very cool okay cool so that's that one
[113:33] all righty let's do a little bit more complex one now what i want to do is i'm gonna dress up this
[113:40] pipe you know we got a big black pipe in our face got these three segments they're the same
[113:45] a little bit boring so what i'm gonna do is we're gonna make a little cage it's kind of a saw one
[113:50] of my references all right so let's do it okay let's create a new folder in our model details
[113:56] i should put these in a folder by the way we'll call this ear detail good so now we got two
[114:02] folders going on so now we're gonna do a new folder for our our pipe cage and we're gonna call it
[114:09] pipe cage and then inside again we're just gonna do past this is good practice i don't know if you
[114:13] need it every time it's just that way if something's not working i'm like what's going on i just that's
[114:17] how i like to use folders is just to contain things all right you know a filled layer i'll call this
[114:22] metal cage and then we'll need this to be metal that's a fine metal color height we'll do a little
[114:31] baby height 0.01 roughness we're gonna make that pretty shiny and then it's gonna be metallic obviously
[114:39] the roughness probably we should set that now i could come in here and then in the height sorry
[114:45] the height to get out the bumps right looks pretty cool also move like that now i could come into the
[114:50] height channel though and like i could bring some of it back so i wonder like just a little bit just
[114:53] so it's just so it's not per you know it's a kind of nerd out on stuff like that it's like why not
[114:57] dude just lower the opacity a little bit okay so we have our metal thing here now we're gonna add a
[115:03] mask to this folder so we can see because that's metal everywhere we don't need that and then let's
[115:09] see if i broke this off no i didn't i think i'm realizing what happened here i thought i was smart
[115:14] and i i separated some of these uvs for the demo but i didn't do it on this version of the model so
[115:20] we're doing it the the old-fashioned way that's okay okay okay so now we got our metal pipe
[115:25] child looks good okay now let's add a black mask to this folder because we have a metal
[115:33] cage in here now we're gonna add some more stuff we're gonna add our little holes so we're gonna
[115:38] add a fill layer on top of this and we're gonna use the hexagons right here hexagon and then
[115:45] we're gonna change this up so tiling we're gonna put two two here just to get it up and then
[115:51] 12 here so quite a lot the balance get that up higher mm-hmm and then contrast uh hit invert
[116:01] and then let's see let's get smaller holes or whatever that looks pretty good all right now
[116:08] we're gonna do a threshold on here to make it super crispy let's see trying to not type so we can
[116:16] actually see where things are but i just i can't help but type it all the time do you see it anywhere
[116:20] oh it's down here so now it's super crispy huh is that too crispy though that's not so bad before
[116:24] you're honest with you i'm gonna leave it like this for now and then i'm gonna do uh anti aliasing
[116:31] fx a a looks pretty good actually like that all right i wonder if we make a little higher i think
[116:36] that's better okay and then so what's cool though is like from back here i'm like oh the hole should
[116:40] be bigger that's the hexagon balance so i can make it look however i want like a cage and then so in
[116:49] case you didn't see what i did there too you can just literally drag these around and also if i hold
[116:53] alt i can copy them so yeah this makes more sense it's easier that way i just do it on the fill
[116:58] layer and the pipe cage is just the mask like where it goes you know what i mean and so i put the holes
[117:03] here but they go everywhere but who cares you know i was like should you blend more those but no just
[117:08] if all if you don't know what to do just add up just add a folder dude yes indeedy okay so that looks
[117:15] kind of good it looks a little thin so i'm gonna make the holes a lot smaller and then i need to
[117:19] make this look like holes and then we'll make it dark yeah we go see isn't that better now clean
[117:25] looks like holes or something like what it actually holds probably not it'd be just leaking gas
[117:29] and just he's like it doesn't work but it's i think it looks better pops out see what i mean nice
[117:34] looks like a like a car part now or something right okay so there we go we got a little extra
[117:39] detail there i'm gonna draw inspiration from here having a little inset guy with some grip on there
[117:46] instead of just a cylinder i think that's gonna look better so let's build that out right now
[117:50] and go back to paint mode there's our pipe cage looking good all right now let's do our orange gasket
[117:58] i'm gonna make a new folder called you guessed it all right we'll set our folder to pass through
[118:06] let's create a let's just create a fill layer in here we'll call it base and then for base color
[118:11] make it darker we'll do a height we'll set to zero because we need to replace something and then
[118:18] roughness 0.5 nice middle ground and then metal be zero maybe like a dark base let's do a black
[118:24] mask and same thing as we did before let's say where this goes right so now we got like our global
[118:30] mask right now we can mess around in here and do whatever we want so i'll create a new fill layer
[118:34] and we'll call it orange and then we'll do vc something nice and orange all right uh and then
[118:43] let's do some height here and then for roughness we'll make it a little shinier let's put a default
[118:48] on there okay and then let's add a black mask to this orange layer to and separate it from the base
[118:54] a little bit and then we'll add a paint and i'm just gonna chip this away we'll line it up with this
[119:00] i'm gonna look nice see did i go all the way through there where is that now what guess what
[119:05] guess what i'm gonna do this looks so sharp oh if only there was a way what would i do what would
[119:09] come on dude bevel smooth dude have you been watching bevel smooth told you it's gonna be a
[119:13] lot of bevel smooth and i keep asking myself every time i use a million of these when i texture i'm
[119:16] like what was i doing like last year before this came out all right uh 0.01 smoothing a little bit
[119:27] a little bit smoothing a little bit smoothing and then negative there we go looks nicer right
[119:32] don't it all right now i do think i need to do our my replace shenanigans again on the base
[119:38] now we're gonna mess around a little bit more that's uh if you see here in the reference
[119:43] we have kind of a lip to it i think that's nice so we're not gonna just go live with 2d like
[119:47] you mess around some more i'm gonna add a blur to this and then it'll just be a little bit you know
[119:52] i'll do 23 dude mj the goat and then add a levels and then we're just gonna crank this a bit so
[120:00] i'm gonna come up around here all right let's add an anchor to this and let's let's add even more
[120:05] detail here let's do a new layer and call it edge height black mask phil let's get our let's get our
[120:13] mask we just messed around with orange and then let's mess around with this some more do a bevel
[120:18] smooth again on this and this time we're gonna go in yeah in distance 0.05 i guess smoothing we'll
[120:26] smooth it up and then for this one we're gonna do a height want to come up or come on come up
[120:32] it's good that looks pretty cool look at that it pops up i mean it looks a little too deep it's too
[120:36] hard on so maybe we're just gonna come up a little bit like that something like that now we add a
[120:41] little grip you know little dots or something okay so yeah see we're cooking though we're like
[120:46] modeling stuff aren't we but it's in the texture guys see that's the idea all right let's do another
[120:51] one side of the phil air call it dots let's add some dots and then let's do height let's go yeah
[120:59] we're making that dots go down roughness again we're gonna so we're making holes anytime i make
[121:05] holes i do roughness one and a o we could do zero we haven't added an a o channel yet we'll talk about
[121:10] that later we're gonna add a black mask to our dots and then we're gonna fill it so first i'll show
[121:20] you what we get some dots and we'll get a little tricky here so i'm gonna do circles and then for
[121:26] the circles uh we gotta do some tiling here and then contrast is gonna be one and then tile more
[121:34] tiny dots tiny tiny dots um balance we'll go whatever or something like that so we got dots
[121:40] over this is how we're gonna do it right we want to put it in here i'll show you this we'll do we're
[121:45] gonna add the phil and we're gonna actually get our orange mask again okay so we have the orange
[121:51] mask to start with okay so we're just mask on mask now the circles we could do um inverse subtract
[121:59] if we flip it so we have the phil here you know we could go to subtract and then it would be right
[122:04] here now we we're gonna which is good just on our orange part again right and then so we got our dots
[122:10] right so what i did was i i filled it again with the orange mask okay so we just got the same mask
[122:15] again to start with then i used bevel to bevel it in and you can see here it's out and then just
[122:21] curve off set in shape literally the opposite of what's in my notes so i don't know what the heck i was
[122:26] i was doing but anyways you can see here with these settings you know it lets me go in and out
[122:31] which is the whole point you know because i i just wanted to offset it uh to get you know around
[122:36] these little bevels so those so the dots are in the middle now if you can notice there's some gradient
[122:41] in there still that's not what i want i just wanted to procedurally make a perfect mask that just you
[122:47] know gets a little smaller so i added a threshold and the threshold comes in like that right and so
[122:52] i'm doing is i'm just raising the threshold right right at the end just so there you go and you could
[122:59] even if you wanted to by the way it depends on how much you need this but you could blur it and then
[123:04] do a an anti-aliasing or just do an anti-aliasing right now if you want but again i'm just using
[123:10] this to say where my circles go and the circles you know i was like inverse subtract less crazy
[123:16] you know but you know you just do multiply guys just do multiply and there you go and now i can
[123:23] like oh these holes are a little bit weird so just go to my bevel smooth and i just up the
[123:26] distance there we go and now my dots are perfectly in the middle so yeah why didn't i do that the
[123:30] first time i don't know stop asking me so many questions dude chill out um but yeah this height
[123:35] thing i think it'd be a little stronger too yeah dude so yeah i think that's a little cool little
[123:39] bit detail there i don't know if it's triggering that tryptophobia thing although again i think uh it
[123:44] is even cooler uh if i take it away from here though yeah it is cooler there it is it's just
[123:51] cooler if it's if it's got the lip coming up you know what i mean yeah that's cooler i don't care
[123:56] what you say mm what you say yeah here we go so now we got some model details don't we so if uh
[124:04] that's that's it for our model details for now and you can see uh where we are here and then
[124:10] where we were before turn off my folder let everything dump there we go so that's it before it
[124:15] looks it looks more plain doesn't it and now there we go with our model detail so yeah looking better
[124:20] now a little bit more interesting and this is just some of the ways that you can add details to your
[124:28] assets while in texturing you know so you can get a little bit more interest and there you go
[124:33] that's model details okay so next uh next i want to share some ways to make decals just pretty
[124:41] simple ways again you can go really deep and do custom stuff i'll show you using the tool and things
[124:45] like that so we'll put some stickers and decals on here next decals stickers numbers emblems you


### Decals [124:49]
**Transcript (timestamped):**
[124:51] know little things in your texture on your model if you're doing sci-fi stuff hard surface stuff
[124:56] super fun awesome way to bring interest detail scale storytelling we're gonna keep it going by
[125:02] staying organized we're gonna put this we're gonna make a new folder called decals and then we'll
[125:09] just start the colors on over here we go pass through and then in our folder we'll put a sticker
[125:18] but to do that why don't we first start with this fancy new tool at least it's new to me i don't
[125:23] know how long it's been in here to be honest with you uh but it's called the custom sticker tool
[125:26] look at that smile it's so cool and these are this is really cool so let's put a warning label
[125:31] right here so i'm just gonna drag this right on my model doink there you go pretty cool it's loading
[125:37] there you go so there's our sticker and you can click this and with you know w you can move around
[125:44] e rotate and then r scale you know like in normal 3d but we need to see what we're doing right so
[125:49] let's all we gotta do is put your image right here now i'm including some stickers and decals to use
[125:57] what you're doing this and so i'm gonna use some here from Jonas Ronegard probably butchering his
[126:03] name maybe Jonas you may have seen his work on our station but i contacted him he was kind enough to
[126:08] loan me two of these to give out to you guys to use i bought his stuff years ago he makes this
[126:14] stuff and you can buy all kinds of stuff but i love his presentation too and sticker book cool designs
[126:19] and all that so i'm just gonna put all these in here actually the ones i'm gonna use for the demo
[126:24] okay so i'm just gonna drag these in to the projects then i'm gonna identify these as textures
[126:30] so they'll be filtered as textures okay that's gonna be in the project so there you go there's
[126:34] my stuff okay so i can just drag my little like warning label right down there and boom there you
[126:40] go now right out the gate the settings aren't you know to my liking but that's okay so we're gonna
[126:46] we're gonna play with some of them so let's see let's go let's start with the outline i don't want
[126:50] the outline like this and then the height's a little crazy too but let's keep going with the
[126:55] material for the roughness that'll be higher and then wear and tear is pretty cool that there's
[127:01] stuff in here edge wear always like edge wear makes it a little bit more irregular yeah uh and then
[127:08] folds intensity i don't think we need that crazy right now and then sticker damage let's get some
[127:15] damage in there we'll go 0.75 and then for the intensity we'll go 0.35 there you guys kind of
[127:20] cool right like a little rip now i do think it looks pretty fat pretty chunky sticker there so i'm
[127:24] gonna come down here you can also change the residue color you know feel free to play around it's
[127:28] pretty cool um now the height range i think is just way too high for me so i'm gonna lower this
[127:33] now i'm gonna position it on the helmet like it was added here when they manufactured it or
[127:39] something like that i don't know mm-hmm mm-hmm it looks a little too new too by the way so let's
[127:45] first let's let's add a filter here and then do HSL that's huge saturation levels we just want
[127:52] it on the base color and this one is saturated darkened a little bit so it looks a little older
[127:57] maybe not too crazy but whatever you get the idea something like that okay that's our sticker let's
[128:01] let's drag it in our decals folder and we'll name this so we know what's going on let's add more
[128:06] more stickers okay let's drag um uh well just we're gonna do a section you know another manufacturer
[128:13] sticker let's do another sticker tool i guess we could we could have duplicated it was kind of fun
[128:20] to just drop drop these things on all right i think again we don't need an outline for this one
[128:24] it's kind of cool going behind the strap no whatever okay um do we need all this stuff i don't
[128:31] know let's do outline thickness zero material uh i guess we can leave it like that i don't know
[128:38] metallic sticker would be kind of cool uh but let's just change the stuff up folds intensity
[128:44] folds density and then corner zero zero zero sticker damage and then yeah we'll do a little bit
[128:51] okay something like that like a little hole there and again the height range uh again probably a
[128:57] little too brand new all right section 1a cool all right well there you go there's a couple stickers
[129:06] that we're cooking with now let's um do an easy one too check this out so we'll do like kind of a
[129:14] branding thing or something right okay so we had this little logo right here i can just drag this
[129:23] straight on to the model and it'll ask me what do you want to do and so i can say well let's make
[129:27] it a mask and then i'll do whatever i want right so again same just like the sticker i can position
[129:33] this so yeah really cool and then i can start giving it some stuff i can say let's give it some
[129:39] height i can say we're gonna replace everything that's for sure here we go and then there you go
[129:46] so looking already pretty cool and then i'll just drag that in there and then you can damage this up
[129:50] too if you want but yeah i thought it looked you know looks pretty cool um maybe we want a roughness
[129:56] too something like that all right there's a little branding okay so how about um a transparent sticker
[130:05] and that's kind of easy to do too we can do transparent sticker by using our sticker tool
[130:10] and then putting something on top so check it out we can do our sticker tool and we'll put
[130:16] like a little orange triangle thing here or something okay and then we'll put our little
[130:20] square here you know so i'll just show like um so like you know and this and these uh references
[130:26] you see how there's like transparent stickers like they will just do one of these like triangles
[130:30] see there's a sharper image of them not really here's one right so you have this
[130:34] square that's transparent and then there's like a picture in it same thing here so like instead of
[130:40] having like all these individual things you could do like you know like it was on a sheet which is
[130:44] a nice detail so that's what we're gonna do so we're gonna start by dragging that sticker tool
[130:47] back on here but we're not gonna put the image in this one all right instead we're just gonna disable
[130:53] all the materials except for height and roughness all the channels we're just gonna disable all the
[130:59] channels except for height and roughness and there you go again i think it's too thick so um oh
[131:06] oops that's position height range we're gonna do height range we're gonna do point three or something
[131:10] that there you go i think the folds are a little uh sharp just drop that down a little bit we'll do
[131:19] sticker roughness variation over here um and that's fine actually it's a good roughness
[131:26] i will give my old shinier if i think it's better and then yeah fold intensity um so there you go
[131:33] that way we can really see it's a sticker right all right so we want this looking shiny that's the
[131:39] difference here right and then we could also make it smoother like let's say we go to our height here
[131:46] and we do replace okay replace isn't working because that's the entire fill layer if we go to normal
[131:56] that'll give us what we're looking for still i'm gonna lower the opacity just a little bit a little
[132:02] bit there you go so kind of you know we're just faking like you can see through it right okay
[132:06] so that's our uh sticker there uh again pretty thick though pretty thick guy so i guess to make
[132:13] it look how we want here looking good so we got our transparent sticker all right so there we go
[132:20] now let's put our triangle on here right we're just that was the whole point of this we needed
[132:24] a backing so we can do a cool triangle here we go we're gonna do a mask again still eyeballing it
[132:29] you could make this asset you know like in photoshop or something and bring it in so you really want it
[132:35] okay then we're gonna make it kind of orange yellow
[132:41] there you go maybe we can make it um a little bit more techy we have any like tech triangles here
[132:47] it's kind of cool this one's kind of cool looks like an infinity going around and around let's do
[132:52] that one so there's that i guess if it's supposed to be probably supposed to be high vis a little
[132:56] bit right and again we're gonna just make sure uh well the height range should be like that and then
[133:03] that's kind of cool actually this looks even better because now the wrinkles kind of like
[133:06] pop up that's like and it's better actually i like that a lot cool there you go and it's nice
[133:11] and shiny right doesn't need to be glossier um that's pretty good point one five cool all right
[133:16] now we got a sticker let's make a a folder for this all right and then again we're gonna make this
[133:23] pass through then triangle backing it's fine so we can put these together in our sticker and we
[133:32] can put these in our decals folder and there we go we're cooking we're cooking all right let's do
[133:38] let's do a little warning label up here on our light again and then why don't we start by just
[133:43] duplicating this thing this backing is pretty cool so let's do that we're gonna get one of these guys
[133:51] we'll use it for something else a little bit different than dragging it huh you can actually
[133:55] in the 3d projection settings you can zero some of this stuff out and get it kind of nice and
[134:02] perfect right isn't this the direction it's going yes okay cool and then also the depth is um up here
[134:09] projection depth point three so this should be enough you can like have it come off all right
[134:14] that's that looks like some height stuff again because we're the way we're blending it that's
[134:20] okay it's going here so for the height position we need to get it above the dots and then for
[134:26] height you know want to wipe it pretty good there again we want to be thin looks like that's going
[134:32] in that's not what we want to come out a little bit good height range is this the wear and tear
[134:38] oh that's the uh it's fine okay and then folds intensity no we don't need that to be that crazy
[134:46] but i do like some edge wear i do like me some edge wear which also i kind of want to do that on
[134:50] this one too edge wears are my favorite parts of this yeah that's sick dude come on now
[134:55] just gotta be careful with my uh my blend technique here huh that what's going on all right
[135:01] i guess i can't do that much edge wear with this it's so pretty cool cool all right back up here
[135:06] back up here we have our label it's got some edge wear maybe not that much it's fine and then
[135:14] it's pretty like shiny is that maybe and now let's do another one so we got uh some kind of
[135:22] danger label and then we'll just say make it the base color actually is that what we want
[135:28] yeah it's fine just show that why not just show that you could make this another kind of decal like
[135:32] thing with roughness and all that but we're just going to do this and then i'm going to fill it in
[135:37] then this one doesn't have to be clear this one could have it's a little bit rougher let's say
[135:44] and then uh no outline and then it's like a charcoal or something like that it's good
[135:49] they can't do too much roughness variation that's because i squashed it so we gotta be careful with
[135:54] that but yeah there you go something and then maybe the decal i could drop the opacity a little bit
[136:00] once look very thin you know kind of good i guess i can't do edge wear looks like edge wear is going
[136:05] in and out of the uh height position or the height yeah no that was okay it's yeah it is that cool
[136:12] another sticker all right last thing last little part of the decal thing is uh projecting i want
[136:22] to show projecting that something comes up there's all kinds of reasons you want to project in the
[136:26] spirit of doing the decals and and putting things on the helmet i'm going to do a checker pattern
[136:32] and i'll show you some more projection tools this is good for like you know think like tattoo art on
[136:38] an arm or some kind of crazy mural maybe stuff on a piece of clothing um that kind of stuff so
[136:45] i'll show you some of the tools where you can bend and manipulate things so let's add our checker
[136:49] pattern kind of uh for us to be like a vinyl wrap so anyways i thought maybe i'll just mess around
[136:55] and show you a setup for this just since we're on this on the subject we're gonna talk about dirt
[137:00] and stuff a little later because that happens at the end but just want to show you can build
[137:04] something like this okay so i created a new fill layer and then what i did is you know i made a
[137:09] dark color i did a multiply in my base color and i added the roughness go up and then the first thing
[137:14] i did is i just added a a um anchor to the backing that's the square and then i brought that in so
[137:22] now i got that anchor and then i'll show you you know if i go add if i go fill layer and then i go
[137:29] anchor the triangle backing now it's not gonna work yet okay because the defaults here so i need
[137:36] to say extract alpha and i want i'm gonna take it from the height channel because remember it has
[137:41] height right so now we get our square so that's how i did that and then next is i use the mask
[137:46] outline to just get a blurry edge on the outline then i'm going to use levels uh so that it's like
[137:53] you know strong in the core and then it fades out and then clouds to just break it up so that's
[138:00] not you know so perfect you know what i mean could be however you want really then grunge dirt
[138:05] i'm just tiling grunge dirt you can tally it even more if you want again you know whatever
[138:10] and it's set to soft light this clouds is multiply again to just take chunks out of it and then this
[138:15] is soft light so the gradients start to get more noise you know this dirty pattern and then i just
[138:21] drag the same anchor at the top and then over here you can hit invert and i just set it to multiply
[138:28] so i'll show you what's happening here right so we got this blurry dirt clouds takes chunks of it away
[138:34] grunge gives it some noise some tooth and then i'm punching out the middle so that it looks like
[138:40] it's been gathering on the edges and then i just dropped it down a little bit so like some of it's
[138:44] creeping in we get a little bit of discoloration but it's got a sharper edge on the corners so yeah
[138:49] there you go and then i can just you know you can come in here and make more less dirt wherever you
[138:53] want clouds you can even hit random on the seed until you get what you like but just thought hey
[138:59] i'll just show you i'll do some sticker dirt right i don't know okay cool what were we talking about
[139:04] i got a little distracted oh yeah we're gonna do now let's continue on with our decal thing we're
[139:10] gonna do our vinyl wrap remember we're gonna do checkers we're gonna add this checker thing and
[139:15] we're gonna position it on our helmet and get it to wrap in okay so first things first what are we
[139:20] gonna do we're just gonna drag um we're just gonna keep our dragging on here we're gonna type in checker
[139:26] we're gonna drag this checker pattern right on here and we're gonna select uh we're gonna use it as
[139:33] a base color that's fine and then for tiling i'm gonna set it to eight so i need to scale this up
[139:41] something like this and then i want to position it i want to fill this like channel that's gray
[139:46] right now i want that to be checkers so let's have a little bit of a bend in it so right now i'm just
[139:50] gonna try to get it to cover the whole section something like this something kind of in the
[139:54] middle ground you know so i guess this kind of middle line i'll try to get you know keep it there
[139:59] all right so now we got the projection we scaled it up so it looks it looks okay right and then
[140:04] what i'm gonna do is i'm going to start editing the vertices of this you can see these you know
[140:10] on these edges we have these arrows pointing right if i come over here to my little warp thing here
[140:16] the transform warp i can edit vertices you can also i'm gonna go to edit vertices and now you can
[140:22] see on each of these points i get a white dot so now i'm actually just like in 3d i'm gonna hold
[140:29] shift i'm gonna select all these rotate them pretty cool pretty cool i'm just gonna start with a
[140:35] basic warp here it looks like it's stretching kind of a lot i think it's okay uh again you can
[140:42] always non-destructive right you can always get it uh like that let's see um let's do a black mask
[140:50] directly to this wonder i have to like mirror that i guess i could can i hear that was there a
[140:57] mirror filter mirror axis x well it's in the projection settings so we'll come over here
[141:04] symmetry x that's good oh flip oh no that's that looks like that's uv's so we have our red line
[141:10] can we get it right in the middle yes we can yes we can of course it'd be in the projection settings
[141:17] that makes sense all right good enough for now my perfectionism is getting in the way so i guess
[141:23] we'll stop uh so yeah we got it pretty good now um we'll just do a little art direction here we'll add
[141:28] um yeah let's let's make this like a yellow and black so we'll add a levels for our base color
[141:36] lift it up a little bit so that it's not like black black and then i'm gonna if i add a fill oh yeah
[141:42] what if i add a fill make it yellow now we got checkerboard too now we got a checkerboard too i
[141:48] wonder if i could um keep my black though is there a way to keep my black color no multiply is probably
[141:55] gonna be so i'll do the multiply first like it's brand new then i'll lift up the blacks
[142:03] there we go so now it's black and yellow so this is our decal pass check it out we've got decals
[142:12] look at that see it's got different roughnesses and stuff we've got little patterns we got stickers
[142:18] all right so now we've got our model with our decals applied we got some life into it
[142:25] interest little bits of color so that's really fun maybe one more let's do uh here i'll let
[142:30] let's do one more sticker here i forgot about one let's do one more let's drag our girl up here
[142:39] i put one of my stickers in here there we go cool we'll leave the outline and everything
[142:46] i think it looks cool looks like a sticker um but yeah we'll have the we'll have the height
[142:52] a normal and then we'll get our and then we'll do our folds intensity a little bit lower all right
[143:02] there's our helmet with some stickers now we got decals stickers uh little emblems clear ones
[143:09] colorful ones we got a checker pattern you know we use some warp and everything that's a bunch of
[143:13] stuff you can do with decals and stickers bring some color bring some life bring some storytelling
[143:18] to your project now that we have our texture in a pretty good spot you know we've we've gone through


### Overlays [143:20]
**Transcript (timestamped):**
[143:24] the block out now we've done a lot of material definition and some texturing and everything
[143:28] now we want to add a bunch of junk on top right so we're following in that kind of core principle
[143:35] we talked about at the beginning of layering things in the similar order that they would be in the
[143:40] real life and so if this were a real life prop we would have built it painted it done some effects
[143:45] and now we're doing the things on top the washes the the dirt we're doing color variation cavity
[143:52] things to pop things out so this is a super fun part of the process satisfying because we're going
[143:58] to get to take advantage of some of the work not only from the model but even mixing with some of
[144:02] the texturing we've done so far and we're gonna we're gonna do this all in a folder i call overlays
[144:08] that sits at the top of your layer stack and we're going to put a bunch of stuff in there
[144:12] that help bring our model and our texture more to life let's create our overlays folder at the
[144:20] very top of our stack all right there's our new folder and all right i guess yeah overlays all
[144:27] right now we'll jump back over to base color and i'll set it to pass through on all channels again
[144:34] for our folder all right now let's start with cavity that's a good place to start it's at a
[144:40] fill layer call it cavity and we're gonna put some junk in the cavities in the cracks you know all
[144:46] right let's go over to base color and we'll do something a little bit darker okay pretty dark
[144:52] maybe as dark as one might go here i'll set the opacity for the base color down though you know
[145:00] something around 40 or something and then the roughness we're gonna go pretty high so we'll
[145:06] go like 0.9 or something which is as high as you might go metallic we're gonna do zero this is
[145:14] really gonna help pop things on the metal and then we're gonna add a black mask to this all right
[145:20] we're gonna get some contrast in color material and roughness right now so let's add curvature
[145:26] generator here we go like we've done many times before and again we're gonna mess around these
[145:31] settings right global balance we can up it a little bit and then we're gonna set the mode right here
[145:39] to from edges to cavities all right you could also by the way why don't i show you this you
[145:45] could also so i'm just gonna use sharp okay so maybe sharp and then maybe fine a little bit and
[145:50] zero everything else out because we don't really tiny details right just want to show you the different
[145:54] options this is cavities it's trying to find the cavities will probably work well for what we're
[145:58] doing but you also have unprocessed you have dual too which is kind of everything you know you might
[146:03] want this for another kind of effect again just to you can imagine doing this just to pop your form
[146:08] you see how it gets readable you know what i mean so this is the kind of like little things that we're
[146:12] doing very subtly that isn't exactly from reality but just to help because it already defines the
[146:17] shapes right and then there's unprocessed this is straight up the cavity bake and again this is
[146:24] useful because you don't have any interpretation you can put a levels on this you have full control
[146:27] so this is like literally your cavity bake jump over here i'm gonna do cavities though for us
[146:31] or sorry that was your sorry this unprocessed this is your curvature bake so this is like your raw
[146:37] curvature which again you could set to overlay here like if you just had this as a base color you
[146:43] could set it to overlay which maybe i'll show you if you just want to see so watch if i make a
[146:48] base uh base color and i set it to curvature all right and then i just go unprocessed i could set it
[146:55] to overlay maybe soft light see the overlay there you go maybe soft light would even be better let's
[147:00] see so so soft light doesn't change the color as much you know so this is the kind of thing where
[147:05] just pops things out this is what we're gonna be doing anyways let's continue on with cavities
[147:09] curvature we got um we got cavities sharp fine how's that looking okay that's pretty good
[147:16] all right now we want to add a little bit more to this let's bring in some soft and then we'll add
[147:23] some some tooth we'll add some detail to this too a little bit like that medium i don't know
[147:28] and then large we got a little bit more gradient going on there okay then for use texture right
[147:35] here i'm gonna show you my highlight i can't do it okay true so we have use texture set to true
[147:41] texture opacity for some reason you have to set this higher it won't work and then for the texture
[147:47] let's look for grunge dirt scratched there we go and then the texture opacity as you can see it
[147:55] it's fading in and out so maybe just just just so it's not you know um perfect so that's like a
[148:01] perfect gradient we get a little bit of tooth in there and then maybe we should tile it a lot more
[148:05] too um let's go to the scale there's a scale for this let's go really high yeah so that's better
[148:12] so there we go so we got some cavity we can continue with this let's mix some more um and
[148:17] then we can dial this back in let's see what this is looking like so far in the model there you go
[148:21] so you're getting some i'll turn it on and off so it's popping the the borders in between of
[148:26] everything right the edges in between which is good separating the elements that's what we want
[148:30] we'll continue by adding or we'll go to the mask see what's going on i'm gonna add ambient occlusion
[148:36] if i could spell but you figured it out all right so the ambient occlusion
[148:40] let's do global balance and then let's see should we invert it yeah i think global invert
[148:50] or just invert all right so look now we're getting some like dust and gunk or whatever
[148:55] dark grimy stuff in here again this is just darkness this is not exactly dirt we'll get back to the
[149:01] the metal and then let's see so this is a lot of contrast we start lowering this okay it gets
[149:08] a little bit in there all right so now it's like inside like shadowy deep areas right so now if I
[149:14] set this over here over here on the layer if I set it to screen it'll add these two together
[149:20] so now we got our cavity cooking so this is kind of like those washes that we're talking about you
[149:24] know we're like you poured some dark thing on here and then you wiped it all away but again it pops
[149:31] because the metalness is dropping the roughness is getting more rough you know the base color is
[149:36] getting darker it just helps make shapes readable so there there's our first little overlay of the
[149:42] day okay let's keep going let's do let's pop out our edges we'll make a fill layer now called edges
[149:52] and then let's do base color of one because we'll probably soft light this and then we'll just use
[150:01] one of our smart masks let's do a black mask okay and then you can just search for smart masks paint
[150:07] subtle scratched we'll just drag that right in there and then you get all three of these things
[150:12] see what this cooks up okay there you go and then what we're gonna do is we're start editing these
[150:18] things so what you're gonna want to do is let's go into um let's go into the mask editor where
[150:25] we're starting and then in our mask editor let's play with our balance actually that's pretty good
[150:32] gold balance contrast maybe a little bit okay and then for our texture we're gonna do blending mode
[150:39] soft light here why don't we take a look at the actual mask there we go all right and then scale
[150:46] to contrast point eight five brightness let's go down there we go because what I want is edges
[150:53] and then I want some you know um I don't want to be perfect perfectly procedural you know before we
[150:58] start using our brush we're just gonna use some of this stuff to to mess it up texture and opacity
[151:04] where's opacity texture opacity we can drop that down to point five there we go okay for now what
[151:12] about texture two for the blending mode we'll do subtract all right scale let's do five and then for
[151:21] the opacity we'll do a point two for that okay so now we're gonna set this blend mode to overlay
[151:28] all right there we go so if I invert it see it's only on the edges now again this cool thing where
[151:35] you know it's popping out we get but we get some tooth to it you can play with the scale too if you
[151:39] want to to like makes things look a little smaller you can see what we get here just gets brighter so
[151:45] edges are getting brighter cavities are getting darker helps make this stuff all right so that's
[151:52] that you could also do like you can make a shiny for instance I'll just show you you could make this
[151:56] like shinier or rougher you know if you want to but I think this is good for now we're just trying
[152:02] to subtly pop it out all right on to our next fill layer let's do more cavities this time we're
[152:07] gonna do a cavity we're gonna call it cavity broad I'll put it below my edges um getting
[152:12] to shuffle these around based on how what kind of looks you want but we'll just continue cavity
[152:16] we'll do a different look here same base colors before we're gonna do a dark one one six one six
[152:22] one six all right and then for the base color opacity again we'll set it something low all
[152:28] right and then let's add a let's make it rough again same same deal all right and then let's add a
[152:34] black mask and then let's let's build something with the mask editor so that was the smart masks
[152:39] we were using on the edges and now we can build something similarly so we can come in here for
[152:43] generator and we can just type in mask editor where you'll mask editor it's a little wrench thing
[152:50] and you know this kind of gives you a starting place from zero and then we can build it up so
[152:55] you can use something and you can save these on your own if you want but those are the other ones
[152:59] ours it's just people made settings in here and then they saved it global balance we'll up this a
[153:05] little bit here let's do this we can take a look at what we're doing now remember we're gonna try to
[153:08] do like a broad cavity that's just a little bit bigger that's not as strong all right um so yeah
[153:15] we got this and then balance and then we'll do let's go to curvature and then for curvature mode
[153:22] let's go cavities already looking better big we want one huge let's see what we got there you go
[153:31] this is it all the way up and we could also um set this to multiply so we don't lose you know so
[153:37] it's not a complete like replace I think I'm going to lower the opacity on the roughness as well
[153:43] but there we go so we're still popping stuff out cool looking cool all right so we've got our first
[153:49] kind of pass at doing overlay stuff cavities getting darker more rough edges getting brighter so
[153:55] we're separating shapes that way you know based on our model detail and now let's start adding dirt
[154:00] so let's build our first dirt all right new layer let's do a base color here some kind of dark brown
[154:06] that's fine maybe it's a little too red but you get the idea that's pretty good okay roughness
[154:11] again I always hit the limit of 0.9 right unless you're doing like an actual cavity
[154:15] is dirt metal no italic zero which is going to help when it's on top of the metal it's going to
[154:19] look cool and then let's do a black mask and then we'll add some of the assets we have in here so
[154:25] let's add a fill and then I'm going to do grunge leak small I'll show you this one right here
[154:33] so here grunge leak small this will be in yours but maybe we can make it look like there's dirt
[154:38] you know I'll show you the mask there's dirt and maybe it's like running down so we could change
[154:43] this to from UVs which you see the orientation is different because the orientations of my UVs
[154:50] the orientation of my UVs isn't perfect you know they're not all going the same direction
[154:55] so if I change the projection from UV to triplanar that'll be projecting it from this cube around
[155:00] and now you can see we get more of a unified direction here and then for hardness um yeah
[155:07] we'll just up the hardest a little bit that's just the blend of the projection points okay so that's
[155:11] layer opacity we might you know we could dial that in later whatever um let's see for this for
[155:18] let's mess around with with our grunge leak small here layer blend all right well let's do this okay
[155:25] so we have oh that was roughness my bad let's go back to our base color okay so we have our
[155:29] triplanar projection going let's tile it a little bit probably that's better and then for balance
[155:37] there we go so now it's just more drips and less overall right and then contrast or your little
[155:44] contrast and that's fine all right cool cool cool all right this is what we got so far we have some
[155:48] like old drips you see by the way where you can see how we're layering up more and more detail in
[155:53] the roughness that's what you want you see how like the roughness is changing so much if we jump over
[155:58] to roughness uh I just realized this is my sticker like oh because the dirt's on there okay cool that's
[156:03] the sticker right there you can see we're getting more and more detail in the roughness and we'll
[156:06] finish this at the when we do our finishing touches we'll pop all this stuff even more okay so we got
[156:10] this leaking now we could go a little bit further too um you know will people notice this I don't
[156:15] know you tell me but check it out we're getting drips everywhere so let's make it so that the drips
[156:20] are strongest on the top as it would be right so to do that we'll add a light generator there's
[156:26] lights in here you could use all right so let's see light right here okay so if I just jump back
[156:31] over to the mask you can see right it looks like a light and you can position this all right so if
[156:36] we do uh something like this and then what's this do like something on the top you see and then for
[156:44] the glossiness that's kind of the sharpness we could drop it down so it's just like where is it
[156:49] dripping and fading out kind of and we could up this which is kind of the contrast and then the
[156:55] light attenuation is how far you know I can make it so it doesn't go all the way down but you probably
[156:59] do want it all the way on there because it is like you know we want it to be kind of on everything
[157:03] if you that makes sense all right so something like this I think is good so then what you do is set
[157:09] this to multiply which punches the black through right and the white just turns uh transparent so
[157:15] you can see we're darkening it now from the bottom and this so this keeps the drips on the top see what
[157:21] I mean again you could like you know play with this glossiness and stuff if you want but yeah a
[157:26] little bit of extra detail there and you can do that for a bunch of other reasons too if you want to
[157:30] okay so that is our little drippy light now we can do some more why don't we add another mask
[157:39] builder let's add another mask builders this generator mask builder all right let's go back to our mask
[157:46] so this uh comes with a bunch of other stuff this is the legacy mask builder um I assume that's still
[157:52] fine let's see so mask builder is the old one and this is the new one mask editor yeah we'll
[157:58] we'll see what the difference is we'll do mask builder why not you know I mean it comes with
[158:02] extra grunge already but it says legacy they might fade this out I mean they're pretty much the same
[158:07] but anyway so let's mess around with this one so we'll set this to screen again to add like to
[158:11] put to add the white together but let's mess around with this for a little bit so we'll do
[158:15] point three and we'll just start doing more dirt stuff contrasts let's make some sharper dirt then
[158:21] um grunge yes more grunge point three grunge is nice a o maybe not so much a o curvature one that's
[158:30] good um let's open that up look at some more curvature curvature range let's go the other way
[158:37] and then concave range smoothness let's pop this out let's uh let's get some grunge too let's do
[158:46] we have grunge right here is it not there's there's grunge oh there we go yes pool there we go
[158:53] all right noisiness zero and then the layer opacity we'll do screen on this merge all the
[158:59] stuff together and then the screen opacity was bringing in so this is dirt again this is gonna
[159:04] like be in the in the cavities dirt that kind of like got stuck it's kind of the idea okay we can
[159:10] tune this while we are looking at it it looks a little bit better without smoothness so you just
[159:15] get it pretty sharp it's kind of cool i like that i think i'm gonna keep that yeah so dirt's on the
[159:20] cracks like that i like that all right we're keeping that it is kind of everywhere around these
[159:24] these sort of look like um edges now so let me see if i can mix let's see do they call it micro
[159:30] details secondary grunge is doing it for me thank you secondary grunge cool okay at least it's
[159:36] uneven now more uneven cool all right there's some dirt again you know this looks like it's just been
[159:41] used it's got some raindrops on it stuff it's been outside or whatever that's the idea let's see
[159:46] what it's looking like in the render okay so it's starting to mix across yeah i think it's working
[159:51] okay all right so far so good let's add more dirt let's do let's do a new fill layer this one will call
[159:59] smeared dirt so you know the first one maybe it's dirt that has had no human interaction
[160:05] think of it that way we added dirt where it's a dirty helmet and then water it's either been tried
[160:10] to be cleaned or it's been in through the rain or whatever and then there's dirt that's been
[160:14] kicked around in the edges and now we're gonna do one where it's kind of got some wipes going on
[160:19] that maybe someone's been wiping it or it fell or whatever this looks pretty sick though every time
[160:23] i see this the white the white metal is pretty cool yeah okay so smeared dirt let's see let's do a
[160:29] base color of uh dark brown again that's fine roughness go 0.85 so not so rough but pretty rough
[160:39] and then zero let's add black mask here let's add a fill and then there's something called grunge
[160:45] wipe dusty that we'll use see here there you go you see that so we got speckles in here we got some
[160:51] direction there we go let's pay let's look at the mask as we build it we'll do tri-planar projection
[160:56] again so that it again it helps uniform you know it goes across everything regardless of UVs and
[161:02] this helps tell that story we're trying to tell tiling three because we want some crispiness there
[161:07] and then balance we can up it a little bit let's up the balance and the contrast okay now if we just
[161:15] looked at it like this you we get some of the specs right so now we have some soft gradients and now
[161:20] we're getting detailed specs that's cool let's let's take a step further i'm just gonna show you
[161:24] some more things you can do anywhere on here but we'll we'll do some stuff well let's let's start
[161:30] let's do a warp and we'll use a custom image input in the warp to try to get some directionality
[161:35] there okay so we'll just add to this all right so let's go let's do a warp filter filter warp okay
[161:43] and we'll set this up a little bit so for our intensity we'll go higher and then for the
[161:49] source mode we're gonna do a custom noise so right now there's nothing's happening you know
[161:54] because we have it we it's zero so instead of using just noise or pearly noise or whatever we can use
[161:59] an image let's look for this thing called leaky paint right here again i don't know it's a bug
[162:04] where it doesn't load there you go you see how we get some directionality here so let's try that
[162:08] to check that out now it's looking a lot more smeared right it looks like white or maybe it's
[162:12] maybe he's going fast this is a pod racing helmet now or something we can change well let's see
[162:18] for the blur should we change the blur we change the blur we'll get a little bit back because right
[162:22] now it looks really noisy right and if i blur all the way it looks kind of crazy so maybe we just get
[162:27] we keep a little bit and then for source tiling let's see if we lower that that's kind of cool
[162:34] looks like some weird drips for sure i do wish that i could um for the custom image i wish i could
[162:42] do a triplanar but i can't okay leak intensity leak scale one angle random no that's not good
[162:52] all right let's see what we got there all right so we got some more stuff and then let's sharpen it
[162:57] up back to our thing because when you do a warp too it's going to need some stuff but we're you
[163:01] know it's always good to sharpen your darts anyways all right let's do sharpen love that i see a
[163:08] little specks there and everything cool so we've got the gradient anything a really tiny and sharp
[163:12] on top of a gradient below that looks nice and then you can always add a paint layer too by the way
[163:16] and then paint out wherever you don't like it or wherever you want to you know obviously don't shy
[163:19] away from that keep it going we'll keep layering stuff up okay so we got our dirt cooking so far
[163:24] all right so that was our dirt so we've layered up a couple of different kinds of dirt right now
[163:28] you can see how if you're gonna do something passive something active something maybe soft
[163:34] has gradients you know so it's older bigger and then tiny more opaque sharper that kind of thing
[163:40] layering more contrast again helps with the appealing this the readability but we're kind of
[163:44] telling a story right we can make it up as long as as long as it's believable enough now another
[163:48] thing i want to show you that this is a tip i got from phil robb actually the you know co-founder
[163:53] art director at turtle rock so years ago he showed me this he did the textures the original textures
[163:59] on the left for dead characters and that's when i was still learning stuff and he showed me that's
[164:02] back when like before normal maps and everything and you know we painted all our textures in photoshop
[164:07] and he showed me this technique where uh you just have some kind of image that has junk and different
[164:14] colors in it and you very very softly put it over your stuff and it really makes it feel more like
[164:20] a photo makes it feel more um realistic because things aren't ever actually like flat colors
[164:27] it's really at least it's a cheat i've been doing that ever since so i'll show you how to do that
[164:30] in substance painter and that's a good little thing to bring some nuance to your to your textures
[164:36] so let's do that we're gonna add another fill there and we're gonna call it color variation
[164:41] then we're gonna search in here let's get out of our smart masks so i'm gonna put this image
[164:47] in there too you see it's called rusty overlay and i'm gonna drag that into the base color
[164:53] then i'm gonna set the blend mode for the base color to soft light this is like literally what
[164:58] we used to do in photoshop i'm just doing it in painter and then we're gonna lower the opacity
[165:04] a little bit so it's pretty low and then i'll put a levels on here too so you can just you can control
[165:09] whatever you want you know so i'll just move the midpoint down you know something like this
[165:14] so this is super super subtle okay let me see if you'll even be able to tell in a stream
[165:20] but so this is before and this is after again this is super subtle obviously when you get into
[165:25] texturing you'll see but just just the just the discoloration on the on here you know like right
[165:30] here getting a light spot all of a sudden i just think it helps things from being flat you know
[165:34] you get a little happy accidents you can obviously move and rotate this stuff around but just getting
[165:38] this like look at this little thing here it doesn't look more like some kind of photogrammetry
[165:42] i don't know maybe i'm crazy but maybe it's a little superstitious but i love adding this
[165:46] kind of thing and it helps you know bring some subtlety and nuance all right now let's end with
[165:54] one more cavity let's do uh let's do cavity sharp all right and then base color zero this is going
[166:03] to be the hardcore cavity roughness 0.9 all right and then if we add an ambient occlusion
[166:10] we can add that we'll add that later all right um black mask curvature y'all know what it is
[166:17] curvature cavities sharp only maybe fine 0.5 okay this is what we're cooking up right here see
[166:24] just to outline all this stuff all right so you might not be able to tell but like it's going here
[166:30] before after before after just to help outlines everything is it a little hardcore maybe you
[166:36] know you could loosen up the the base color a little bit if you want but very tiny thing it's
[166:42] just like outlining everything there we go i might even uh come in here and go metal zero
[166:46] see it just helps separate the elements that's our last overlay now we have our overlays on our
[166:54] helmet you can see a lot more stuff going on now and i think it's you know that's the thing with
[167:00] texturing the more layers of different things that are going on you know just looks a lot more
[167:04] complex and interesting so we still haven't done a lot of work with manual you know getting your
[167:09] brush and i said that at the beginning you got to be careful i just want to walk through setting
[167:12] this up you can and oftentimes when i'm texturing i set a lot of this stuff up and then i spend a
[167:17] lot of time hand painting in and out of masks and adding stuff um but for the sake of showing
[167:22] everything i think it's cool to show the interactions you could paint anything and
[167:26] everything obviously in any of these layers you can remove add paint your own drips exactly where
[167:31] you want it but i just want to show a bunch of the tools and functionality and everything
[167:35] so we'll keep going that is the overlays um now i'll just show you my helmet's gonna have some
[167:42] emissive glow you know what before i jump in and show emissive i feel like i should tag something
[167:48] on the end of the overlays and that's picking up some of the detail we've done so let me show you
[167:55] that let me let me jump in here we've set up our overlays now and it's looking pretty good but i
[168:00] just want to show how we can we can pick up some of the detail that we have in anchors okay so i'll
[168:06] add this to uh curvature let's let's do that to our normal anchors right so here's our cavity sharp
[168:13] so in curvature i'll do it here first or maybe i should do it uh in cavity first down here and
[168:19] then i'll do it again and sharp we'll see the differences so we have some like here you know
[168:23] it's just we should see it pop up here remember we added these details so for curvature let's come
[168:28] over here and what we need to do is say use micro details now i don't know why it's called that so
[168:34] micro height and normal are both on great i'll close this image tab so we have micro height micro
[168:40] detail on that's crazy it's under image inputs yeah so it's really just a mislabeling this is
[168:46] kind of on painter and then for micro normal we could choose oh we haven't add anchors yet you
[168:53] know like come down here normal stamps add anchor point up here cavity curvature micro details
[169:02] yes uh height normal you just need normal but maybe we can pick up the height too
[169:06] so now micro normal anchor point normal stamps reference channel normal yeah dude check that out
[169:17] dude all right we got it all right cavity sharp let's come here micro details true micro normal
[169:26] stamps there we go now we got that nice outline see that pretty good big difference i think okay cool
[169:33] so now we got our stuff we got our details in our overlays much better so let's come over here
[169:42] and we'll just put a new folder towards the top you could put it below overlays too if you want a
[169:48] little bit of dirt in your in your glow all right let's go let's add some lights why don't we all


### Emissive [169:49]
**Transcript (timestamped):**
[169:54] right now we got to do is turn on a missive well where is it well we have to add that it's not in
[169:58] here yet so we'll come into the texture set settings and we'll add our first new channel we
[170:03] haven't added a channel this whole time because our template had everything we needed so far but we
[170:08] can add any more of these and what we're gonna do is is just like a roughness and metallic it's an l
[170:13] eight all right an eight bit because it can be packed into a channel we don't need to get too deep
[170:18] into this but essentially this you know we just need black and white and then we can put it in an r
[170:24] gb or a channel you know a red green and blue alpha channel that's a full texture map we can
[170:30] just put this anywhere so we're gonna go emissive and we're gonna change it to l eight so now we
[170:35] have an emissive channel okay great so now back in our layer we have our light and then for emissive
[170:41] we're gonna up it and it should glow let's see after it starts thinking or is done thinking
[170:47] there you go why is it green i don't know honestly okay so i had a black mask
[170:53] out of paint layer and then we can just come in here and then i think i have lights in here
[170:56] don't i no i don't do i have lights in here no i don't um but you get the idea i mean this is an
[171:01] object so we'll just i'm probably just gonna make a material for these and put inserts in them but
[171:05] just for the demo i could see okay if i did do s r gb so i can get emissive color i can go into the
[171:13] shader settings and i can find emissive intensity and crank that up so now you get some color and
[171:21] some lens layers that's the post effects so the post effects is that glare you know from before
[171:27] so this is how you can preview it now it doesn't work in the ray trace renderer unfortunately
[171:32] but we'll get it in unreal again we're not gonna do color you know you can do screenshots in here
[171:36] if you wanted to do cinematic stuff but it doesn't really we don't really need that because we're
[171:41] gonna add the color later we're just gonna pack this into a channel so back to here we're gonna do
[171:46] l8 and that's gonna make it black and white so let's let it recalculate that and then we'll
[171:53] finish painting our emissive mask we'll do a light around the inside of the helmet and then
[172:00] maybe in this tube um let's go whatever lights i'll say emissive we'll just put it all in here
[172:08] you see now i'm adding paint layers and i'm naming them inner light and then let's see i'll
[172:14] just come in here and uh can i just choose this maybe i can do a strip should i do that wide or
[172:22] i'm wondering if i should do it too wide or just one wide honestly i don't know why it's yellow and
[172:27] it is it is tripping me out i i'm trying to not let it i'm what why is it yellow and i can't even
[172:34] change the base color it doesn't even matter it's like a sickly yellow too i'm like what and then
[172:38] don't work in no uh irate right if you say so okay so there's that and then i was gonna add a little
[172:46] bits um just the ear light again this is kind of just good practice because it helps me uh i need to
[172:52] edit this all right that is emissive again we're doing pretty basic we're doing a black and white
[173:01] mask for emissive we're doing a missive mask and then in unreal i can give it color and all that
[173:06] stuff so just good to visualize it in here why don't we finish texturing kind of techniques
[173:12] with the the cords the wires in the back of the helmet uh that way i can show using fonts text and
[173:18] stuff so kind of related to the decals from before that's something we haven't shown so i'll show you
[173:24] how you can use text in your texturing and we'll just figure we'll finish up the texturing part
[173:30] besides the glass which will do last okay so let's do that now and so now i'll show you how you can


### Fonts (Wires) [173:35]
**Transcript (timestamped):**
[173:36] import a custom font and you can use the text tools in substance painter to put text and writing in
[173:42] your textures and you got a tool you can play with so a couple different ways but we'll just use it to
[173:45] put a print along the cable to make it look like a like a tech cable so some simple stuff so far
[173:50] if you've been following along we've uh we're gonna do the same kind of basic stuff here and add a
[173:55] fill layer i'm just gonna go fast too uh we'll do orange delete the default layer and then we'll
[174:01] just pick a nice orangey color um something like this all right then roughness we'll do 0.5
[174:12] middle this zero and then we'll just do a couple that's good okay let's do another one black
[174:20] and then for this one kind of like this roughness i'm gonna get more rough i guess a little bit
[174:27] of variety there same uh metal zero and then a lot of black mask to this one so it'll just be on top
[174:34] so the big ones will be black how about that all right and then let's do some well why don't we do
[174:42] our our metal part so we'll do a folder called metal and then we could do uh chords okay and then in
[174:51] metal we'll do base metal i'll just say base metal here we'll do hide on for now roughness
[174:59] 0.25 metalness zero now we'll add the mask to the folder like we did before right that way we know
[175:08] okay so we got metalness right down now there's a little groove in here we can add some knurling
[175:11] i think that'd be cool so why don't we just add another one and we'll call it all right and then
[175:19] for this one we'll put a height on it and then let's do black mask and then we'll do tile generator
[175:28] done that before oops how to generate okay and then see pattern we're gonna change it to pyramid
[175:34] tiling we'll do a lot of them and then amount we should do a lot two these is probably fine
[175:42] amount it's maxed that out resolution i guess size one and one scale 1.16 okay now why isn't this
[175:56] hmm there's two different scales weird is there a way to offset it too i feel like we should offset it
[176:04] that's the side oh position offset oh 0.5 is that the magic number yeah sick okay and now
[176:15] scale will that go inside oh it's like over the border okay so let's get that under so it's not
[176:21] getting clipped and then is it scale can i make this bigger yeah dude over crank trying to limit me
[176:28] you can't limit me dude okay now how do we make this tiny now tiling see it changes everything
[176:35] oh i mean this will work but this is a dirty way we got here that's not a good scale
[176:39] there's two things called scale so many parameters you know what don't use tile generator i take it
[176:44] back okay when this knurling is done don't ever just don't ever do this let me add a filter yeah
[176:51] this is supposed to be about text guys how you getting me off
[176:53] how are you doing this to me some ghetto masking here we're just gonna say bye and then i'm gonna
[177:02] come back and go and go like this and then go multiply so was that worth it everything i don't
[177:09] think so guys all right just admit just memory wipe that from your brain okay uh while we're here
[177:14] though i do think um there was another little thing that that'd be cool so in the chords we could do
[177:20] fill layer call it lines i saw a chord like this in my reference wonder if i still have it up this
[177:25] is the kind of text we're gonna do by the way we're gonna do text like this along the chord right
[177:29] so we just need height let's do 0.7 or whatever add a black mask add a fill and then we're gonna do
[177:38] line stripes i think is what it's called there stripes and then tiling is this already did this
[177:47] before 29.03 see it right here and then stripes number 32 see it looks kind of cool right it kind
[177:57] of looks like there's like cables inside twisting i think that's what i saw like in one of the images
[178:02] so it makes it kind of that makes kind of cool there you go i think it looks kind of cool especially
[178:06] on the black ones anyways we'll leave it there why don't i just set the pastor and then let's do
[178:14] height replace let's do a replace on this so we don't get the chords coming through pastor on the
[178:19] folder replace on that there you go okay cool and then maybe for the lines i'll get rid of it on
[178:25] the orange ones keep it on the black ones maybe that's what we'll do now for the main event let's
[178:31] add some text all right so yeah we're gonna do printed text like this along so what we can do is
[178:39] do it in the chords and we'll say text and then pretty easy but what you can do is you can download
[178:46] fonts to get something specific if you want so i can just drag this in and then it knows it's a font
[178:52] and then i can say whether i want to do that project or in my whole library if i want to use that
[178:56] again and again so import this font so i have this dot digital font and there's a couple of different
[179:00] ways you could do it you could do a fill layer you could drag it in 3d and you can also drag it in 2d
[179:05] you can see i've laid out the chords horizontally which is going to help so if we do a mask here
[179:10] and then we do um yeah color white now we could type in our and then i'll drag this where our text
[179:17] is i don't need that layer if we drag in to the viewport so yeah there you go now we've got this
[179:23] we could say you know i don't know this chord is property of chord core label 1905
[179:36] thousand million okay and then i can scale it up and if we did f2 f1 we could see both of these
[179:45] the same time and then we can really see like what size it is okay that's obviously what the big
[179:50] i'm holding shift now get a position of it something like that i like it's kind of squashed
[179:56] that would be kind of cool uh squashing it we could also uh do some text effects so i think
[180:02] if i hold control and shift i can scale it down okay that's cool all right now let's do some more
[180:09] effects here to show you so one thing is i'll show you in the in the uv so over here for
[180:17] uv wrap you can wrap just horizontally so now it's just going horizontally which helps us for
[180:22] our row right and then also i could kind of spread out you see how the a little bit more spacing in
[180:28] the letters if we wanted to you know uh what we have that ability under advanced character spacing
[180:34] you can space it out a little bit looks a little bit more printed i think like that right and then
[180:38] so you could copy this a few times so if i hold alt and drag up i got another one maybe i don't
[180:45] want it to be perfectly in view and i'll drag it up again and then we'll just put on the other one
[180:52] and then maybe we want it to be a little bit darker so that we can still see it on both all
[180:57] right so now we put some text on there and you could similarly that's just some of the text
[181:02] effects so i could show you tiling horizontally character spacing in advance you can do more
[181:07] spacing and stuff but yeah you could use this to even make some of the decals that we're doing
[181:10] before if you want to put on a sticker or whatever you know comes up from time to time but i think
[181:14] it's really easy to use fonts bring in fonts drag them to change them so yeah super easy and intuitive
[181:20] now if you want to add text to your textures let's texture this glass visor last but not least so do


### Glass [181:22]
**Transcript (timestamped):**
[181:26] that we're going to come over i turn off the lights to a little distracting so do that we're
[181:29] going to jump over to our texture set for the visor now we want to do transparency to do that we
[181:35] have to make sure that we're using a shader that can do transparency you can see the two here
[181:40] metal rough with alpha test and metal rough with alpha blending blending lets you do gradients and
[181:47] that's what we want okay so we're on there now the other prerequisite is you have to have an
[181:51] opacity channel or else you can't see through this right so we're going to come in here we're
[181:54] going to add no opacity so there you go so first thing that we'll do is we'll add a base all right
[182:01] and then um we can give it some color pretty much what i had before i don't know if the color is
[182:07] going to matter that much when we render it to be honest but it's just set an anchor a base you know
[182:11] whoa i've got cap stock on uh roughness so small point one metallic we're going to go one looking
[182:19] like glass so far right and then opacity point two and there you go we've got some glass don't we
[182:27] got some glass and if i come in here to the ira the you know ray trace renderer look at that we can
[182:32] render glass and it's actually going through now this model i did try to double up the glass to
[182:38] make it look thick but i honestly i might just delete one layer because it doesn't really work
[182:43] and it's not gonna we're not going to do an actual simulation or anything so i'll probably just keep it
[182:46] one layer thin but for the sake of this we'll continue on but there you go we have some glass
[182:50] right maybe you should have done this earlier so that at least could look cool let's add some detail
[182:55] here you can see that's a perfect reflection we can see the environment but let's start to add
[182:59] some cool stuff some nuances here let's jump back over to the paint mode first thing fingerprints
[183:05] that's fun right so we're just going to create some normal kind of grungy stuff scratches and
[183:10] fingerprints and then we'll fade the edge put a fade around the edge too so it's kind of a
[183:16] transition we don't have this you know perfectly sharp thing helps draw the tension in the face
[183:20] and then you know some interesting things can happen might look like breath or like help with
[183:24] the light and the glow so again just to show a few different techniques so fingerprints and then
[183:30] bc let's do a little bit brighter and then roughness this is gonna be our main tool and then opacity
[183:37] one so the the fingerprints are gonna like have schmutz on there but then we can dial these things
[183:43] in after but let's add a black mask and then there's some fingerprint maps in here see which
[183:48] one's fingerprints dirty grunge fingerprints dirty cool it's already looking cool dude already cool
[183:55] man but yeah tiling let's go more than that let's just look at what we're doing here no fingerprints
[184:01] are still really big balance a little bit more cool nice okay now that's just fingerprints
[184:08] straight on there we let's get a little bit more interesting right actually i think i'm gonna i think
[184:14] i'm just gonna delete this actually you can see it's doubling up so i'm gonna fix this right now
[184:18] okay i just made it one plane now and re-import it okay so let's go back to our advisor
[184:26] all right so we have fingerprints let's add some more stuff let's let's add more layers so it's just
[184:32] not just straight up this uh we can add things that like uh like it's wiping right so we'll like
[184:37] someone's trying to wipe it off or whatever so let's go uh do wipe smudgy soft and we need to
[184:45] tile this to uh and then we're gonna make this multiply so you go so someone's been been wiping
[184:54] it away cool and then maybe we could do um clouds i mean i just honestly i could just do this whole
[185:03] thing we're gonna call the smudges and add more stuff let's do clouds okay and i know this is
[185:09] whatever but i'm gonna make it be like so so minimal again just so it's not perfect you know
[185:16] nice looks better okay uh now let's do the edges i was talking about let's do new layer edges and
[185:22] then we'll add rbc here dark darker and then roughness again point point eight eight eight
[185:31] opacity one let's do black mask let's see let's see what we're cooking here and we're gonna do
[185:38] the ambient occlusion is how we're gonna start this you can see already right so we're gonna
[185:43] try to turn this into a thing so we do global invert and then blur let's up this and the global
[185:50] balance there we go something like this and then can we blur the couple lot of it yeah see something
[185:56] like that and then we'll do some negative in here so it's not perfect again why don't we do
[186:01] fingerprints smeared is it and then we'll tile that to feel about the size of a hand
[186:09] something like that i guess and then uh there's just a little bit of tooth to it there we go
[186:15] all right looking cooler right let's finish up we'll do a sharpen on here
[186:22] you can see the difference much better right now let's do scratches and then i'll
[186:28] can mess around with the scratch generator um let's add a black mask to this well let's let's
[186:34] set our settings i guess so we'll just do we'll do height i'm not gonna export this probably
[186:40] though you could if you want to i just replace the normal map i suppose roughness we'll make it
[186:47] a little bit and then we'll add a black mask to this add our fill layer do the and we'll go back
[186:51] to the scratches generator okay we'll mess around with this all right so spline number
[186:57] 25 spline scale to spline width smaller and then random yeah yeah lots of random angles fine
[187:06] spline rotation random fine distortion um a little bit less distortion frequency
[187:15] well big wobbles this is essentially what we want and then luminance random one is good
[187:20] distortion random i know sure there you go so we got some scratches there and then the fade mode
[187:26] we'll do start and end i like that more so it just comes in and out you know all right see what we
[187:30] got as it moves over you can see again we don't need like you know you don't need the height i mean
[187:35] looks better in the render but there we go so we got some scratches all right let's see we see what
[187:39] we cooked up there's our helmet now with some smudges on there maybe the edges a little bit too
[187:46] much edges that's the blur photo cool i love just this is most of my time is just moving the lights
[187:54] around of stuff but yeah there we go so we have all of the pieces with textures i'm gonna finish up
[188:02] with just some finishing touches things i put at the very top of my stack and also double checking
[188:06] pbr and then we'll briefly go over export settings and then get this in unreal all right so back in


### Finish [188:13]
**Transcript (timestamped):**
[188:13] our substance project let's i'll demo this on the helmet it has the biggest texture stack all right so
[188:19] here's our helmet thing our helmet texture stack that we've built up over time so i'll add a new
[188:24] folder at the top i'll just call it finish and then we're gonna set this to pass through on all channels
[188:31] like we've been doing now the first thing is uh one of the things i want to do is i want to pick up
[188:37] all the edges and pop it out all right so we're gonna drag this mat FX HBO in here let's hop over
[188:46] to the ambient occlusion so we can see what's going on you can see it automatically goes to the
[188:50] height channel that's good so to see what it's doing you can see it's actually picking up that
[188:55] height detail that we added that model detail right which is good that's exactly what we want
[188:59] even the um like even the sticker super cool okay but we also want to add these um normal stamps
[189:05] those are the normal map channel right not the height so i come over to ambient occlusion
[189:09] i'm just going to duplicate this by holding alt and dragging up this one's going to be
[189:14] normal there you go now it's normal you can see it's replacing everything so if we set this to
[189:19] multiply then we get it you know we get the normal stamps combined together so i can zoom in here
[189:25] we get the a o in the cavity of our normal stamps too so again it just really helps
[189:29] seat these things in as if they were modeled okay nice little finishing touch to put at the very top
[189:36] okay easy to do all right now i'm going to do another thing which is uh adding a paint layer
[189:43] and then you can call this this is a global control so we're in a o right now if i go to base color
[189:48] and i set this to pass through on all channels now this folder is already passed through on all
[189:53] channels so that means it'll affect everything below so you know for instance a just nice little
[189:59] thing to do at the end is to add a sharpen and you can add it on all these channels that you want
[190:05] maybe even height if you want to right now but on this global layer i can do anything i can also
[190:11] you know add um a levels i can add an hsl right if i wanted to change the uh color temperatures of
[190:19] everything you know what i mean the lightness darkness whatever because this is my global
[190:24] control at the top again just easy practice i can probably illustrate that by showing you one last
[190:29] thing that you want to do towards the end of your texturing project a node for validating your pbr
[190:35] values uh i'm doing unreal so i'll show you the setting to change for unreal and why this is really
[190:41] useful so this is how it works it's called pbr validate so again a final step i would do i'll
[190:46] type in pbr validate there it is and you want to drag this to the top of your stack you want to be
[190:51] very very top and now over here for the albedo dark range you want to set this to 50 s rgb this is
[190:57] for unreal now there's an aces tone map and things are very complicated and everything changes all
[191:03] the time but still this is probably a good practice it's better to be a little bit lighter than too
[191:09] dark and once it once it you're too dark with your values it gets crushed and then it just looks
[191:15] not that good everything is not like that black right everything gets a little shinier and stuff
[191:19] like that so by changing it to the 50 s rgb dark threshold it's a little bit higher so you can see
[191:25] this is the red parts are too dark in our base color so we want to lift them up and we'll do the
[191:31] we'll use the global control to do that come over here and we'll add a levels and then we'll just bring
[191:37] this left we're on the base color affected channels and yes i just brought up a little bit
[191:42] and i'm okay with a little bit of red and like yellow and stuff this is fine so we just slightly
[191:47] tweaked it we can turn this validator off and there you go so yeah there is our nice helmets
[191:53] here we go look at that wow textured lots of different things going on right cool we want to
[192:02] export this out right so let's talk about export settings i'll briefly cover it and then i'll just
[192:09] apply an export preset that i have i'll go over what it does and then we'll export this and we'll
[192:14] see what happens what it looks like when you just directly import it into a level that i already made
[192:19] so let's talk about exporting this out so here we go we have our whole thing here so what we want to
[192:24] do is let's close this stuff up all right now under texture set settings no it's not um well i always
[192:33] do the hotkey control shift e which i guess is the same as export textures right here so if we come
[192:40] over here you'll see the export the export textures kind of settings they might look different by
[192:46] default if you come over here i don't know what output template it could be on like it could be on
[192:52] there's an unreal one right unreal packed unreal engine packed and so if we come into the output
[192:57] templates because yeah i've made some if we go to unreal engine packed you can see how these are set
[193:03] up so this is a good way to just learn you know the different ways people are doing this stuff
[193:08] but i'll go over my export preset which i'm using so i'm going to go over to um ccu e
[193:16] u dim and i'll just keep it there honestly and i'll show you what that is so ccu e udim so here we go
[193:22] so this and you can see this little button lets you choose these common variables for your naming
[193:29] conventions which are different based on what you want to do and your projects and all that stuff
[193:33] so just to read this this is the project which is helmet demo helmet underscore demo then the
[193:40] texture set which is helmet for me all right and this is cables right here these are texture set names
[193:46] and then for base color i'm saying bc and i'm saying that's the base color right here and then
[193:52] udim because my helmet has multiple udims now you could change it per but it's okay it's a personal
[193:59] project so i'll show you how you can do that if you want but that's it so this is it if i go to
[194:04] list of exports it'll tell you this is what it's gonna write out helmet demo cables helmet demo
[194:09] helmet and you see bc mask normal my pbr and it's got my udims on there as you can see it's pretty
[194:16] crazy like because i have four udims on my helmet look how many textures gonna export just my helmet
[194:20] it's pretty bananas if i come over here uh you can see how this is packed so this is normal the base
[194:24] color and then in the alpha i'm putting the opacity mask and then in pbr this is normal
[194:31] way to do it you do the mixed a o and r and then roughness in g metallic and b emissive i put in
[194:37] a you could swap these two if you really want to but that's okay and then it's normal direct x
[194:43] that's the regular thing to do and then the mask is just these extra things for like costumes and
[194:49] stuff so what i can do is i can just say for the helmet just don't export masks i can check it off
[194:57] and here the helmet we don't need the masks cables mask you can see i can even uncheck
[195:02] particular tiles and then i can even overwrite so the visor and the cables don't have a udim i can
[195:07] actually come in here and then just change it to the version without the udim if i wanted to be
[195:12] really clean about it so it's really cool you have full control over everything the moment has
[195:16] finally arrived so in secret in the background i have a scene made in unreal ready to import these
[195:24] textures so here it is right here we have the helmet i got the material set up theoretically
[195:30] we just got to export our textures and everything will magically pop up so hopefully that's what
[195:34] happens but yeah let's see if we can experience the fruits of our labor here let's jump back over to
[195:41] substance and we are going to double check our settings we have the cables helmet visor good good
[195:47] good and we have our list of exports okay so we're going to hit export and hopefully nothing
[195:54] crashes here we go we're in for it let's go the computer fan is spinning up let's go over to
[196:02] unreal and see what happens did everything name right is it gonna auto import i don't know i guess
[196:07] it's not gonna out of my board let's see here all right so now we got to go here oh i wonder if
[196:13] one sec false alarm okay let's come in here let's do this again okay so in the export settings
[196:20] we need to make sure i'm choosing the right directory so we're gonna go to um de unreal projects
[196:28] helmet helmet girl textures select i think that's right content helmet girl textures here that's
[196:36] right okay there we go running out of memory oh boy okay so we're gonna hit this outboard list
[196:42] exports okay we're gonna hit export there goes exporting all these textures so many textures
[196:48] look at all those textures and we'll see here it comes importing in oh it's coming it's coming
[196:53] it's coming my computer is flying right now there we go hey check it out a little bit blocky maybe
[197:02] we gotta stream in get a little closer here so yeah it's working it's working i will show you
[197:08] some stuff when it comes to these textures so for the normal map all right let's see if it's
[197:13] done it right did it do it right okay good srg srgb should be off these look a little too shiny so
[197:20] i have a feeling yeah srgb is on we don't want that holy shit hello and then save that what
[197:29] else do we got um we could probably just do it all at once my computer is crying over here by the
[197:34] way let's let's go over here and pause this we don't need this loading all the time okay let's see
[197:40] so we got pbr here normal map tables let's do it on the property matrix srgb should be off from all
[197:48] of these so is the roughness just way too rough for the glass i guess that's what's happening so let's
[197:53] holy shit do the frame rates unbelievable all right let's let's um open my glass and then for max
[198:00] roughness let's drop this because this is crazy feel the frame rate is insane guys all right there is
[198:08] helmet with some cool stuff in unreal real-time rendering looking cool super low frame rate but
[198:14] good for portfolios you know but yeah we got the detail on there lots of paint everything looking
[198:18] pretty cool we got the emissive there you go we got there in the end there is a texture demo


### Results [198:25]
**Transcript (timestamped):**
[198:41] and that is how i did this helmet texture that's it for this tutorial thank you for
[198:48] watching if you made it all the way to this point i just want to say again that the project files
[198:52] are available down below and the full unedited version is available at characterclass.com for
[198:57] students and also channel members and patrons so i truly hope that this video has helped in some way
[199:02] and if you end up texturing the helmet and you do something awesome yourself i would love to see it
[199:06] please tag me message me share with me i just would love to see anything that you guys make
[199:11] and i hope this helps you make awesome textures thank you for watching i'll see you in the next one
[199:16] peace out



---

## Captured Frames

- [15:58] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_000.jpg
- [18:20] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_001.jpg
- [21:30] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_002.jpg
- [24:30] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_003.jpg
- [32:45] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_004.jpg
- [46:10] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_005.jpg
- [51:05] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_006.jpg
- [54:30] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_007.jpg
- [74:45] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_008.jpg
- [87:40] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_009.jpg
- [101:55] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_010.jpg
- [115:50] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_011.jpg
- [125:30] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_012.jpg
- [139:50] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_013.jpg
- [145:40] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_014.jpg
- [156:45] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_015.jpg
- [170:05] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_016.jpg
- [179:00] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_017.jpg
- [182:00] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_018.jpg
- [190:45] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_019.jpg
- [193:45] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_020.jpg
- [197:30] tutorials/frames/how-to-texture-everything-in-substance-painter/frame_021.jpg

---

## Structured Notes

### Core Technique
A complete, non-destructive material-authoring pipeline for a hard-surface sci-fi helmet, covering nearly every common Substance Painter material family (metal, plastic, spray paint, leather, rubber, fabric, a fake-PBR "coating," glass) plus the connective techniques that make them read as one coherent object: anchor points driving multiple simultaneous effects from a single hand-paintable mask, model detail added entirely in texture (normal stamps + generator-driven extrusion picked up by later cavity/curvature passes), decals/stickers/projected text, a unifying top-of-stack "Overlays" composite pass (cavity, edge, dirt, color variation), emissive, and a PBR-validate-then-export-to-Unreal finish.

### Summary
J Hill's sequel to his skin-texturing tutorial ("everything else" this time), demoed live on a sci-fi helmet with downloadable project files. He opens with a texturing philosophy (balance "what it's made of / where it's been" storytelling against a clean, readable "first read / second read / third read" silhouette, citing Hollywood prop-painting references) and a scene-setup pass (swap the default HDRI for a neutral studio HDRI — "Tomoko" — to avoid color cast, set camera focal length to 50mm). The core method is: **block out every material as flat fill layers + masks first** (metal, paint, plastic, leather, fabric — each its own folder, ordered bottom-up the way the materials would physically stack in reality), *then* go back and add nuance/wear/detail to each one in turn. Anchor points are the throughline of the whole video — a single paintable "control" mask lives at the bottom of a folder and drives color, primer, edge, and detail layers above it simultaneously, so one brush stroke updates several linked effects at once. The `Bevel Smooth` filter (a then-recently-added filter — see App & Version) is used constantly to turn flat procedural masks into soft, physically-plausible offset/curled edges (paint chips, leather cracks, gasket lips, pipe-cage holes). The video ends with a PBR-sanity-check node (`PBR Validate`), a walkthrough of a UDIM-aware export preset, and a live import into an already-lit Unreal Engine scene.

### Key Steps

**0. Scene setup (before texturing anything)**
1. Swap the default "sunny field" HDRI for a neutral/desaturated one (creator uses a custom "Tomoko" studio HDRI) via Display Settings — raise Environment opacity, lower blur — to avoid an unwanted color cast on the base materials.
2. Set the viewport camera's focal length to `50` (roughly matches human-eye perspective; `85` for portraits).
3. Note texture-set layout: this project has 3 texture sets (Helmet, Cables, Visor); the Helmet texture set spans 4 UDIM tiles. `F1` toggles between the Layer Stack view and a combined Bake+Layout view.

**1. Block-out pass (§ Blockout, 7:03–16:24)**
4. Delete the default layer. Add a `base` fill layer at the very bottom of the stack with **every channel explicitly set to its default** (Height 0, Roughness default, Metallic 0, Normal 0) — this is deliberate: because Painter blends bottom-up, an unset "anchor" base layer prevents later layers from silently inheriting whatever the previous project state happened to be.
5. For each material (Metal, Paint, Plastic, Leather, Fabric): create a folder (materials capitalized for organization), add a `base` fill layer inside with a rough approximation of BaseColor/Roughness/Metallic, add a black mask to the **folder**, then build up coverage with `paint` fill layers (never paint directly into the mask — always add a Paint fill layer on top of the mask so strokes stay editable/re-orderable) using Polygon Fill / Mesh Fill / UV Chunk Fill selection modes depending on how the mesh is UV-split.
6. Order folders bottom-to-top matching real-world layering (metal → paint → plastic/leather/fabric details → dirt on top), matching the layer stack's visual order to "how it would be in the real world."
7. For Fabric, drag in a ready-made Painter material (`Fabric Cotton Jersey`) instead of hand-building — adjust its exposed parameters (Tiling ×8, Fabric Color, Fabric Color Variation, Weft Distortion ~0.1, Height Range lowered) rather than building fabric noise from scratch. (frame_000, captured right after block-out completion — note the block-out already reads fairly convincingly because these are real fill/material layers with inherent surface variation, not flat placeholder colors.)

**2. Base Metal (§ Metal, 16:24–31:10)**
8. `Wear` fill layer: darker BaseColor, Roughness ~0.8, black mask, then a `Grunge Paint Scratched` fill inside the mask (tiling ×10, tune Balance/Contrast), topped with a `Sharpen` filter (~0.15) for crispness (frame_001).
9. `Noise` fill layer (BaseColor ~0.85, Roughness ~0.85): mask built from two `3D Perlin Noise Fractal` generators — first one set to **Match per UV Tile** projection (needed because the mesh uses UDIMs) at Position ~0.36/Contrast ~0.45/Scale 10; second one added on top set to **Multiply** blend to subtract detail, high Contrast, even Scale — layering two noise passes this way (add, then multiply-subtract) reads as far less "proceduralized" than one pass alone.
10. `Edge Wear` fill layer (BaseColor white, Roughness 0.5) with the **`Metal Edge Wear` generator**: raise Wear Level, lower Wear Contrast, lower Grunge Amount (so it doesn't fight hand-added grunge later), Edge Smoothness ~1.7 to soften, plus a `Sharpen` filter (~0.25) (frame_002 — full generator parameter panel: Wear Level, Wear Contrast, Ice Diplomer, Displacement Blending Contrast, Vaguery Amount, Vaguery Scale, Edge Contrast Change, Edge Smoothness, Ambient Occlusion Weighting, Curvature Weight, Micro Details).
11. `Scratches` fill layer with the **`Scratches` generator**: Spline Number ~200, Spline Scale ~0.75, thinner Spline Width, Width/Scale Random on, Spline Distortion + Distortion Frequency on, Fade Length applied to both ends for taper-in/out.
12. `Screws` fill layer (Roughness 0.5, Metallic 1): BaseColor driven by a **`Curvature` generator instead of a flat color** — Alt-click "Color" to isolate the color channel, Balance ~0.45, Mode = Edges → Sharp (weight ~0.66), Big ~0.25 — darkens recesses/holes procedurally for a worn/anodized screw look, masked to just the screw geometry (frame_003 — Curvature generator panel: Global Invert False, Global Blur 0, Global Balance 0.44, Global Contrast 0, Curvature section, Use Texture/Use Micro Details toggles, Image Inputs = Curvature/World Space Normals/Position Gradient).
13. `Surface Imperfections` fill layer (Height 0.03): mask built from a `Clouds 1` fill (Scale 3) with Height-channel blend mode set to **Linear Dodge (Add)** at ~40% opacity — demonstrates the recurring "per-channel blend mode/opacity" gotcha (see Layers/Tools/Settings). A second `Grunge Plaster Paint` fill (Balance 0.9) adds "missing chunks."
14. Finish metal with a `Shiny Metal` fill layer: BaseColor value ~0.7–0.75, Height channel blend mode switched to **Replace** (not Add) so it fully overrides layers below and creates clean "polished pocket" reveals; masked with the `Metal Edge Wear` generator again, smaller/smoother settings, more grunge.
15. Key teaching moment on **layer blending across channels**: each PBR channel (BaseColor/Height/Roughness/Metallic) is its *own independent layer stack* with its own blend mode and opacity — changing one channel's blend mode to Pass Through does NOT change the others. **Right-click → "Apply to all channels"** is the fast way to sync a blend-mode change (e.g. setting Height to Replace) across every channel at once.

**3. Plastic (§ Plastic, 31:10–40:38)**
16. Reworked the placeholder plastic fill into a real "Rubber Raw" **Substance base material** (drag from the asset shelf) — switched its UV projection to **Triplanar** so the tiling reads consistently across UV seams, Tiling ×10, then tamed its built-in Roughness Variation by adding a `Levels` filter isolated to the Roughness channel only (compresses the material's baked-in variation range so the artist's own added variation isn't fighting it) (frame_004 — Fill layer Properties panel: UV Transformation Scale/Rotation, Symmetry, Material tab showing color/height/rough/metal channel thumbnails, "Rubber Raw" substance material loaded).
17. Additional plastic sub-materials layered on top by UV Chunk/Polygon-selecting different plastic parts: `Black Shiny` (dark BaseColor ~0.15, Roughness ~0.15), `Gray Plastic`, `Red` (duplicated from Black Shiny to inherit its Replace height setting). Each demonstrates the same channel-blend-mode Replace/Apply-to-all-channels pattern from Metal.
18. Plastic wear: `Scratches` fill (BaseColor blend Overlay, white, Roughness +0.7) masked with the **`Paint Subtle Scratch` Smart Mask** dragged straight onto the mask slot — then Global Invert flipped True (the smart mask ships inverted from what's wanted here) and a Sharpen filter added; demonstrates dropping a pre-built Smart Mask and then hand-tuning its exposed parameters rather than rebuilding from scratch.

**4. Paint — anchor points introduced (§ Paint, 40:38–73:47)**
19. Sub-folder "Paint Colors" inside Paint, containing flat color fill layers (Red/Orange/Blue) each individually masked with Paint fill layers / polygon selection to lay out where each spray-paint color goes.
20. Hand-painted spray-paint look: mirror mode on, an airbrush-style stroke pass, then a `Gaussian Spots 2` fill layer (tiny scale, Balance ~9.5) set to **Soft Light** blend to turn gradient edges into speckled spray texture; a `Levels` filter clamps the whites for more "opaque" coverage.
21. **Anchor point workflow (core technique of the whole video):** Create a plain paint layer at the very **bottom** of the Paint folder named "Paint Mask Control" with a black mask (anchors can only reference layers below them, hence bottom placement) → right-click it → **Add Anchor Point**. Any layer *above* that references this anchor (Fill layer → mask source = the anchor) inherits the exact same live mask — painting on the control layer instantly updates every layer that references the anchor (frame_005 — Paint fill layer Properties, Brush panel, layer stack showing "Paint Mask Control" folder structure).
22. Built up the anchor's driven mask with a stack of generators *below the anchor point*: `Curvature` (Multiply, Global Invert True, Mode=Edges, Sharp weight ~1, Soft ~0.3) → `Curvature` again using a custom **Texture** image input (`Grunge Concrete Burnt`, Contrast raised) for extra breakup → `Metal Edge Wear` (Multiply, Global Invert True, Wear Contrast/Grunge Amount/Grunge Scale/AO Masking tuned) for extra crispness.
23. Split the single anchor-driven effect into **two offset layers for a two-tone paint-chip look**: duplicated the folder into "Primer" (uses the anchor mask directly) and "Paint Colors" (uses the anchor mask but pushed back with `Bevel Smooth` — Distance ~0.0095, Smoothing 0, Curve Offset ~ -0.15, Curve Shape -1, Mask Threshold 2.17 — plus a `Warp` filter with low Intensity/high Blur for an irregular, non-extruded edge, then `Sharpen`) so the primer "pokes through" at the paint's worn edges (frame_006 — Bevel Smooth filter panel: Direction, Distance, Smoothing, Curve Shape, Mask Threshold, Distance Map Multiplier, Reverse Wrap toggle; layer stack shows color-coded "Paint Colors"/regions for visual debugging).
24. Added a second, lighter "Light Primer" layer with its own Bevel Smooth settings (Distance 0.01, Smoothing 1.75, Curve Offset -0.78, Curve Shape -1, Mask Threshold 0.43) plus its own Warp (Intensity 0.25, Source Blur 1, Source Balance 0.75, Tiling 5) and a **`Quantize`** node (set to 3 — like Photoshop's Posterize, flattens a gradient into N discrete bands) for a stepped, worn-paint look.
25. **Direct hand-painting on the anchor's control layer**, using the Smooth Noisy brush (varies pressure + has its own pattern), to spot-fix where the procedural wear should/shouldn't happen — art-directing the automatically-generated chip pattern region by region while every downstream layer (primer reveal, warp, bevel) updates live from the same brushstroke (frame_007 — viewport mid-paint, color-coded paint regions visible for debugging, brush panel active).
26. Added `Dirt` (yellow-brown, Roughness 0.7) using a **`Tile Generator`** in Custom-Image mode loading a custom "Dirt Stain Large" image, with Random Rotation/Symmetry/Scale randomization exposed per-tile. Added `Stains` (multiply blend) using the **`Dust Stain` Smart Mask**. Added `Shiny Stains` (Roughness 0.1, targeted shine) using **`Grunge Map 007`** (Triplanar, Balance 0.41). Added `Roughness Variation` (Roughness maxed, masked with 3D Perlin Noise, Contrast 0.16, Scale 30, Distortion Intensity 0.35, opacity lowered in the mask). Added `Fingerprints` using **`Grunge Fingerprints Smeared`** (Triplanar, Overlay blend in the mask, tiling 4).
27. Added `Edges` (Multiply BaseColor) darkening near metal boundaries via `Curvature` (Balance 0.3, Mode=Edges→Sharp/Soft/Medium tuned) for a "burnt paper edge" pop-out look, plus `Dust` via `Grunge Dusty Scratch`.
28. **Edge-peel detail pass**: new `Paint Edges` fill layer at the very top of Paint Colors, Height ~0.02, mask built from the **anchor again** run through a `Mask Outline` filter (Outside Threshold 0, Width 0.03, Blur 0, Curve Shape ≈ -6.5) to get a thin ring right at the paint edge; a second copy of the anchor set to **Multiply** with the outline punches out the middle so only the ring remains; a `Warp` filter (Source Blur, Tiling, Intensity, small Blur ~0.1) roughens the ring so it doesn't look like a uniform extruded rim, reading as curling/peeling paint.

**5. Metal Coating — deliberately breaking PBR (§ Metal Coating, 73:47–82:11)**
29. For a fake-metallic hard-coat/paint look (e.g. sci-fi flashlight housing): new `Base Coating` fill layer with **Metallic set to a middle value (~0.6) instead of a "correct" 0 or 1** — an intentional, explained PBR break ("this isn't true PBR") to fake the look of metal-flake paint / partial-metal coatings without it reading as either bare plastic or bare metal (frame_008 — Fill layer material panel showing Metallic slider near mid-range on the "Base Coating" layer inside a "Coating" folder).
30. Mask built from `Curvature` (Global Invert True, Mode=Edges→Sharp/Soft/Medium) layered with `Grunge Dirt Scratchy` (Overlay) and `Grunge Scratches Rough` (Multiply, smaller tiling), then crunched with a **`Threshold`** node to make the wear read as more binary/chipped rather than a soft gradient.
31. Added `Flakes` (Height 0.02) via **`Gradient Flakes`** fill (Triplanar, very small scale, high Pattern Amount) plus `Sharpen`, and a low-opacity `Grunge` fill (`Grunge Paint Scratched`, Triplanar) — raised the Flakes layer's overall Height contribution (~50%) afterward because the coating was losing its edge definition once combined with other layers.

**6. Leather (§ Leather, 82:11–99:38)**
32. `Leather Raw` sub-folder: `base` fill (Roughness fairly rough) + `Grain` fill (BaseColor blend **Divide** for brighter/more-saturated grain, small Height), masked with **`B&W Spots 2`** (Contrast up) + `Sharpen`.
33. On top of the raw base, dragged in the ready-made **`Leather Skin` Substance material**, recolored its 3 exposed slots (base/tip/patina colors — kept them subtly different, not high-contrast), lowered its Height Range from 0.05→0.01 (its default height detail read as too strong), and set the Height blend mode to **Replace**. Masked with `Metal Edge Wear` generator (Invert True) plus an added `HSL` filter isolated to color-only to darken/desaturate. Hand-painted extra cracks using the built-in **Leather brush** (with Flow enabled instead of just Opacity, for more natural buildup), finished with a `Threshold` for crisp edges (frame_009 — viewport close-up mid-stroke with the Leather paint brush, brownish leather-strap material visible, distinct paint/wear brush thumbnails in the shelf).
34. **Height Position** (not just Height Range) is called out as the control for how "thick"/how far above the raw-leather base level the leather-skin layer sits — raising it lets the leather-skin layer visually sit above (rather than sink into) the raw leather below.
35. `Stain` fill (Multiply, Roughness 0.3) via `Clouds` (Balance/Contrast tuned) + `Grunge Dirt Scratchy` (Multiply, Invert True) for color-variation flecks; masked additionally with an **anchor from the Leather Skin layer's own mask** (multiply) so staining only lands on the visible skin, not the raw-leather-revealed areas.
36. `Cracks` fill (BaseColor blend Soft Light, Height negative, Roughness high) via **`Leather Damage`** fill, `Blur`, then **`Bevel Smooth`** (small Distance, Smoothing, offset Curve Shape, Mask Threshold ~4) plus aggressive `Sharpen` (value 4) then **Invert** — the combination reads as convincing river-like leather cracking; author explicitly notes Bevel Smooth's Smoothing/Curve Shape parameters are what turn a hard procedural edge into a soft, "filled-in" organic curve.
37. Extra edge-crack detail layer (Height 0.65) via the Leather Skin anchor + `Bevel Smooth` (Distance ~825→ ~0.03/0.24/0.08-range tuning) for curled-up edges, plus `Warp` for irregularity — same anchor→bevel→warp→multiply-punch pattern used throughout the video.
38. **Stitches**: added via the built-in **stitch/path tool ("Top Stitch")** — a curve/spline tool: click along a seam to lay down control points, tune Spacing (~0.25–0.3 to un-clump touching stitches), stitch color, and toggle Vertical/Horizontal/Imperfections stitch variants. Key limitation called out: stitch parameters are per-stroke — **the first stroke's settings should already be exactly what's wanted**, because to edit an existing stitch path later you must reselect the path tool, click the specific path (highlighted blue in a Paths list), then adjust.

**7. Model Details — adding geometry-level detail purely in texture (§ Model Details, 99:38–124:49)**
39. **Normal stamps**: any hard brush + a Normal-Stamp alpha (Painter ships several; more available for purchase) dragged into the **Normal channel** of a paint layer placed at the very **bottom** of the stack (so cavity/curvature generators built later can pick the bumps up "as if modeled and baked"). Full Preview mode (toggle in the upper-left, described in-video as looking like "Flubber") shows the stamp live before clicking. Ctrl+right-click-drag scales the stamp; Ctrl+left-click-drag rotates it. Used for vents, screws/ball-bearings, thumb switches, and a sci-fi service-panel door (frame_010 — Assets shelf showing purple/magenta Normal-Stamp thumbnails, a "Handle Circle" stamp tooltip visible, viewport showing the helmet in grayscale material-preview mode).
40. `Edges Extrude` model-detail layer: `Curvature` generator (Mode=Edges→Sharp, Balance/Contrast raised, Global Invert True) picks out panel edges, refined with **`Bevel Smooth`** (Smoothing rounds it into a "purposeful," non-raw-procedural bump) — used to add extra hard-surface panel detail (e.g. around an ear-cup) purely from curvature, no new geometry.
41. Complex multi-material ear-cup insert: **Polygon Select** a notch pattern directly on the mesh in the 2D flat/UV view (counted rows of quads for symmetry), `Bevel Smooth` to round the cut, an **anchor point** on the shape ("Ear Shape Outline") run through **`Mask Outline`** (Threshold 0, Width 0.01, Blur 0.01) for a seated/inset look, then hand-brushed extra material variation using the **Alignment = UV** setting under Brush Projection ("painting in the UV view but still technically 3D projection by default — switching Alignment to UV avoids brush-size/angle distortion when you're deliberately working in the 2D/UV viewport").
42. **Pipe cage** (mechanical cage detail around a cable/pipe): `Metal Cage` base fill (shiny metal), folder-masked to the pipe geometry, then a **`Hexagon`** generator fill on top (Tiling, Balance, Contrast+Invert tuned for hole size) plus a `Threshold` + **Anti-Aliasing FX** filter for crisp cutout edges — individual hexagon holes can be **dragged directly in the viewport, and Alt-dragged to duplicate**, letting the artist hand-place/skip specific cage holes procedurally-then-manually (frame_011 — Generator/Fill Properties panel on a "Hexagon" layer nested inside "Model Detail → Pipe Cage," UV Transformation Tiling/Rotation/Offset sliders, layer stack showing Pipe Cage folder structure).
43. Orange rubber gasket detail: base + colored fill + hand-chipped paint layer, refined with `Bevel Smooth`, `Blur`, and a `Levels` push for a lip/rim look; a `Dots` fill layer uses **inverse-subtract mask math against the orange layer's own mask** (i.e., reusing an existing mask as a starting point for a *new*, related mask rather than building from scratch) plus `Bevel Smooth` + `Threshold` for perfectly centered grip-dot indentations.

**8. Decals, Stickers, Text (§ Decals, 124:49–143:20; § Fonts/Wires, 173:35–181:22)**
44. **Custom Sticker tool**: drag directly onto the 3D model — gives a movable/rotatable/scalable (W/E/R) sticker gizmo. Load a custom image (creator credits decal sheets by Jonas Ronegard) into the Assets shelf first, tagged as a Texture resource, then assign it to the sticker. Exposed sticker parameters: Outline (thickness/color), Wear and Tear (Edge Wear, Folds Intensity/Density, Sticker Damage amount+intensity, residue color), Height Range. An `HSL` filter (color-only) desaturates/darkens a sticker slightly so it doesn't read as "brand new" (frame_012 — full helmet viewport with multiple decals/stickers/checker-wrap already applied, layer stack showing Decals/Model Detail/Coating/Fabric/Leather/Plastic/Paint/Metal folder order).
45. **Branding/logo decals**: drag an image straight onto the model → choose "mask" behavior → position/scale → add Height (Replace) and optional Roughness.
46. **Transparent/clear stickers** (e.g. a decal sheet's plastic backing): use the sticker tool but disable every channel except Height and Roughness (no BaseColor) so only a subtle raised/shiny outline reads — small Height Range (~0.3), softened Folds Intensity, boosted Roughness for shine; layered a separately-colored solid sticker "behind" it to fake a colored decal seen through clear plastic.
47. **Checker-pattern vinyl wrap / bent-surface decal**: drag a `Checker 1` procedural directly into BaseColor, Tiling ×8, then switch to **Edit Vertices** mode (via the Transform/Warp tool) to manually drag the projection's corner points in 3D so the flat decal bends/wraps around curved geometry; **Symmetry X** set from the *projection settings* (not a general mirror toggle) to mirror the bend; finished with a `Levels` lift on blacks + a Multiply-blended yellow fill for a black-and-yellow warning-checker look (frame_013 — full checker decal wrapped across the helmet's crown, layer stack showing "Checker 1," "Decal Label," "Label Backing," "Triangle Backing," "Grape Border Triangle," "Screen Dirt" entries).
48. **Anchor-driven grime specifically for a decal**: a decal backing's own Height channel is extracted via **anchor "Extract Alpha" set to Height** so a follow-up grime layer can build dirt that respects the decal's exact silhouette (Mask Outline for blurry edge → Levels for hot-core/faded-edge falloff → Clouds for breakup → Grunge Dirt tiled → the same anchor again, inverted, Multiply, to punch the center clean so grime reads as "collected on the edges").
49. **Text/fonts on cables**: drag a custom `.otf`/font file onto the shelf (Painter recognizes it as a font resource; import scope = project or full library), type text directly in the 2D or 3D viewport, drag onto a UV-unwrapped strip (cables were laid out horizontally in UVs specifically to make this easy). Useful text controls: **UV Wrap** set to Horizontal-only (keeps text from stretching around the whole wrap), **Advanced → Character Spacing** for a more "printed" look, Alt-drag to duplicate a text instance (frame_017 — font-thumbnail asset browser labeled "Ag," cable/wire 3D mesh isolated in viewport for text placement).

**9. Overlays — the unifying top-of-stack composite pass (§ Overlays, 143:20–169:49)**
50. New `Overlays` folder at the very top of the whole stack (pass-through on all channels) — deliberately mirrors real-world prop-making order: build it, paint it, apply effects/washes on top.
51. `Cavity` fill (BaseColor darker at ~40% opacity, Roughness ~0.9, Metallic 0): mask from `Curvature` generator with **Mode switched from the default "Edges" to "Cavities"** (author demos all 4 curvature Modes — Edges/Cavities/Unprocessed/Dual — noting "Unprocessed" is the raw, uninterpreted curvature bake useful when you want full manual control via a Levels node afterward), tuned Sharp/Soft/Medium detail levels, then blended a `Grunge Dirt Scratched` **Texture image input inside the same Curvature generator** (`Use Texture = True`, high Texture Opacity, large Scale) for extra tooth (frame_014 — Curvature generator Parameters panel: Global Invert/Blur/Balance 0.44/Contrast, Curvature section, Use Texture/Use Micro Details toggles).
52. Added `Ambient Occlusion` on top of the same mask (Global Balance lowered, Global Invert True), then set the **layer's blend mode to Screen** so the AO contribution adds to the curvature-cavity contribution rather than replacing it — described as recreating the classic prop-painting "wash poured on and wiped away, pooling in recesses" look.
53. `Edges` fill (BaseColor 1, Soft Light blend) using the **`Paint Subtle Scratched` Smart Mask** directly (all 3 of its exposed sub-masks used) — tuned inside the **Mask Editor**: Balance/Contrast, per-texture-slot Blend Mode (Soft Light on texture 1, Subtract on texture 2) and per-slot Scale/Opacity — brightens edges to complement the cavity darkening.
54. `Cavity Broad` — a second, softer/bigger cavity pass built from scratch via the **Mask Editor generator** (typed in fresh rather than dragging a Smart Mask, to show it can be hand-built): Global Balance up, Curvature Mode=Cavities, Big weight maxed, Multiply blend, Roughness opacity lowered.
55. Dirt pass 1 — `Dirt`: dark-brown BaseColor, Roughness 0.9, Metallic 0, masked with **`Grunge Leak Small`** switched from UV to **Triplanar projection** (fixes inconsistent drip direction caused by non-uniform UV island orientation), Hardness raised. Direction control added via a **`Light` generator** in the mask (Polar/Azimuth angle position the "light" so its falloff aims drips toward the top), **Multiply** blend so its black areas punch through and white goes transparent — used to bias drip/dirt accumulation toward the top of the object as gravity/weather would (frame_015 — Light generator Parameters panel: Polarization Angle, Azimuth Angle, Highlight Sharpness, Highlight Level, Light Attenuation, Image Inputs = World Space Normal/Position; layer stack shows "Dust Level," "Grunge Leak Small," "Light," "Ambient Occlusion," "Corrosion" entries).
56. Dirt pass 2 — `Mask Builder` (legacy) generator used deliberately (vs. the newer Mask Editor) for its built-in extra grunge presets: Contrast, Grunge amount, Curvature (range set to "concave," Smoothness) tuned, screen-blended in.
57. Dirt pass 3 — `Smeared Dirt`: **`Grunge Wipe Dusty`** (Triplanar, tiling 3) for speckles, then a **`Warp` filter driven by a custom image (`Leaky Paint`) as its Source Mode instead of noise** for directional smear ("maybe he's going fast — pod-racing helmet now"), `Sharpen` on top for crisp specks over a soft gradient base.
58. **Phil Robb photo-overlay trick** (credited, ex-Turtle Rock Studios art director): a subtle image with varied color/junk (`Rusty Overlay`) dropped into BaseColor at **Soft Light** blend, opacity pushed very low, with a `Levels` midpoint nudge — deliberately non-procedural, photo-derived color noise that breaks up flat/CG-looking color without reading as an obvious "effect."
59. Final `Cavity Sharp` pass: BaseColor 0 (hardcore black), Roughness 0.9, Curvature Mode=Cavities→Sharp only (Fine ~0.5) — a tight, high-contrast outline pass over everything, described as the very last overlay before moving on.
60. **Picking up model-detail bumps in generators**: Curvature/Cavity generators have a **"Use Micro Details"** toggle under Image Inputs — wiring the earlier Normal-Stamp anchor point in as the Micro Normal (and optionally Micro Height) source makes curvature/cavity generators react to the stamped detail exactly as if it had been sculpted and baked, even though it only exists as painted-in normal-map detail.

**10. Emissive (§ Emissive, 169:49–173:35)**
61. The project's shader template didn't include an Emissive channel by default — added manually via **Texture Set Settings → Channels → +** → choose `Emissive`, format **`L8`** (single 8-bit grayscale channel — cheap to pack into a spare RGBA slot on export rather than a full RGB emissive) (frame_016 — Texture Set Settings panel: General Properties, Channels list with Base Color/Height/Roughness/Metallic/Normal already present, Shader Instance "Main shader," Mesh Maps section).
62. Painted a black-and-white emissive mask by hand (paint layers named e.g. "Inner Light," "Ear Light") — kept it grayscale-only in Painter (viewport preview needs a manual **Emissive Intensity** bump in Shader Settings and an sRGB color swap to actually see a glow with bloom in the 3D viewport's post-effects; does **not** preview correctly in the Iray/raytrace renderer) — actual coloring/intensity is deferred to Unreal after export, since Painter is only producing the black-and-white mask.

**11. Glass / Transparency (§ Glass, 181:22–188:13)**
63. Prerequisite: switch the Visor texture set's shader preset to one that supports transparency — **`Metal Rough with Alpha Blending`** (vs. `Alpha Test`, which only supports hard cutout, not gradients) — and add an **Opacity** channel (without it nothing is transparent regardless of shader).
64. Base glass fill: Roughness ~0.1 (very smooth), Metallic 1, Opacity ~0.2 — already renders correctly in the **Iray raytrace renderer** (camera-icon button), showing real refraction/see-through (frame_018 — full helmet with visor still plain glossy white/cream, i.e. captured just before detail passes on the glass — texture-set list shows separate "Visor" and "Helmet" entries).
65. Detail passes on top: `Fingerprints` (`Dirty Grunge Fingerprints`, large tiling, moderate Balance), `Smudges` (`Wipe Smudgy Soft` Multiply + `Clouds` for uneven cleaning), `Edges` (built from Ambient Occlusion — Global Invert, Blur, Balance — plus `Fingerprints Smeared` tiled to roughly hand-size, `Sharpen`), and `Scratches` via the **`Scratches` generator** with Fade Mode set to **Start and End** (tapers both ends of each scratch spline rather than one).

**12. Finish, PBR Validate, Export (§ Finish, 188:13–198:25)**
66. New `Finish` folder at the very top (pass-through all channels). Added `MatFX AO` (Ambient Occlusion) generator fill twice: once feeding **Height** (auto-picks up the earlier model-detail bumps) and a duplicate (Alt-drag up) switched to feed **Normal**, set to **Multiply** — combines AO-in-cavities from both the height-based model detail *and* the separately-baked normal-stamp detail, "seating" every added detail as if it were truly modeled.
67. A global-control paint layer at the very top (Pass Through, all channels) is used for last-mile universal adjustments — e.g. a `Sharpen` or `HSL`/`Levels` applied across the entire stack at once, rather than hunting down individual layers.
68. **`PBR Validate`** node dragged to the very top of the stack — a diagnostic overlay (not a real material change) that flags BaseColor values outside a plausible albedo range for the target engine's tone-mapping. Set **Albedo Dark Range = 50, sRGB (Unreal preset)**; areas painted red are too dark (risk of crushing to pure black once through Unreal's ACES tonemap) — fixed by adding a `Levels` node inside the top global-control layer to lift shadow BaseColor values slightly. Turned the validator back off once corrected (frame_019 — Filter panel on a "Sharpen" filter, Sharpen Intensity slider ~0.35, layer stack showing a "Finish" folder area).
69. **Export**: `Ctrl+Shift+E` opens Export Textures. Output template used: a custom `CC_U_UDIM` preset (author's own naming-convention preset, not a stock one) — walks through the **Output Template editor's naming-variable picker** (project name, texture set name, per-map suffix like `BC`, and a UDIM token). Shows the packed-map layout used: **Normal map RGB channel-packs BaseColor's alpha slot as Opacity/Mask; a separate "PBR" map packs AO→R, Roughness→G, Metallic→B, Emissive→A**; Normal export format set to **DirectX** convention. Per-texture-set overrides are available (e.g. disabling Mask-map export for a texture set that doesn't need it, excluding specific UDIM tiles, or swapping a UDIM-suffixed filename for a non-UDIM one on texture sets that don't use UDIMs) (frame_020 — Export Textures dialog: Settings/Output Templates tabs, preset list on the left including several stock engine presets, output-map row assignments with color-coded channel chips, "4 output maps will be exported" note).
70. Exported directly into an Unreal Engine project's content folder; Unreal auto-reimports on file write. Post-import checklist called out live: **turn off sRGB on the packed PBR/Normal/Mask textures** (they're linear data, not display-referred color, so leaving sRGB on visibly wrecks Roughness/Metallic/AO/Normal) and, for the glass material specifically, **clamp Max Roughness** because the raw exported roughness read as too rough/frosted in Unreal's real-time renderer compared to Iray (frame_021 — finished helmet rendered live in the Unreal Engine viewport with visible emissive glow on the ear/cheek area and a lit character head inside the visor).

### Layers / Tools / Settings
**Generators used repeatedly:** `Curvature` (Modes: Edges/Cavities/Unprocessed/Dual; params Global Invert/Blur/Balance/Contrast, Sharp/Soft/Medium/Big weight sliders, Use Texture + custom image input, Use Micro Details for picking up Normal-Stamp anchors), `Metal Edge Wear` (Wear Level, Wear Contrast, Grunge Amount, Edge Smoothness, AO Masking), `Scratches` (Spline Number/Scale/Width + Random variants, Distortion + Frequency, Fade Length, Fade Mode Start/End), `Ambient Occlusion` (Global Balance, Global Invert), `Tile Generator` (Pattern: Grid/Hexagon/Pyramid/Custom Image; Tiling, Balance, Contrast, Random Rotation/Scale, Position Offset), `Hexagon`, `Light` (Polar/Azimuth Angle, Highlight Sharpness/Level, Light Attenuation — used as a directional mask driver, Multiply-blended), `Mask Editor` / `Mask Builder` (legacy) — hand-buildable equivalents of Smart Masks.
**Filters used repeatedly:** `Sharpen` (Intensity, e.g. 0.15–4 depending on how aggressive), `Bevel Smooth` (Distance, Smoothing, Curve Offset, Curve Shape, Mask Threshold, Distance Map + Multiplier, Reverse Wrap) — the single most-used filter in the video, for turning hard procedural masks into soft physically-offset edges, `Warp` (Intensity, Source Mode incl. Custom Image, Source Blur/Tiling, Blur), `Mask Outline` (Threshold, Width, Blur, Curve Shape), `Threshold`, `Levels`, `HSL` (isolatable to Color-only), `Quantize` (posterize-style step count), `Anti-Aliasing FX`.
**Smart Masks / stock materials used:** `Paint Subtle Scratch`/`Paint Subtle Scratched`, `Dust Stain`, `Fabric Cotton Jersey`, `Rubber Raw`, `Leather Skin`, `Grunge Paint Scratched`, `Grunge Dirt Scratchy/Scratched`, `Grunge Scratches Rough`, `Grunge Map 007`, `Grunge Leak Small`, `Grunge Wipe Dusty`, `Grunge Fingerprints Smeared`/`Dirty Grunge Fingerprints`, `Grunge Concrete Burnt`, `Grunge Dusty Scratch`, `Grunge Plaster Paint`, `B&W Spots 2`, `Clouds 1`, `Gaussian Spots 2`, `Leather Damage`, `Gradient Flakes`, `Checker 1`.
**Anchor point pattern (used 6+ times across the video):** bottom paint layer with black mask → right-click → Add Anchor Point → any Fill/Paint layer above sets its mask source to that anchor → optionally chain a `Bevel Smooth`/`Warp`/`Mask Outline` after the anchor reference, then re-reference the anchor a second time with **Multiply** blend to punch/refine the result — this "reference the same anchor twice with different post-processing" pattern recurs in Paint, Leather, and the decal-dirt sections.
**Channel-blend-mode gotcha (repeated teaching point):** Painter's layer opacity/blend-mode controls are **per PBR channel**, not global to the layer — switching BaseColor to Pass Through does nothing to Height/Roughness/Metallic. Fix: right-click the layer/folder → **Apply to all channels**. Height channel specifically is switched to **Replace** (not the default Linear Dodge/Add) whenever a layer needs to fully override buried detail below it (shiny-metal pockets, plastic panel inserts, gasket lips).
**Projection modes:** UV (default), **Triplanar** (used constantly on materials/grunges applied across UDIM seams or non-uniform UV orientation — e.g. Rubber Raw, dirt drips, cavity texture breakup), **Match per UV Tile** (used specifically for UDIM-spanning noise so it doesn't re-tile per tile).
**Texture Set / channel setup:** Emissive channel added manually via Texture Set Settings, format `L8`; Visor texture set uses shader preset `Metal Rough with Alpha Blending` + an Opacity channel for glass.
**Tools:** Custom Sticker tool (3D-gizmo-driven decal placement, W/E/R move/rotate/scale, exposed Wear-and-Tear/Folds/Damage/Height-Range params), stitch/path tool ("Top Stitch," curve-based, Spacing param), Text/Font tool (drag `.otf` onto shelf, UV Wrap Horizontal, Advanced Character Spacing), Edit Vertices (under Transform/Warp) for bending a flat decal projection around curved geometry, Polygon Fill / Mesh Fill / UV Chunk Fill selection modes, Full Preview toggle for brush/stamp visibility.
**Finishing:** `MatFX AO` (Ambient Occlusion generator) duplicated to feed both Height and Normal-based cavity pickup; `PBR Validate` diagnostic node (Albedo Dark Range preset e.g. "50 sRGB (Unreal)").
**Export:** `Ctrl+Shift+E`; custom UDIM-aware naming-convention output template; packed maps = Normal(RGB)+Opacity/Mask(A), PBR(AO=R, Roughness=G, Metallic=B, Emissive=A); Normal format DirectX; per-texture-set/per-UDIM-tile export overrides.

### Difficulty
Advanced. Assumes comfort with the Painter basics (fill layers, masks, folders) going in, then builds almost every technique on top of anchor points, multi-layer generator stacking, and per-channel blend-mode control — genuinely advanced non-destructive workflow, not beginner material despite the didactic narration.

### App & Version
Not stated on screen or in narration, and no version number/UI-chrome timestamp is visible in any captured frame. However, the video repeatedly and centrally uses the **`Bevel Smooth` filter** — per this skill's own version-history research (`references/release-notes-painter-11.0.md`), `Bevel Smooth` was one of 6 new filters introduced in **Painter 11.0.0 (2025-03-11)**. The creator explicitly calls it "somewhat new" ("I don't know what I was doing before"), consistent with having adopted it not too long after release. This places the video at **Painter 11.0.0 or later**. It also uses the **Custom Sticker tool**, which per `release-notes-painter-9.1.md` shipped earlier, in Painter 9.1.0 (2023-11-07) — consistent, not contradictory. No PBR Validate node history is tracked in this skill's release-notes backfill, so that feature's introduction version is unconfirmed. Given the Bevel Smooth lower bound and no signs of the 12.1.0 OpenPBR-default UI (shader dropdown shows classic `Metal Rough` presets, not OpenPBR) or the 12.1.0 Baking Mode UI split, a reasonable estimate is **Painter 11.0.x–11.1.x**, but treat the exact patch as unconfirmed.

### Tags
layers, fill-layer, paint-layer, masks, smart-mask, smart-material, generator, anchor-point, blend-mode, curvature, ambient-occlusion, tri-planar, procedural, MatFX, udim, texture-set, pbr, metal-rough, basecolor, roughness, metallic, height, normal-map, emissive, opacity, alpha, iray-render, export, export-preset, channel-packing, game-engine, unreal-export, advanced

---

## Related Tutorials
- [How to make SKIN TEXTURES in Substance Painter](how-to-make-skin-textures-in-substance-painter.md) — same creator (J Hill); this video is the explicitly-named prequel this tutorial opens by referencing ("four years ago I made this video about texturing skin... this is the sequel"). Shares the same layered-procedural-noise-mask + hand-paint-on-top pattern and folder-per-material/per-tissue-layer organization (there: Sub-Dermis/Dermis; here: Metal/Paint/Plastic/Leather/Fabric), but that video predates this one's use of anchor points and the `Bevel Smooth` filter (see its App & Version note — UI evidence suggests it's from before Painter 8.3.0, several versions earlier than this one's 11.0.0+ floor).
Future ingests covering anchor points (Jared Chavez's "Building Masks Explained," "Peeled Paint Effect with ANCHOR Points"), leather/fabric materials, decal/sticker workflows, or PBR export-to-Unreal pipelines should also cross-link back here — this video is the deepest single source in the library on anchor-point-driven multi-effect masking, the Bevel Smooth filter, and the Overlays composite pass.
