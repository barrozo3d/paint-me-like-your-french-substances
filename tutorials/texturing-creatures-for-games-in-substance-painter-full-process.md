---
title: Texturing Creatures for Games in Substance Painter | Full Process
source: YouTube
url: https://www.youtube.com/watch?v=dHATe4tKd_Q
author: Logan Wiesen
ingested: 2026-08-12
app: "Substance 3D Painter"
version: "not specified (modern UI, standard Baking Mode/Mesh Map Bakers panel, no version-pinning element visible)"
tags: [layers, fill-layer, paint-layer, masks, baking, mesh-maps, curvature, ambient-occlusion, thickness, world-space-normal, position-map, id-map, blend-mode, procedural, tri-planar, basecolor, roughness, normal-map, color-management, texture-set, export, advanced]
extraction_status: complete
frames_dir: tutorials/frames/texturing-creatures-for-games-in-substance-painter-full-process/
frame_count: 10
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Texturing Creatures for Games in Substance Painter | Full Process

**Source:** [YouTube](https://www.youtube.com/watch?v=dHATe4tKd_Q)
**Author:** Logan Wiesen
**Duration:** 56m54s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hey, Logan here. In this video, we're going to do a deep dive into creature texturing in Substance Painter.
[0:06] More specifically, creature texturing for real time creatures or game ready creatures.
[0:13] So in this video, we're going to learn some fundamental principles, as well as some practical applications that are just going to help you with any future texturing that you do.
[0:23] And by the end, you'll be able to texture creatures just like this. And it's going to be great.
[0:28] So let's get straight into it. So I just set up my scene in Substance Painter here, I have my low poly version of my model right here, with just a basic base texture with a color set to 0.5 value, and a roughness value set to 0.5, just so that we can see our model pretty clearly here.
[0:48] And you see we have two texture sets, we have the body, and we have the mouth. So these are, this is the building block of what we're going to be doing here.
[0:58] Now, I should note that the sculpt itself is very, very well detailed. Now, in order for you to get the most out of your texturing, in order for you to have the best texturing experience, in order for this to be the quickest and the best texturing method, you need to have a really, really good model.
[1:20] You cannot out texture a bad model. So you really need to spend the time in the sculpting stage to build up the proper primary, secondary and tertiary forms until you get something that reads well through the sculpt itself. Because if you can look at a sculpt and just immediately tell how something feels like this scaly area here, you can kind of tell how that feels just by looking at it. And that is what's really going to help with texturing.
[1:48] It's just going to speed up the texturing progress. So texturing ultimately starts with the model. So you really have to take your time during this sculpting stage to build out a really, really good model in order for the texturing stage to go as smoothly as possible.
[2:06] And on top of all of that, we can use all this sculpted detail in here, like all the skin pores, all this kind of stuff, it's going to get baked into a curvature map so that when we are texturing, we can utilize the actual detail of the sculpt or of the model itself and create more accurate texture maps that way as well.
[2:25] So I've exported out both my low poly and high poly versions. The high poly is just a decimated version. I use a decimation master here, sitting in around 800,000 points here, just so that we get a nice clean performance inside of painter.
[2:41] If this was like a complete portfolio project, I probably would go a little higher just so that we get as much detail as possible. But for demonstration purposes, 800,000 is totally fine.
[2:52] So to bake the maps here, we're just going to come up to the bake tab, and you'll see that I already have my high poly model loaded in right here.
[3:00] And the cage distance, this is something that you can kind of play around with you can test with distance base. I believe this is the default distance based is going to set a certain distance around the entire model as the cage.
[3:14] This can work great. Sometimes it doesn't work the best for everything. But when you're using this, you just want to set the max frontal distance to as low as possible without getting any of the red artifacts. So this is a little too low.
[3:28] But something like that, that would be a good baking distance for the distance based cage version here.
[3:35] Alternatively, and this is what I recommend using is the automatic, you can see it says experimental and there are a few kind of weird things going on here.
[3:44] But I have noticed that even though the cage is a little messed up here, I don't get artifacts from this like it's a really nice clean bake, even though it's an experimental.
[3:55] So play around with it. Maybe you get some artifacts with this, maybe distance base is better, but play around, see what works better.
[4:01] So first of all, we're going to make sure that we have all of our necessary maps checked here. So we want we're looking for normal, world space, normal ID, ambient, occlusion, curvature, position and thickness.
[4:12] These are all maps that we're going to need for creating better textures.
[4:17] Some of these substance painter just needs to like read and understand how the model actually works.
[4:22] So we're going to start by baking all of these at just one K, just so that substance painter has all the necessary files that needs.
[4:30] So we're just going to bake those real quick.
[4:32] Just at one K, we don't need super high resolution for these.
[4:35] But after this is done, then we can come up here to 4K, we can set the output size to 4K, and we can get rid of world space, normal ID and position and probably even thickness too.
[4:48] Just so that we have curvature, ambient, occlusion and normal, because these are the highly detailed maps that we want to see those extra details inside of Zbrush, like all the skin pores, all these kind of things.
[5:00] These are what's really going to show through in the curvature map.
[5:05] It's going to show up in the ambient occlusion map.
[5:07] And then of course, the normal map.
[5:08] So we're just going to bake these out here.
[5:10] Just let substance painter do its thing while it takes a few minutes to bake out all the maps.
[5:15] And now if we return back to painting mode, you'll see that all of our textures are baked in.
[5:21] And this looks almost exactly like our model straight from Zbrush.
[5:26] So that is perfectly what we want.
[5:28] There's no artifacts.
[5:30] I recommend just going around, moving the lighting to check if there are any artifacts.
[5:35] And it seems like we have a pretty clean bake here.
[5:39] So one thing I should note is that the environment is actually set to Studio Tomoko right here.
[5:46] By default, I believe this is set to this one, Panorama.
[5:50] And this kind of gives like a slight greenish hue to the lighting, which I really don't care for.
[5:56] Honestly, Adobe should just make Studio Tomoko like the default, the default environment map, because every single artist that I know complains about that.
[6:06] So Adobe, if you're watching this, change the default one to Studio Tomoko.
[6:10] But anyway, now we can actually start texturing now that our maps are all baked out, come up here.
[6:16] And you might need to change your document size because it might be pretty low and then you won't be able to see all of the extra details in here.
[6:24] So be sure that you have this set to 4K.
[6:27] And this is just the actual document resolution of the textures that we're seeing here.
[6:34] So the absolute first thing that we're going to do is just get a rough, very rough base color.
[6:40] I'm thinking something pretty pale and almost dead feeling for this particular creature.
[6:48] So we're just going to go something like this.
[6:49] I don't want to go too saturated because I want the character to feel kind of ghoulish.
[6:55] So I think we're going to go right around there.
[6:58] And then this base fill layer right here is going to have just a roughness value of 0.5
[7:03] just so that we have a base roughness value.
[7:06] Now we can get into the building up the textures.
[7:11] Now, working from the bottom to the top, it's very similar to sculpting in the sense that we're going to be working from the largest shapes to the smallest shapes.
[7:21] So we're essentially going to have our primary, our secondary and our tertiary details inside of the texture maps.
[7:30] And one of the ways that we really like to start out the base textures, if we just take a look at the base color, it's completely blank.
[7:37] We have like no data in here, basically.
[7:40] So we're just going to create a new fill layer.
[7:41] We're going to call this curvature.
[7:44] And we're going to right click at a black mask and add a fill layer.
[7:48] In the fill layer, we are going to add our curvature map.
[7:55] I can spell it right curvature map.
[7:57] And we're just going to grab make sure that's the curvature body.
[8:01] We're going to get that.
[8:03] And now if you turn on in the base color, you can very roughly see it here.
[8:07] We have to change the color.
[8:09] So if we change the color down to something pretty dark, you can see what this is doing.
[8:13] So it's using the information of the sculpt, the high poly sculpt.
[8:18] And it's like crunching all the details.
[8:20] It's almost like if you ever used a high pass filter inside a Photoshop, that's essentially what this is doing.
[8:27] So what we can do is just right click at a levels and invert this so that the crevices are actually the darker parts instead of the crevices being the lighter color.
[8:38] So this is essentially just acting as like a cavity map.
[8:43] And that's going to help crunch the details out so that we get these nice, all of our sculpted details inside of the color map itself.
[8:52] That's just going to help make things look much nicer and cleaner.
[8:55] What we can do is just copy this control C, go to the mouth and paste that on there.
[9:02] And for the mouth color, we can just get a very rough base color going on in here.
[9:09] So the curvature map, this is a staple for anything that I'm texturing.
[9:14] I always end up using a curvature map.
[9:16] It's just so, so helpful when creating textures because you're essentially just extracting the data from your sculpt and putting that into the textures, which is really handy.
[9:29] And on top of the curvature map, I also like to use the ambient occlusion map.
[9:34] So I'm just going to create another fill layer with a black mask and a fill inside of there.
[9:41] Just search for ambient occlusion.
[9:45] Go here.
[9:47] And I'll just make the color a bit darker.
[9:50] And then we also need to add a levels and invert this as well.
[9:56] So you can see what the AO is doing.
[9:58] It's just creating some ambient occlusion in the texture.
[10:01] This is a bit much.
[10:02] So I'll just take it down just so that we get a little bit of ambient occlusion in the actual color map itself.
[10:10] Before we continue, I know there are a lot of you that struggle with creating studio quality 3D characters because it's tough when you don't have the right guidance.
[10:19] So I put together a full 14 hour training, walking you through the full process of creating a studio quality character portfolio piece.
[10:27] And right now there's an early bird discount.
[10:29] So the next 25 actually now 19 the next 19 new members get a massive discount.
[10:36] So the links in the description for that training, if you're interested.
[10:38] And then next utility map that we're going to add is going to be the thickness map.
[10:45] So this is what I meant when we were when I'm talking about using like those baked texture, the baked texture maps.
[10:52] These are really, really handy.
[10:54] So the workflow is the same for all any any baked textures that you're using.
[10:59] So curvature, AO, thickness, let's just add a fill layer, black mask, add a fill.
[11:05] We'll come in here and search for the thickness map.
[11:09] And what the thickness map does is let's come here at levels and invert this as well.
[11:15] So it's taking things based off of the actual thickness of the model.
[11:19] So so obviously the hands and the feet are going to be thinner than the torso area.
[11:26] But what this helps us do as just as just like creating a base texture is it's going to we can come in here
[11:34] and just change the color to like some kind of red.
[11:36] And you'll see immediately this looks more realistic because the hands and the feet are generally more red
[11:43] because there's more blood flow going to those areas than areas like the torso or the upper parts
[11:48] of the legs here, we see we're getting that red around the mouth.
[11:52] And that's exactly what we want.
[11:55] So we can also change play around with the blending mode, try multiply.
[12:02] And that actually looks pretty good.
[12:05] You can play around with the color here.
[12:07] Maybe we want something a little lighter, a little more saturated just so that we get some nice color
[12:15] variation going on in these certain areas.
[12:18] And then we can always change the opacity of the layer here too.
[12:24] Just until we get something that we're pretty happy with.
[12:30] And we can always come back and change these layers later.
[12:34] But for now, that doesn't look too bad.
[12:39] So when we're creating realistic textures, it's really just a process of layering things on top of each other,
[12:45] just continuously layering color and data on top of each other until we get something that we're happy with.
[12:51] Because there is so much variation in skin or anything organic that you're creating.
[12:58] You want to have as much variation as possible.
[13:01] So it's really just a matter of layering things on top of each other.
[13:05] But it helps to understand like the principles of layering and what layers you want to have in the outline here.
[13:15] So we need some more color variation in the skin here because skin is not just a solid color.
[13:21] Like I said, there is so much variation in it.
[13:24] And we have a little bit of variation going on with the thickness map that's helping us get some nice color variation around the hands, the face, the feet.
[13:32] But now what we're going to go in is we're going to do some hand painted maps.
[13:36] So first we're going to start off with some yellow tones because skin has like temperatures through it.
[13:44] So I'll show you what I mean right here.
[13:45] We're just going to create a black mask and a paint layer.
[13:49] And we're going to select a pretty yellow color here.
[13:53] So when painting skin, the areas where bone is closest to the skin,
[14:01] bone is closest to the surface, it's going to show up as a pretty yellow color.
[14:07] And I like to get a pretty broken up brush.
[14:09] I really like dirt number two.
[14:11] And I turn off the size pressure and enable the flow pressure.
[14:17] And now we can enable symmetry.
[14:20] Come in here and make my brush a little smaller, turn up the hardness there.
[14:27] And then we're just going to paint around where the bones are closest to the surface.
[14:33] So we have the sternum protruding out here.
[14:36] Obviously the ribs, we can go in here and just kind of hint at each one of the ribs individually.
[14:43] And this is also a part where like storytelling comes into play as well.
[14:48] Obviously, a lot of the storytelling for this character is done through the sculpting before the texturing.
[14:55] But you want the texturing to support the storytelling of the character.
[15:00] And when I say storytelling, I'm talking about making our model unique and appealing to look at.
[15:08] Or to have like a story behind it, you know,
[15:12] because ultimately our goal when creating characters or creatures
[15:16] should be to create something that resonates with the viewer through telling a story.
[15:21] And you can tell a story through materials, through just all kinds of different things
[15:26] like scratches, wounds, through details in the model, through the pose.
[15:32] There's just a lot of different ways that you can tell a story through the model.
[15:37] And texturing is one of the ways that we do that.
[15:39] So for this particular character, you can see he's got like torn up areas around here.
[15:45] Lots of scars and wounds going on, which probably indicates that he's been in a lot of fights.
[15:50] He's gotten the crap beat out of him.
[15:52] He's beaten the crap out of a lot of people.
[15:53] So that is the kind of story that we're we're creating the illusion of
[16:01] when we're creating a character like this.
[16:04] So we want to make sure that the the textures support the story that we're creating.
[16:12] So particularly on like the back here, these spines, these look really painful.
[16:18] So we can add some more variation, maybe make these red at the very tip,
[16:22] like the skin is really stretching and pulling and it's just really painful for the creature.
[16:27] So these are the kind of things that you want to be thinking about with
[16:32] with the storytelling of your creature or your character or whatever you are creating.
[16:39] So we have most of the bony spots here.
[16:43] We can go up here and add some yellow to the skull.
[16:50] And you see, I'm being pretty patchy with like the color here.
[16:54] I don't want to go in and just cover it all, make it one solid color
[16:58] because that's where we get like the nice kind of break up and the the underlying tones inside of the skin.
[17:07] So you can come in here and just kind of erase with by pressing X,
[17:12] you'll switch you'll switch between the add and then the add and the subtract on the black mask.
[17:20] So we'll just go in here.
[17:26] Just paint around where the bone is closest to the surface.
[17:30] So we're going to have elbows right back here.
[17:36] A bit of the radius or the ulna, excuse me, back here.
[17:42] Okay.
[17:52] And then we can also get a little bit on the knuckles here.
[18:00] So texturing is a mix between using procedural textures, baked textures and hand painted layers as well.
[18:09] And all of these things combined is what's going to help us create the most accurate and help us get a quick result or a good result fairly quickly.
[18:23] So I'll just finish painting.
[18:26] He's in pretty quick.
[18:28] And then understanding anatomy, of course, that's going to help with understanding where more of the yellow tones are in the body.
[18:37] But if you're creating a creature, you're sculpting a creature like this, you should know your anatomy pretty well, but it's just a good reminder.
[18:46] So that is our yellow. Obviously, it looks a little overpowering.
[18:52] So what we can do is play around with the blending modes.
[18:55] I tend to choose something like screen for the yellow tone, just because it kind of mutes it a little bit and it helps it blend in with the rest here.
[19:05] And then we can take down the opacity a little bit.
[19:09] And you see now it kind of looks like bone that's sticking through and protruding through here.
[19:14] And that's the yellow tones that we're getting in here as well.
[19:18] So the body has quite a few different tones.
[19:23] The main one or the bone one being yellow.
[19:27] The next one is a blue layer.
[19:31] We can do blue tones.
[19:35] And with the blue tones, these are going to be cooler tones or areas of the body where there might also be bruising.
[19:42] And we can also use this as sort of a hand painted cavity map for areas that we want more more cavity areas.
[19:51] So essentially, I tend to come in here and just go around and darken up some of the areas around here.
[20:04] And just go around and place the blue just so that we get some color variation in the model.
[20:14] And obviously you want to be looking at reference as well.
[20:20] I have reference on my second monitor of some creatures very similar to the style that I'm going for.
[20:31] So you can kind of take inspiration from other artists reference and how they approach the different color variations in the body.
[20:41] Because there's really so much you can do.
[20:44] And if you're creating a different skin tone creature, say like a green creature or something, the tones are going to be different.
[20:52] But there will still be those subtle yellow, blue and red tones in the model as well.
[20:58] So essentially, this blue layer is just acting as a secondary ambience occlusion or curvature map.
[21:13] So we can set this to multiply.
[21:18] And then we get those nice kind of deep blue almost purpley tones in the model here.
[21:28] And we're just trying to make these these crevices pop as much as we can.
[21:49] Coming down around the back here.
[21:52] And the reason we do like a slight color blue instead of just a black is so that there is still some saturation in the model.
[22:06] It's going to help keep things looking much more alive as opposed to just a black color where it's it feels kind of dead and not super live.
[22:16] So the blue is going to help keep things saturated and looking lively.
[22:22] So just finish getting the blues in here on the model.
[22:43] And then we can move on to the reds.
[22:48] So the reds are going to be areas where there's more blood flow on the body.
[22:55] So typically the head, the hands and then any wounds across the body as well.
[23:01] So let's just set this to a fairly bright red color.
[23:08] Something kind of like that.
[23:10] Right click at a black mask, add a paint layer.
[23:17] And we can come in here.
[23:20] And we're obviously going to want some red across the face here.
[23:25] And we can turn off symmetry, remove some of it from over here because when I had sculpted this, I wanted him to have this kind of burn damage going across the face here.
[23:37] That is going to help again, support the story that we had for this particular creature.
[23:48] There we go.
[23:50] And then we have these kind of fleshy areas right here.
[23:55] So we're going to want some more red tones in there.
[23:59] And you'll see that the colors themselves, they pop quite a bit like you can clearly see there's blues in here.
[24:06] Clearly see the yellows clearly see the reds.
[24:08] And all of this is going to come together more later.
[24:11] You just have to trust the process.
[24:12] You can also play around with the blending modes.
[24:15] Typically for the red tones, I like to choose something like overlay, screen or soft light.
[24:23] I think soft light is generally what I tend to use for the red tones just because it looks good, but it's also going to vary for every single model that you do.
[24:35] So just play around with the settings.
[24:37] Try to find one that you like because the blending mode is just going to make it more integrated into the color map with what's underneath it.
[24:45] I keep pressing that.
[24:47] Okay.
[24:49] There we go.
[24:52] And have some red tones coming through here where there's more blood flow coming through the veins like so.
[24:56] Same thing on this arm.
[24:58] And then of course the hands, we're going to want more red tones overall just from extra blood flow going to the hands.
[25:12] We don't want the hands to be too red.
[25:14] So we can remove some of this, but the hands, the feet and the head are generally going to be the areas where there is more blood flow going on.
[25:27] And we can just come in here.
[25:30] And then we can just come in here.
[25:31] And add some of those red tones back here to reinforce that story that these things are painful.
[25:41] And as we start to fill these up, you'll see that the red color is going to be a little bit more red.
[25:49] So we're going to add some of those red tones back here to reinforce that story that these things are painful.
[25:54] And as we start to fill these up, you'll see that the red contrasting with the yellows as well as the blues, it makes this look pretty painful, which is exactly what we are going for.
[26:11] So we can do kind of a similar thing right here.
[26:15] We have these kind of stretchy stretched out flesh bits right here.
[26:19] Obviously going to want some red tones going in through there.
[26:24] Same thing with under the pecs right here.
[26:30] And then where the muscle, the muscle tendons are actually stretched out here as well.
[26:35] So you just got to get creative with placing the colors in the textures.
[26:49] But once you do it a couple of times, you really starts understand the process and where certain colors needed to be placed and where to avoid placing other colors.
[27:05] So we're going to do that.
[27:19] Okay.
[27:21] And this doesn't look too bad right now.
[27:24] Going to add some red tones around the wounds.
[27:31] And then obviously if you're creating a creature, you're going to know where you placed all the wounds and the story elements that you really need to sell that.
[27:43] That creature and the story that's behind it.
[27:45] And then just be sure that you're you're supporting that story through the textures.
[28:01] Like so.
[28:05] And then we have these nice asymmetrical wounds as well, which is just again going to make the character feel more alive.
[28:14] And more believable as opposed to if everything is just symmetrical, then feels pretty unbelievable.
[28:28] Okay.
[28:31] And then in the model itself, we have these kind of muscle striations coming through here where the skin sort of been torn away.
[28:39] And those are going to we're going to really want those to shine and to be just a unique element of this creature.
[28:50] So we can come back to yellow tones, maybe and turn on symmetry.
[28:57] Have some of these tones just spreading out a little more just so that the line isn't perfectly straight and clean.
[29:05] So that we have some variation going on through here, like the bones are actually wrapping around the ribs.
[29:21] And then right here, there's another skin tear where the rib is poking through.
[29:28] We want to make sure that you have that showing and then we can remove the red tones from the rib there.
[29:39] Nice.
[29:41] Okay, so now we have our base skin tones.
[29:44] What we're going to do now is focus on making these feel more together and more integrated into the model while also adding further breakups.
[29:53] And the way we do this is through procedural textures.
[29:56] So we're just going to call this breakup one, not 12, one.
[30:02] And then we're going to right click on this, add a black mask, add a fill layer.
[30:07] And then we're just going to search for some kind of grunge map.
[30:12] And I really, I like this grunge cobweb.
[30:16] So we're going to select this, come up to projection type, change that to triplanar.
[30:23] And then we're going to get some kind of more organic color going on here.
[30:32] So probably some kind of orange, like so.
[30:40] Maybe a little more red.
[30:42] And then also play around with the blending mode here.
[30:44] We can change that to soft light.
[30:48] Maybe we want to change the tiling size.
[30:54] Cool. So you can see, we just get this nice kind of breakup on the texture map.
[31:02] And then it's going to help integrate the rest of the colors going on through here.
[31:11] All right, let's take a look at the curvature map.
[31:14] And I think I want to add a little more color to the curvature map.
[31:24] Just so that we get a little more saturation showing through the model there.
[31:34] And let's change the base color a little lighter.
[31:39] Yeah, that looks better.
[31:41] Now we have more of that pale kind of creature.
[31:45] More of that pale look that we're going for.
[31:47] Sweet.
[31:49] So what we can do, duplicate this breakup one, all this breakup two,
[31:55] and we can change this to a different color now.
[31:59] I tested this earlier.
[32:01] And I think a purple color and a orange color here for the breakups, they work pretty well.
[32:08] They kind of contrast each other.
[32:10] And if we set the purple one to multiply, where is that right here?
[32:18] You'll see that we get this nice kind of breakup.
[32:21] And then we can also change the grunge type here to something a little more interesting.
[32:29] Maybe the burnt concrete, that looks kind of nice.
[32:37] And of course, we can change the opacity if it's ever too much.
[32:40] But you can see just by adding these two breakups, it helps integrate the rest of the layers.
[32:48] So we get a more realistic looking result.
[32:56] Maybe lower the opacity of bony areas here.
[33:05] And then in the red tones, I want to come in here with symmetry turned off.
[33:13] And scale down my brush a little bit.
[33:21] And just come around here and kind of trace around where these fleshy bits are,
[33:30] just so that we get a little extra variation coming in through here.
[33:44] So just tracing kind of these burn marks going around through here.
[33:55] And then same thing through here.
[34:04] We get a little more contrast into the color map, you can just see that through there.
[34:09] And then on the blue tones, we can also trace over the veins, add some color to the veins.
[34:20] And that's going to also help the model feel a little more alive.
[34:25] Because veins help things feel alive because it actually imitates the illusion of blood flow through the model.
[34:35] So when creating characters or creatures, it's good to have, you know, the veins in the actual color map itself.
[34:43] And it just looks freaking cool.
[34:45] So you get that nice added element there.
[34:50] And you don't have to trace over all the veins.
[34:53] And some you can have more subtle than others.
[35:04] But it just helps with the overall texturing.
[35:10] Some veins on the leg here.
[35:16] And then this also comes back to like the layering as well.
[35:20] Because in real life skin, we actually have a lot of veins underneath our body.
[35:26] So getting these in is also going to help with the added realism and all that.
[35:34] So just having these veiny patterns kind of going through the skin.
[35:48] You can see how that's starting to add more and more realism.
[35:56] Same thing up here, we can have some going across the shoulder.
[36:00] You can even get like a vein brush, something kind of like this and go around and do that.
[36:09] I would be careful with this.
[36:10] Don't overuse this too much.
[36:13] But it can be a really powerful tool for getting nice, nice color variation in shapes and going on in here.
[36:29] Have veins going along there.
[36:33] Veins going through here.
[36:37] Veins on the calf.
[36:49] And there we go.
[36:51] So you can see that even with just a few layers that we have, it's already starting to come together and to feel much more realistic.
[37:03] As opposed to just having like a flat single color.
[37:07] We have these nice layers here, which are each playing a role into creating, you know, the variation, the breakup, creating a more realistic creature.
[37:16] And what we can do for some even further variation is we can duplicate one of our tones here and change the color to green.
[37:26] And for creatures, you actually can add green into the model and get away with it as some added color variation.
[37:34] In fact, I would recommend adding green to some parts of the model, just because it's added variation.
[37:40] And it's going to give a unique aspect to your creature.
[37:47] So if you just kind of go around and just add some subtle green variation around the creature.
[38:00] It's going to help it look more realistic.
[38:02] And also on bruised areas or more wounded areas, you can play around with throwing in some some green color tones, just to kind of see what works.
[38:16] So on this area here, we can add some green tones for that's going to kind of come across as bruising as well, which can be nice.
[38:32] There we go.
[38:40] I'm around to the back.
[38:46] Maybe there will be a little more green on the pits as well.
[39:03] And just some overall general color variation coming in through here.
[39:10] There's not really like a one size fits all approach when adding the green here.
[39:15] And it's going to vary from creature to creature.
[39:19] But you just kind of want to go in, add some some light break up going around.
[39:23] You could probably get away with using a procedural texture with a green as well.
[39:29] And then just kind of turn the opacity down.
[39:36] Then we just take the opacity down slightly.
[39:42] That doesn't look half bad.
[39:46] Maybe in the blue tones here, some of this is a little harsh.
[39:53] And we can probably go a bit darker.
[39:59] There we go. It's coming together pretty well, especially for only having spent like 35 minutes on this.
[40:07] And that's what I mean when I say that the sculpt is more important than the texturing itself, because we all a lot of this information that we have here is from the sculpt itself.
[40:19] And I couldn't imagine having to do like all of the the curvature and stuff by hand.
[40:25] So it's really, really important to have a good sculpt as a foundation before even bringing it into the texturing software.
[40:33] And if your your model is not as good, you're going to notice it pretty quick when you bring it into the sculpt or the texturing software, because you're going to just be like, OK, this this is tough.
[40:45] I really don't know where to start.
[40:47] Because you won't have like that curvature information to get something that looks decent.
[40:54] And speaking of curvature, we can actually come up here to fill air and add another curvature on top of this.
[41:01] So I had a fill.
[41:03] I'm here and search for curvature.
[41:05] And we can try out this one this time.
[41:10] See, we can pull that down.
[41:13] Play around with the balance here.
[41:17] And if that doesn't work well, then we can let's check it inverted.
[41:25] That's not giving us exactly what we want.
[41:28] We can just use the curvature of the body again.
[41:33] Come up to levels, invert this.
[41:36] And then we can also crunch this just down a little further.
[41:43] Like so.
[41:45] And then get a darker color going on here.
[41:54] Something kind of like that.
[41:57] Add a little bit of saturation into this.
[42:03] There we go.
[42:05] So without and with you see, it just crunches those poor details so that we get those nice extra crispy tells.
[42:14] Inside of the.
[42:17] The color map itself.
[42:19] So now what we could do is since we have all these layers, we can just kind of play around with the colors to try to get something that.
[42:30] That fits our model here.
[42:34] So if we want, I'm thinking it looks a little purple.
[42:38] So probably take down.
[42:40] The opacity of this layer.
[42:47] And we can play around with the color as well.
[42:50] Maybe make it a little more red.
[42:55] Or a little more blue.
[43:03] And then with the base here, we can just lighten this up.
[43:07] We go with the yellow tones.
[43:11] I'm going to make this slightly more orange.
[43:17] And make those pop a little more.
[43:20] I'm going to add some more yellow tones to the hands.
[43:27] And then we can add some more yellow tones to the hands.
[43:31] And then we can add some more yellow tones to the hands.
[43:38] Just because the hands are pretty bony.
[43:42] And they look a little too red right now.
[43:59] Nice.
[44:00] Nice.
[44:04] And for this thickness, I think we might actually go a little more yellow.
[44:15] Okay, and then the curvature map up here, I'm going to set this to let's see how multiply looks.
[44:24] And play around with the levels. Maybe we can crunch these even more.
[44:31] There we go.
[44:33] Because oftentimes you need to exaggerate something a little more than you think and then you can dial it back.
[44:49] There we go.
[44:51] We can also add some yellow tones into the face up here for some added variation.
[45:00] You see the yellow tones with the red.
[45:03] It just makes this look really gnarly, really painful, which is exactly what we're after.
[45:20] This looks really nasty right here.
[45:24] On this creature, he's definitely been through it.
[45:30] But ends up being a pretty nice result.
[45:34] So now generally at this stage, we need some feedback.
[45:39] So how do we get feedback on this?
[45:41] Obviously we can ask people, but the one of the best and quickest ways to get feedback when texturing is to export out the textures and bring it into a render engine.
[45:51] So I'm going to export out the textures, select my folder here, we can export these out at 4k.
[45:56] We don't need all the textures.
[45:59] We just need color and normal for now.
[46:04] We'll just do color and normal.
[46:08] Export both of those out.
[46:11] And then once those are exported, we can come into Blender and take a look at how the textures are doing.
[46:17] So I'll just split this, go to the shader editor here, take a look at rendered.
[46:22] I'm using EV.
[46:23] So it's just in real time.
[46:26] It's just a simple scene that I'd set up with a few basic lights.
[46:31] We take a look here.
[46:33] Just a few simple lights, three point light setup.
[46:36] And this is just to help us get feedback.
[46:41] And then we'll just select this control shift T select those.
[46:46] And we can take a look at how this looks in here.
[46:49] Let's check the normal space.
[46:51] I think that should be on direct X.
[46:54] Yeah, definitely on direct X.
[46:57] And it's not looking half bad.
[46:59] Actually, we can do the same with the mouth.
[47:02] Control shift T.
[47:03] Select these two.
[47:05] Change that to direct X.
[47:09] And now, now that we have this in the render engine, this gives us a lot of feedback.
[47:15] So we can see that the yellow parts of the texture are a bit too harsh.
[47:21] So we know that to tone those back and seems like the hands are a bit too saturated.
[47:30] So now we can use this feedback and we can go back into substance painter and change this.
[47:35] But first, I'm going to add some subsurface scattering.
[47:39] And this up.
[47:41] And then we'll just turn the scale.
[47:45] Just slowly increase the scale.
[47:48] Do we get something that works better?
[47:52] Sweet.
[47:53] We'll do the same with the mouth.
[47:55] Change the subsurface.
[47:56] Turn that on.
[47:58] And take the scale way down.
[48:01] Sweet.
[48:02] All right, now back into painter.
[48:05] We can come in here with the yellow tones.
[48:08] And I'm actually just going to.
[48:12] Make sure symmetry is turned on and just kind of remove these a little bit.
[48:19] And then we can also come in here and I think the whole most of the model could use a little more yellow.
[48:26] Into it.
[48:27] So I'm just going to come around.
[48:31] Just lightly.
[48:34] Create some more yellow tones on the rest of the model.
[48:39] Because I like that yellow tone color.
[48:43] Or this particular creature.
[48:50] And then we can go back into the color.
[48:53] And turn.
[48:56] The thickness down.
[48:58] I think that was too much for the hands.
[49:09] Sweet.
[49:10] And then the blue tones.
[49:12] We can come in here.
[49:14] Add a little more of a crevice.
[49:17] Right there.
[49:18] And we're just trying to make these portions on the texture pop as much as we can.
[49:24] We can come in here.
[49:26] Add some separation between the ribs there.
[49:29] And we're just trying to make these portions on the texture pop as much as we can.
[49:44] We can come in here.
[49:46] And add some separation between the ribs there.
[49:49] And we can come in here.
[49:52] And add some separation between the ribs there.
[49:55] Some separation between the chest striations.
[50:02] And shoulder striations.
[50:19] Let's go with something kind of like that for the blue color.
[50:25] Nice.
[50:26] And then for the curvature.
[50:28] I think we'll take it a little bit less saturated.
[50:32] Just because it was giving us that kind of really reddish tint.
[50:37] Which I think is a little too much.
[50:50] We can change the color of this break up here.
[50:53] Maybe go a little more yellow tint on that.
[51:02] Less green tones in there.
[51:06] And that also on the yellow tones.
[51:09] We can come up here.
[51:11] And paint the jaw.
[51:14] A little more yellow because that's a pretty bony part.
[51:17] I forgot to do that in earlier.
[51:25] Up here.
[51:26] And I think the whole yellow color could probably use a little more orange hue.
[51:33] We can take that down just slightly.
[51:36] Something like that.
[51:38] Maybe increase.
[51:41] Okay.
[51:42] Yeah.
[51:43] I actually like that.
[51:44] And once you have all the layers here, a lot of it's just kind of going back and forth and changing the colors, changing some painting on the layers themselves.
[51:54] Until you get something that you're happy with.
[51:57] So a lot of it is just back and forth.
[52:01] And then of course you obviously want to export out your textures.
[52:05] Check it inside of Blender.
[52:06] Make sure that everything looks good.
[52:08] So we can just do that real quick.
[52:11] Export textures.
[52:14] Export.
[52:18] And then inside of Blender.
[52:21] We'll just re-import.
[52:24] This is the mouth.
[52:27] Out there.
[52:29] Out there.
[52:30] And then be sure that on the normal we set this to non color.
[52:35] Same thing here.
[52:37] Body.
[52:39] Body.
[52:41] Body normal.
[52:42] Change this to non color.
[52:45] There we go.
[52:46] So now we're getting something that looks a lot nicer.
[52:49] And a lot of the texturing process is infused with like the look dev process because they really go hand in hand.
[52:57] You don't know exactly how your textures are going to look because obviously this doesn't look exactly how this looks because well there's not a shader in substance painter.
[53:07] So we're not actually seeing like the final result.
[53:10] So it's good to just keep kind of jumping back and forth between the substance painter and then whatever render engine you're using to get the most accurate result possible.
[53:22] So with a few more minutes of playing around and tweaking colors and textures, you can see for the most part we still have all of the same layers here.
[53:32] I did add some nails.
[53:34] So just a basic color for the nails here just to separate them from the rest of the body.
[53:41] And then I moved the red tones above the curvature just so that those really pop.
[53:46] And then I had another red layer here just to really emphasize the wounds and the fleshy bits on the texture here so you can see what those are adding.
[53:57] So all the wounds they have a lot darker red just so that they kind of they pop a little bit more and then they really show through the texture.
[54:08] But yeah guys that is pretty much the whole process for creature or creature texturing.
[54:15] And if we take a look at this in blender, you can see this is the result that we got.
[54:22] And I also added a rig to this just real quick and put it in a pose so we get something pretty menacing and we can really test the textures make sure that they really fit this creature.
[54:35] And I think the textures turned out pretty nice for this particular creature.
[54:41] But yeah guys that is the process so you really want to remember the fundamental principles.
[54:47] Good texturing starts with the model you have to have a good model before you even think about texturing.
[54:53] You really want to utilize baking maps or the baked maps so the curvature map the AO the thickness map those are all really helpful tools.
[55:03] And if you're not utilizing them then you're doing yourself harm.
[55:08] Layering you really want to focus on just building up the layers continuing to add breakup on top of breakup because that is what realism is there's lots and lots of breakup underneath each other play with around with the blending layers or the blending modes of each layer to get something that looks more integrated with with each of each layer.
[55:31] There's going to be a lot of color in the skin variation that's another fundamental principle.
[55:37] So just be sure that you're adding more color variation than you think and more contrast than you think that's generally what I learned is that the contrast especially if you're using subsurface scattering the colors tend to lose some of the contrast so the texture map itself will need to be a little more contrasty.
[56:00] Then you think and then of course we really want to focus on telling a story through the textures and through the sculpt as well but this video is focused on textures so focusing on telling that story through the textures and having the textures support the story of the model.
[56:18] And then of course just taking it into a render engine getting feedback getting feedback from other people as well to see what works maybe you know this color doesn't work for this creature and if we you get feedback from someone maybe you know a purple or blue creature might or blue color skin tone might work better but for this creature this is what we ended up going with.
[56:40] And that is the whole process of how to texture creatures for real time or games.
[56:48] So yeah guys hope you found this video helpful and I will see you in the next one.



---

## Captured Frames

- [2:52] tutorials/frames/texturing-creatures-for-games-in-substance-painter-full-process/frame_000.jpg
- [5:15] tutorials/frames/texturing-creatures-for-games-in-substance-painter-full-process/frame_001.jpg
- [8:03] tutorials/frames/texturing-creatures-for-games-in-substance-painter-full-process/frame_002.jpg
- [11:34] tutorials/frames/texturing-creatures-for-games-in-substance-painter-full-process/frame_003.jpg
- [14:01] tutorials/frames/texturing-creatures-for-games-in-substance-painter-full-process/frame_004.jpg
- [19:31] tutorials/frames/texturing-creatures-for-games-in-substance-painter-full-process/frame_005.jpg
- [23:01] tutorials/frames/texturing-creatures-for-games-in-substance-painter-full-process/frame_006.jpg
- [30:16] tutorials/frames/texturing-creatures-for-games-in-substance-painter-full-process/frame_007.jpg
- [34:04] tutorials/frames/texturing-creatures-for-games-in-substance-painter-full-process/frame_008.jpg
- [52:46] tutorials/frames/texturing-creatures-for-games-in-substance-painter-full-process/frame_009.jpg

---

## Structured Notes

### Core Technique
Full real-time/game-ready creature texturing pipeline built around one repeated principle: bake every useful mesh map from a high-detail ZBrush sculpt (curvature, AO, thickness, normal), stack those baked maps as color-driving utility layers first, then build up organic skin-tone variation through hand-painted color-temperature layers (yellow/blue/red/green) refined with tri-planar procedural breakup, validated throughout via an export-to-Blender feedback loop.

### Summary
A from-scratch, single continuous session (no chapter markers) creature-texturing walkthrough on a two-texture-set (body + mouth) game character. Opens with the video's central thesis — "you cannot out-texture a bad model," texturing quality is capped by sculpt quality — then covers the full bake setup (Automatic vs. Distance-Based cage, recommends Automatic despite its "experimental" label because it produces cleaner bakes even when the cage preview looks odd; a two-pass bake strategy: 1K for maps Painter just needs internally, 4K for the detail-carrying maps). Texturing proper starts from a flat pale/ghoulish base color and layers baked Curvature, Ambient Occlusion, and Thickness maps (each inverted via a Levels filter and tinted) as color-driving utility layers before any hand-painting begins — Thickness specifically tinted red and blended via Multiply to redistribute blood-flow color to hands/feet/head. The bulk of the video is hand-painted anatomical color-temperature layering: yellow where bone sits close to the skin (Screen blend, kept patchy/broken up rather than solid), blue for cool/bruised/cavity areas (Multiply, doubling as a hand-painted secondary AO/curvature pass), red for blood-flow and wound areas (Overlay/Screen/Soft Light), and an optional green pass for added organic color variation and bruising — all explicitly tied to storytelling (scars, burns, muscle striations reinforcing the sculpted narrative of a creature that's "been in a lot of fights"). Two tri-planar-projected procedural grunge "breakup" layers (contrasting orange and purple, Soft Light / Multiply) are added to integrate all the hand-painted color into one cohesive surface, followed by hand-painted vein detail using a dedicated vein alpha brush (used sparingly). A second curvature pass is layered on top later for extra crunch. The workflow is validated twice via a Color+Normal texture export into Blender/EEVEE with a 3-point light rig and Subsurface Scattering added on the shader side (normal map explicitly set to DirectX space) — first pass reveals over-saturated yellow/hands, prompting a return to Painter to tone those down and rebalance; ends with additional nail color, reordering the red layer above curvature for more pop, and a final Blender render with a rig/pose for a "menacing" presentation shot.

### Key Steps
1. **Model/sculpt quality gates texturing quality:** stated up front as the video's core principle — a well-built primary/secondary/tertiary sculpt (skin pores, scaly detail readable by eye) is what makes fast, high-quality texturing possible; texturing cannot fix a weak sculpt.
2. **Export both a low-poly (bake target) and a decimated high-poly** (~800k points via Decimation Master, noted as low for a portfolio piece but fine for demonstration) mesh pair before baking.
3. **Bake setup — cage choice:** tested `Distance Based` cage (tune max frontal distance as low as possible without red ray-miss artifacts) vs. the `Automatic` cage (marked "experimental" in the UI) — recommends Automatic as the default despite visually messy cage previews, because in practice it produced a cleaner bake with fewer artifacts; explicitly says to test both per-project.
4. **Two-pass bake resolution strategy:** first bake `Normal`, `World Space Normal`, `ID`, `Ambient Occlusion`, `Curvature`, `Position`, and `Thickness` all at 1K just so Painter has the data it needs internally; then re-bake at 4K keeping only `Curvature`, `Ambient Occlusion`, and `Normal` (the maps that actually carry fine sculpted detail like skin pores) to save bake time on maps that don't need the extra resolution.
5. **Verify the bake by orbiting/relighting before painting** — check for red/black artifact patches; also swap the default viewport environment away from the greenish-tinted default panorama to `Studio Tomoko` for neutral lighting during color work.
6. **Set the base document/texture resolution to 4K** before painting so fine detail is visible while working, and lay down a flat, deliberately desaturated/pale base color plus a flat 0.5 base Roughness as the starting fill.
7. **Layer baked Curvature first, as a "staple" utility layer:** new Fill Layer + black mask + fill sourced from the baked Curvature map, tinted dark, then run through a `Levels` filter with `Invert` checked so crevices read dark rather than light — described as functioning like a cavity map and "crunching" all the sculpted pore/detail data directly into the color map (compared explicitly to a Photoshop high-pass filter).
8. **Layer baked Ambient Occlusion the same way** (Fill Layer, black mask, fill = baked AO map, darker tint, Levels+Invert), opacity pulled back until it reads as a subtle occlusion tint rather than an overpowering shadow pass.
9. **Layer baked Thickness as a blood-flow color-distribution map:** same Fill-Layer-with-Levels-Invert recipe, tinted red, blend mode set to `Multiply` — because thinner geometry (hands, feet, mouth) reads redder on a thickness bake, this automatically redistributes warm color toward blood-flow-heavy extremities without hand-painting; opacity and hue tuned to taste.
10. **Hand-paint yellow "bone proximity" tones:** new black-masked Paint Layer, yellow color, using a broken-up brush (`Dirt 2` alpha, size-pressure off / flow-pressure on, symmetry enabled) to paint only where bone sits close to the skin (sternum, ribs, skull, elbows/ulna, knuckles) — kept deliberately patchy/incomplete rather than solid fill, since solid coverage kills the underlying color breakup; blend mode set to `Screen` and opacity pulled down so it reads as bone showing through rather than a yellow overlay.
11. **Tie every color-layer placement decision back to character storytelling:** explicitly frames yellow/blue/red placement, scars, wounds, and asymmetry as narrative tools ("a lot of the storytelling... is done through the sculpting... but you want the texturing to support the storytelling") — e.g. red stretched spine tips reading as pain, asymmetrical wounds reading as more believable/alive than symmetrical ones.
12. **Hand-paint blue "cool/bruised/cavity" tones:** new black-masked Paint Layer, blue, functioning as a second hand-painted cavity/AO pass in crevices and bruise-prone areas; blend mode `Multiply` for deep blue-purple crevice pop; explicitly chosen as blue-tinted rather than pure black specifically to keep the model "saturated... alive," since pure black shading reads dead.
13. **Hand-paint red "blood flow" tones:** new black-masked Paint Layer, bright red, concentrated on head/hands/wounds/veins-near-surface areas and any burn/scar storytelling zones (symmetry toggled off for asymmetrical damage like a one-sided facial burn); blend mode tested across `Overlay`, `Screen`, and `Soft Light` (creator's usual default is Soft Light) — explicitly framed as blend-mode choice varying per model, so testing is expected.
14. **Optional green layer for extra organic variation:** duplicate one of the existing tone layers, recolor to green, apply sparingly/patchily as added bruising or general organic color variance — explicitly recommended as safe to push further than expected on creatures specifically (works for non-green base skin tones too, "still be those subtle yellow, blue and red tones... but there will still be" the base palette underneath).
15. **Integrate all hand-painted tones with tri-planar procedural "breakup" layers:** new Fill Layer + black mask + fill sourced from a procedural grunge map (`Grunge Cobweb`, later duplicated onto `Burnt Concrete`), `Projection` set to `Triplanar` (avoids UV-stretch artifacts on organic geometry), tinted orange on one layer and purple on a duplicate, blend modes `Soft Light` and `Multiply` respectively — described as the step that pulls all the previously separate color passes together into one integrated-looking surface; tiling size adjusted to taste.
16. **Trace veins with a dedicated alpha/brush** over the blue-tone layer specifically, used sparingly per the creator's own warning ("don't overuse this too much") since overuse reads as gimmicky rather than adding the intended "illusion of blood flow... helps things feel alive."
17. **Second curvature pass added later for extra micro-detail "crunch":** a second Curvature-sourced Fill Layer added near the end of the session, deliberately over-exaggerated (levels crunched further than looks correct) with the explicit reasoning that pushing an effect further than expected and then dialing back tends to land closer to correct than being conservative from the start.
18. **Validate via export-to-Blender feedback loop (used twice):** export Color + Normal only (4K) via the Export panel, re-import into Blender's Shader Editor, set the Normal map's color space to Non-Color and the normal map node to `DirectX` (matching Painter's default normal-map handedness), light with a simple 3-point rig, and add Subsurface Scattering on the shader for a closer approximation of final look — explicitly framed as necessary because Painter's own viewport has no SSS shader, so "you don't know exactly how your textures are going to look" without this round-trip.
19. **Act on render feedback, then re-export and re-check:** first Blender pass revealed the yellow tones and hand saturation were too strong; returned to Painter to tone those down, added more yellow elsewhere for balance, adjusted thickness-layer strength on the hands, then re-exported and re-validated in Blender before final polish (added a separate nail-color layer, reordered the red wound-emphasis layer above curvature so wounds read more clearly, added a rig+pose in Blender for a presentation shot).

### Layers / Tools / Settings
- **Bake maps used:** `Normal`, `World Space Normal`, `ID`, `Ambient Occlusion`, `Curvature`, `Position`, `Thickness` (1K internal pass) -> `Curvature`, `Ambient Occlusion`, `Normal` (4K detail pass)
- **Bake cage options compared:** `Distance Based` (manual max frontal distance tuning) vs. `Automatic` (experimental, creator's recommended default)
- **Utility-map color-driving layers (each: Fill Layer + black mask + fill = baked map + `Levels` filter with Invert):** Curvature (dark tint, "cavity map" behavior), Ambient Occlusion (dark tint, subtle opacity), Thickness (red tint, `Multiply` blend — blood-flow redistribution)
- **Hand-painted anatomical tone layers (Paint Layer + black mask, symmetry toggled per-need):** Yellow/bone (`Dirt 2` brush alpha, size-pressure off, flow-pressure on, `Screen` blend), Blue/cool-cavity (`Multiply` blend), Red/blood-flow (`Overlay`/`Screen`/`Soft Light` blend, creator favors Soft Light), Green/extra-variation (duplicated + recolored tone layer)
- **Procedural breakup layers:** `Grunge Cobweb` and `Burnt Concrete` procedural fills, `Projection` set to `Triplanar`, orange (`Soft Light`) and purple (`Multiply`) tints
- **Detail brush:** dedicated vein alpha/brush for hand-traced vein tracery over the blue layer
- **Export/validation loop:** Export panel (Color + Normal, 4K) -> Blender Shader Editor, Normal texture set to `Non-Color` color space, Normal Map node set to `DirectX`, 3-point light rig, EEVEE real-time viewport, Subsurface Scattering added on the shader side
- **Base fill:** flat pale/desaturated Base Color + flat 0.5 Roughness starting point

### Difficulty
Advanced — the individual layer operations (Fill Layer + mask + Levels invert, Paint Layer, blend-mode stacking) are each simple, but the tutorial assumes comfort with baking setup, PBR/color-temperature theory for organic skin, and render-engine round-tripping (Blender/EEVEE, SSS, normal-map color-space handling) to get a production-quality result; paced quickly with minimal dwelling on individual UI clicks.

### App & Version
Not stated explicitly on screen. Baking uses the modern `MESH MAP BAKERS` / `Common Settings` panel layout with `Automatic` and `Distance Based` cage options and per-map checkboxes (Normal, World Space Normal, Ambient Occlusion, Curvature, Position, Thickness) — consistent with the post-8.3 Baking Mode era generally seen across this skill's other ingested tutorials, but nothing in-frame pins an exact version.

### Tags
layers, fill-layer, paint-layer, masks, baking, mesh-maps, curvature, ambient-occlusion, thickness, world-space-normal, position-map, id-map, blend-mode, procedural, tri-planar, basecolor, roughness, normal-map, color-management, texture-set, export, advanced

---

## Related Tutorials
- [How to TEXTURE in SUBSTANCE PAINTER | Creature TEXTURING](how-to-texture-in-substance-painter-creature-texturing.md) — different creator (Jared Chavez), also a from-scratch original-creature texturing process video; shares the sub-dermal/anatomical color-blocking philosophy (yellow/blue/purple zone logic there vs. yellow/blue/red/green color-temperature logic here) and the render-engine validation loop (Unreal there, Blender here).
- [REALISTIC CREATURES: HAND PAINTED TEXTURES in SUSTANCE PAINTER](realistic-creatures-hand-painted-textures-in-sustance-painter.md) — different creator (Jared Chavez); shares the anatomy-driven color-zone blocking approach and large-to-small detail hierarchy for creature skin.
- [How to make SKIN TEXTURES in Substance Painter](how-to-make-skin-textures-in-substance-painter.md) — different creator (J Hill); shares the baked-thickness-map-drives-blood-flow-color technique and the iterate-export-render validation loop (Marmoset there, Blender here).
