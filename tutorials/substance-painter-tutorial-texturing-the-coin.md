---
title: Substance Painter Tutorial: Texturing the Coin
source: YouTube
url: https://www.youtube.com/watch?v=7kV4Q4UBvl4
author: Abe Leal 3D
ingested: 2026-08-13
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/substance-painter-tutorial-texturing-the-coin/
frame_count: 0
frame_status: pending-selection
---

# Substance Painter Tutorial: Texturing the Coin

**Source:** [YouTube](https://www.youtube.com/watch?v=7kV4Q4UBvl4)
**Author:** Abe Leal 3D
**Duration:** 29m7s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py substance-painter-tutorial-texturing-the-coin <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hey guys, welcome to another video in this channel. Today I'm going to be showing you
[0:03] how to do this coin right here. This is a game-ready asset that you could import right
[0:07] into Unreal and I'm going to be showing you not only how to do one, but four different
[0:12] coins with variations in texture so we have a lot of options. Now we're going to be covering
[0:16] retopology, UVs and texturing. So that's it, let's go. Let's start working on this coin
[0:21] right here. Now the first thing I'm going to do is, as you can see, we have a very like
[0:25] weird line going around this element and I definitely want to clean it up. So there's
[0:30] a bunch of ways in which we can do this. I'm just going to use trim dynamic to be honest
[0:34] and with trim dynamic, I'm literally going to push that line towards the character so
[0:38] that we're kind of like bridging the gap pretty much like that. Same thing over here, just
[0:45] very, very softly. It's supposed to be an old coin. So even if things are slightly off,
[0:49] that's fine. We're dynamesh and again, keep pushing those elements because they could cause
[0:54] a little bit of an issue. Another good option to get rid of those elements is with inflate.
[0:59] You can like very lightly inflate the polygons on those areas. And that's also going to like
[1:04] collapse all of the polygons into one point. And it's going to be a little bit easier to
[1:09] work with. Then with clay buildup, we can like bring back a little bit of the details
[1:15] of the character if we need to. There we go. So just a basic thing. I mean, this coin is
[1:21] probably going to be seen at this distance. There are some gains you probably see them
[1:24] when you go into the inventory and you can analyze the object, which is very cool. But
[1:27] what usually happens in those games is you have different levels of detail, LODs that
[1:31] are called. So when you see them very close up, the resolution and the textures are going
[1:35] to be higher. And when they're far away, you're going to see them really, really small and
[1:38] really simple. So the first thing I need to do is I need to clone this so that we can
[1:42] work on a different element. And I'm going to go to C plugin, decimation master, I'm going
[1:46] to decimate it to 250k is usually a good number for for props like this, it holds a
[1:51] lot of the detail and allows us to work very nicely. And the question that everyone's going
[1:55] to be asking is, do we need to do manual retopology for this thing? And the answer is if you want
[2:01] the best possible result, then yes. But don't worry, stay tuned right now because I'm going
[2:06] to show you a very cool process that we can do inside of Maya to to work very nicely.
[2:12] So let's go here. I'm going to go export. And I'm going to export this to the desktop
[2:17] for now, I'm going to call this coin underscore high, this is going to be an fbx export. And
[2:22] there we go. And let's open Maya real quick. Very well. So we are here inside of Maya,
[2:28] and I'm just going to go file import and going to the desktop, we can import our coin high.
[2:32] The first thing one of the most important things is we should try to have this in the
[2:36] real world scale because a lot of the things in the 3d world work nicely in real world
[2:40] scale. So I'm imagining that it's going to be like an inch so like 3.5 centimeters or
[2:45] something like that. So it's pretty much already there. So I'm just going to grab this element
[2:49] right here. I'm going to change the radius to 3.5 centimeters. Actually, that's the height.
[2:55] So this one has changed to 3.5. I think that's a good size. And if we need to scale it down,
[2:59] it's usually a little bit easier to scale things down than it is to scale them up. Let's
[3:04] rotate this 90 degrees and I'm going to scale this to the top view. There we go. Something
[3:09] like that. Perfect. Now here I need to decide whether I want to texture the coin like up
[3:14] and down or like completely flat. I actually think completely flat like this is going to
[3:18] be a little bit better. I'm going to show you some generators later on that are going
[3:21] to be useful in this position. So let's freeze the transformations. It's very important because
[3:26] this is going to be our new size and we're going to go to front view and we need to start
[3:29] creating the low poly mesh. So here's the trick. I'm going to go to mesh tools and I'm
[3:33] going to use a create polygon tool and I'm going to create a big polygon that goes around
[3:39] the whole like silhouette of the coin. Remember that a resolution or when we're doing a retopology,
[3:46] one of the most important things is to capture the silhouette of the object as close as we
[3:51] can as close as possible. Let's go one right there and one more right there. As you can
[3:56] see, all of these points, they very closely close the coin. I can still see a couple
[4:02] of points that could be like further improved and that closer we are to the silhouette,
[4:07] better. It's going to give us the cleanest effect over the whole thing. For instance,
[4:12] here I can definitely feel or see that we are missing one. So I'm going to go with my
[4:16] cut tool. I'm just going to add one point right there. Grab that one, just push it up
[4:21] a little bit again so that we get a better distribution. So if we take a look at that
[4:26] polygon, you're going to see that this is a very ugly end on and if you've been like
[4:30] learning 3D, you probably heard that you need to make sure that you don't have any
[4:34] angons on your character and that's like completely, completely real. However, we can
[4:38] actually use angons to our advantage. So for instance, right here, if I just say mesh display
[4:43] and reverse and I go to the top view and I extrude this control E forward right to about
[4:50] there, which is where the coin border ends. What's going to happen as you can see right now is all
[4:55] of those points are now like a very clean nice silhouette like a cylinder. It's like if we've
[5:00] had created a cylinder and move the points around, but it's a lot easier to do it this way.
[5:04] I'm going to grab the back part right here. I'm going to say control E. I'm also going to push
[5:08] this back right here. There we go. So that's pretty much it. The next thing that we need to do is we
[5:14] need to think about this like chain effect, for instance, here on the back, and we need to ask
[5:19] ourselves the question, are we like really like how many coins are we going to have on the game?
[5:23] Right? If there's like a treasure horde and you're going to have like millions of coins or whatever,
[5:28] then probably something like this is more than enough. I might even like remove this edge right
[5:32] here so that we only have as you can see 64 triangles on our element because these two faces,
[5:38] if we just go mesh and triangulate, that's a perfectly fine effect. Actually, in this case,
[5:43] I would suggest going edit mesh and poke. It's going to give you a nicer cleaner effect. As you
[5:48] can see, 68 triangles. That's all we have for one single coin. And when you see it from afar in the
[5:53] game, again, that's perfectly, perfectly bad. But I want to go a little bit higher because I want to
[5:58] have a little bit more like resolution to our whole thing. So if we take a look at the coin here,
[6:02] you're going to see that he has like several high points, especially like the face on this
[6:06] side. And on this side, it's pretty much just this area. So we're going to grab this face,
[6:10] I'm going to press Ctrl E, and I'm going to offset this so that we go close to the chain right around
[6:14] there. And then I'm going to Ctrl E, push it up and offset a little bit. So it's kind of like a
[6:21] little ramp that we're using to capture the high point of where the chain is. And that's going to
[6:25] give us a little bit of a better shading. It's not going to be perfect, but at least the coin is
[6:30] not going to look perfectly or completely flat. So we're going to have a little bit of a off effect.
[6:34] I know some people will be like, Oh, this is a waste of polygons. And yeah, maybe it's not the best
[6:38] like a use of them. But again, it's a good way to capture the sort of silhouette. Same thing for
[6:43] the axe, we could do another Ctrl E right here, another offset. When this case, I'm just going to
[6:47] use R to scale. I'm just going to scale this face in like this. And then we can scale this up,
[6:53] just push it up a little bit. And that way, as you can see, we create a little bit of a rise
[6:58] effect on this thing. So that's going to give us, you know, not in every single part of the coin,
[7:04] but especially when you see the coin at us itself, like right here, let's go mesh display, soft
[7:10] and edge, there's going to be a little bit of something right like that little effect right
[7:13] there is going to it could help maybe this last one might not have as much to be honest. So I'm
[7:18] just going to leave it at this point. I think the chain is good, but the axe is not really necessary.
[7:22] So now what I want to do here is I want to make sure that we have the
[7:27] the back part of the coin ready. So this face right here, I'm just going to say edit mesh
[7:32] and poke. For those of you that are like super optimizers and you want to have like the best
[7:36] possible resolution, yes, we can go to some of the triangles, like skip one and select the next one
[7:42] like this. And just collapse them, we can collapse them in that's going to have like
[7:46] reduced the amount, it's a flat area, it's not going to affect anything, we're still capturing
[7:50] the high point on that area. And again, shouldn't be that much of a problem. Again, we can say mesh
[7:54] display and soft and edge and that's it. We got a nice simple coin. Now on this one, this one's a
[7:59] little bit trickier. And this is where I would actually suggest using quadra. So what I'm going
[8:03] to do here is I'm going to grab the coin, I am going to give myself a little bit of a border
[8:08] so control E and just offset a little bit. Not too much right around there, push this up a little
[8:15] bit so we're close to like the chain and things, like right around there. There we go. And then
[8:22] I'm going to delete this face, grab the coin, make this a life surface, grab my low poly and go
[8:27] into quadra mode. And what I want to do here is I want to start like creating a profile for the
[8:33] main phase of pyros right here, which is my character. I'm actually, if you guys are not aware,
[8:40] we did a Baldur's Gate playthrough or intro video. So if you want to check it out, it's on the channel
[8:45] as well. And the character that we created is named Pyros after one of my favorite characters that
[8:51] I've done in the last couple of years. So there we go. As you can see, I'm going to try to capture
[8:57] this round shape because you can see there's a little bit of a high point right there.
[9:01] And if we just keep that or if we just add that high point, we might get a little bit of a better
[9:06] effect. I don't need to capture every single detail everywhere else, like just keep it really simple.
[9:13] But I do recommend like capturing this little edge right here. I know it sounds like a or it might
[9:19] appear like a little bit of a waste of polygons because it's a very thin like element. But again,
[9:25] if we if we do it, if we do capture this, this thing right here, here's a trick for retopology,
[9:31] I'm going to use a tap. If you use tab, you can just extrude one line. And that's a little bit
[9:36] easier for Maya to to follow. So by doing this, I am going to be able to catch a little bit of a
[9:42] shadow on the on the high polar and the low poly rather. And that's going to give me a little
[9:46] bit more depth in general. So even though yes, this is not as optimized as it can be, like the
[9:51] most optimized thing is the little first like circle that I show you, this is still a perfectly
[9:54] valid way. And this is a discussion that I have frequently, especially in online forums, like
[9:59] when I post works or people are commenting about like portfolio pieces. So I was like, oh, the
[10:04] topology is not perfect. And as Alex Alba is the founder of No Man used to say, topology is a guide,
[10:10] it's like a like a set of instructions, but it doesn't need to be or it doesn't have to be this
[10:14] like a cult where if you don't do proper topology, the topology police is going to come to your door
[10:19] and they're going to be like, oh, you're now banned from being an artist because you did not follow
[10:22] proper topology. That's never going to happen. Like it's just not what's going to happen. For
[10:26] instance, here's a small little trick to to keep topology a little bit cleaner. It's just
[10:30] at a triangle right there. And by doing that, and going back to quadro, I'm going to be able to fill
[10:36] those elements right there. From here, just big, big freaking squares right there, one.
[10:41] And then let's do another one right there, another one right there triangle right there,
[10:45] that's fine. It's a flat area. No need to worry about it. So I do feel like students,
[10:50] especially like newer students, and we as a teachers, we tend to like, inflict or or create
[10:56] that fear in people of telling them, hey, you need to have like perfect topology, if not,
[11:01] like no one's going to hire you. It's not perfect topology is just good topology. Okay.
[11:06] So there's always ways to to make things even more perfect. But as long as it works, then you're
[11:10] going to be fine. So that's it. As you can see, we now have this thing right here, which is our coin,
[11:15] I'm just going to say mesh a display and soft and edge. Now for this one in particular, we need to
[11:21] do UVs. That's why I personally prefer to have one extra line on the center of this line right here.
[11:27] Some might be like, Hey, that's like 20 extra polygons or something. Yes, it is. But it also
[11:31] allows us to do a very clean cut down the middle. That's not going to be as visible. We could also
[11:35] do it here on the on the side. But again, I personally think that that's a good point to do so.
[11:40] So I'm going to select this edge right here. Because otherwise, when you do the cut on the
[11:43] on the lines on the very border, when you do the bakes, some things you get like very weird bakes
[11:47] and I personally think it looks a little bit worse. So I'm going to go UV. And well, first of all,
[11:53] we're going to do UV, delete UVs. And we're going to say UV. And we're going to do a camera based
[12:01] projection. And once we do that, we just go UV, 3d cut, and we cut down the middle. Like,
[12:06] this is probably the most or the simplest UV you can do. We just control you to unfold,
[12:11] control L. And there we go. We get this one. Now, since we have enough space, I can see we have
[12:17] enough space right here. And there's no way we can cut this to get more space. Or if we cut it,
[12:20] it's just going to be a waste of cuts. One thing that we could do though, is we could duplicate
[12:26] this coin twice. And we could have two, three, four different coins that are going to give us
[12:31] a slightly different results, like slightly different textures. And that way, when you see all
[12:34] of the coins in the same place, they're not all good, they're not going to be all the same,
[12:37] they're going to be the same in the geometry. But with the textures, we can hide certain things,
[12:41] we can make some of them a little bit more rusted, a little bit less rusted and stuff like that.
[12:44] And that's a perfectly valid way to do so. So the only thing with that is if we're going to be
[12:48] doing bakes, we need to do the bakes for all of the coins. And that means that we're going to
[12:52] have to duplicate this thing a couple more times. Or yeah, now we need to do that. Because otherwise,
[12:57] the normal maps are not going to work. So I'm going to remove this thing right here,
[13:00] grab both elements, I'm going to control D, duplicate both of them, just move them to the side.
[13:06] Make sure you move them enough apart so that ambient occlusion from one of the coins is not
[13:09] going to affect the other one. And then do the same thing right here. Now I know this is one
[13:14] million triangles now with high polys, but usually, again, nowadays, triangles are not that much of
[13:18] an issue. So this is going to give us a nice effect. What I'm going to do though, is I'm going to
[13:22] grab all of the high polys, and I'm going to combine them into a single object. The history
[13:27] for instance, mentioned all that all the stuff. There we go. And I'm going to grab all of the
[13:32] low polys and combine them into a single object as well. And again, delete everything. Later on,
[13:36] we can separate the low polys and have them as individual coins. That's fine. I'm going to UV,
[13:40] UV editor, and now we just go control L to lay them out. And as you can see, now we have four
[13:45] coins. So we're going to have more textures. And again, we can do a little bit more variation on
[13:49] each of these elements. I'm going to grab the low poly coin, I'm going to call this coin underscore
[13:55] low. I'm going to grab this one, I'm going to call this coin underscore high. And that's it.
[14:02] Now before we continue with the substance bar, just a little commercial here. If you are interested
[14:06] in doing this workflow, we're very similar workflow, but for a huge, huge, like very cool
[14:11] acts right here, a game prop with all of the specifications that we go through modeling,
[14:16] sculpting UVs and stuff, this course is available right now, you can check it in the description
[14:19] is in Udemy, it's usually in like a good discount. So we don't have discounts, but Udemy usually has
[14:24] them. So make sure to check it out if you're interested in learning the full process for a
[14:28] more complex prop. Let's continue. So now that we have this coins, we need to export them, of course,
[14:33] I'm going to grab the lows, I'm going to say, did I rename them wrongly? So this one's going to be
[14:38] called low. And this one's going to be called high. There we go. So we're going to export the coin
[14:46] lows file, export selection. Let's go to the desktop for now. fpx is usually good. I prefer
[14:53] xpx to OBJ, because it works a little bit better with most softwares, OBJ loses a lot of information.
[14:59] I'm just going to call this coins or coins like that. And then the high, we're going to call them
[15:03] coin high, which is the one that we have right here. And we hit yes. Now let's open Substance Painter.
[15:09] There we go. So we're opening Substance Painter and we're covering three softwares in one little
[15:13] video. So if you're not subscribing, you think this is valuable, please, please help us with the
[15:16] subscription. It helps the channel grow. And it allows me to keep this, keep doing this for you,
[15:20] my friends. So we're going to go here select, we're going to select our coins with S multiple,
[15:25] and usually a 2k map for this assets is more than enough. We're going to keep it direct x,
[15:29] because I do want to show you how this coins could look inside of Unreal, which is a good
[15:33] stuff, or a good thing that we can do. So we're going to do direct x right there. And that's
[15:38] pretty much it. Just hit OK. What we should see right here are our low poly versions of the coins.
[15:43] Now I'm going to go to this little crosshunt option right here, which is the baker,
[15:47] we're going to set this to 248. And on the high definition meshes, we're just going to load in
[15:51] our coins. What this do, I've explained the baking process a lot of times, but I'm going to do it
[15:56] again. What this do is it projects lines outside and inside of the object, and it looks for information
[16:01] on the high poly, which we're loading right here. And as you can see right now, we're not getting
[16:05] any error. So the cage that we're generating should be more than enough to catch pretty much all of
[16:09] the details. And again, it's important that they're like separated enough, because otherwise the ambient
[16:13] occlusion could contaminate them. And you could get like, we're shadows on the sides. But in this
[16:17] case, I don't think that's going to happen. We really don't need to do the matching, but I am
[16:21] going to use this anti aliasing by four so that we get a softer effect on the normal map. And we
[16:25] just bake. This is a GPU powered. So as you can see, it's very, very fast, and we can get a very
[16:30] nice result with not a lot of effort. And we get all of the maps that we need to work inside of
[16:35] inside of substance, we get the normal map, of course, we get the cavity map, we get the ambient
[16:40] occlusion map. So that's it. This is the coin that we will be seeing in the game. And it's very,
[16:45] very low on polygons. And look at how much detail we have. So this is what we're looking for. Now,
[16:50] let's very quickly look for some old coins, and see how they look right like what kind of coin do
[16:56] we want. I think I'm going to go for like the traditional, like gold, sort of like bronze coin
[17:02] that we have. So this sort of like effect right here. So it's like this gold tarnished effect.
[17:07] Interesting. Oh, this one's perfect. This is like this is exactly the type of texture that I want.
[17:12] One interesting thing, pure metals or what we call like the fancy metals like silver,
[17:17] gold, bronze, they don't rust in a traditional way. And I don't know the chemicals or the
[17:24] reasons why that is some of you might want to leave me the information down here on the on the
[17:28] description. But I do know that the colors that they get is not really rust is like a tarnished
[17:32] sort of effect. So for instance, silver, silver creates this very interesting tarnish,
[17:40] where you get this sort of like dark color, but again, it's not rust, it's tarnish. So it's a lot
[17:45] easier to clean than rust. So yeah, so this one right here, this is perfect. I'm just going to
[17:50] copy this image. And I'm going to open pure riff, pure riff for those of you that don't know it's
[17:55] an amazing software to get your like reference. So we're going to use this one as a reference and
[18:00] reference is king whenever we're doing texturing and pretty much anything in the three the world.
[18:04] So if you're not using reference, you I can say, like with confidence there that you might not be a
[18:09] great artist because every great artist should be using reference. We got this one right here with
[18:14] this stylized a raw metal or something, I'm going to drop it into my coins. And the first thing I
[18:20] want to do is I want to match the roughness and the color of this coin right here. Unfortunately,
[18:24] I don't think this thing Oh, we can perfect. So we could just sample this thing. And I'm just going
[18:28] to go for like the most like basic color right there, which is that one, that seems to be like
[18:33] the base color. And in the roughness, I definitely need to increase the roughness quite a bit.
[18:38] So it's quite quite rough, we're going to have some like, like shiny areas, but the base metal
[18:42] should be quite, quite tarnished, quite, quite dark. Now, I know I just said that metal or this
[18:47] metal does not rust, but I'm going to use the metal rust right here to generate the same color,
[18:52] because we can go to the rust itself, pick the color and grab this really greenish,
[18:56] Hueyish effect. Look at that. Oh, beautiful. And we can use this to generate the rust on our coins.
[19:02] So I'm going to say add a black mask. And we're going to add on this black mass, of course,
[19:06] a generator that's going to be a dirt generator. And that way, as you can see, we're going to get
[19:11] the very, very nice rust in all of our coins. So what I see on the rust is that's not it's a
[19:17] little bit more contrasty. So I'm going to push the contrast contrast contrast a little bit up,
[19:22] I'm going to increase the intensity a little bit more as well. And I think the color is a little
[19:26] bit too dark. So I'm going to go back here to the color, just bring the color a little bit cleaner
[19:30] to like a blueish hue. There we go. And I'm actually going to blur it a little bit more. So I'm
[19:35] going to the dirt contrast, I'm going to bring it down. So that's a little bit more blurred.
[19:39] I don't like the fact that this is adding a little bit of height information. So I'm going to
[19:42] remove the height information. Actually, I kind of like it. Kind of like it, but it's a little bit
[19:47] too much. So there's two ways you can change the height, you can go to technical parameters
[19:51] and bring the height position down. Okay, so I'm going to keep it like point for something like that.
[19:59] Or you can go to the height information over here and just reduce the intensity, both of those
[20:02] methods work similarly. Now the problem with this, and you can notice that when we look at all of
[20:07] the coins, is that the rust on all of the coins is exactly the same, which is exactly what we
[20:11] wanted to avoid when we were doing this exercise, right? Like we decided to have four coins, so
[20:16] that we can have variation between them. So I'm going to add here a very traditional layer that
[20:21] I have, which is a fill layer. I'm going to add a fill layer. And I'm going to add there are, I
[20:27] believe, some rust elements, I actually have some mask right here like this rust leaking.
[20:31] This grunge mask. Let's use this grunge rust define. And what I'm going to do is I'm going to increase
[20:40] the balance, increase the contrast, and increase the tiling. So we get this like spotty effect.
[20:49] Let's increase the contrast even more. So what I want to do with this mask is I'm going to multiply
[20:54] this against the coins. And as you can see now, every single coin has a slightly different sort
[21:00] of like rust effect throughout the whole thing. And we can play again with the balance here. And
[21:04] you can see how they all change slightly different. So this grunge mask is really, really important
[21:09] because it's really going to break down the way my coins look. So they should look similar because
[21:13] they're supposed to be the same value, right? But the texture is going to allow us to generate a
[21:18] very nice variation. Now I see this dark spots right there, very nice dark spots. And I'm going
[21:23] to use another rust layer here for those dark spots. But what I'm going to do is I'm only going to be
[21:28] using the color. Oh, here's the tricks I want suggested on the comments. So if I want to turn
[21:32] everything off except for the color, I press alt and click, and that's going to turn everything
[21:35] off except for the color. Great tip, by the way, thank you. I don't have your name right now,
[21:38] my friend. But if you're watching this video, thank you very much because I've been using substance
[21:42] for eight years, and I didn't know that. So black mask right click, and I'm going to use a fill layer
[21:47] here. And I want to use again, we can even use my rust generally, there we go, that one looks
[21:53] pretty sick. And what we can do with this one, first of all, I'm going to invert it. So I'm going
[21:57] to add a filter where I levels, I'm going to invert the element, there we go. I'm going to play a
[22:02] little bit with the with the values of this thing. And then I'm just going to change this to something
[22:06] like an overlay, and reduce the intensity quite a bit. So what that's going to do, as you can see,
[22:11] it's just going to dirty up my coins in such a way that they get some interesting variations
[22:16] undertones, without giving me a like super obvious effect kind of looks like blood. So I actually
[22:22] like the sort of effect that we're getting right there. So yeah, that's the that will be my let's
[22:29] call it the dirt pass of my of my coins. Now we're going to go for the like polish pass of the elements.
[22:35] And what I want to do is I want to add a metal edge where of course it's going to like bring the
[22:39] shine out of our coins, and maybe some scratches or something like that. So for the metal edge where
[22:44] I'm going to go back here, I'm going to bring again my stylized gold right here. I actually think
[22:49] that's a very nice color. It's not super saturated, but it gives us a nice, like clean brightness.
[22:55] I'm going to add a black mask, and we're going to add a generator. This is going to be of course,
[22:59] the metal edge where generator. And as you can see, that's going to bring out the high points of
[23:04] the coins that the points that you will normally rub against your fingers, against your pants,
[23:08] in your wallet, or on your coin pouch, like that's the sort of stuff that you might find
[23:12] when you're dealing with this guys. Now I am going to bring the wear level up, and the wear
[23:17] contrast down because I want to really, really soften this up. Another way in which we can soften
[23:22] this is we can right click and add a filter. And by adding a blur filter right here, as you can see
[23:27] that's going to give us a slightly blurred effect for the whole thing. I usually like to change this
[23:32] to linear dodge so that it like punches the colors of my coins. And here I'm definitely going to
[23:37] bring the intensity down. So this is like normal effect, like this is the normal coin that we have.
[23:42] And if we start adding a little bit of that effect, we can bring this hardness of this
[23:47] sort of like clean gold effect up. And as you can see, that's going to give us a very, very nice
[23:52] effect. Now I still think it's a little bit too much. So I'm going to go to the color and I'm going
[23:56] to bring the color down a little bit. You said it's not like overwhelming and like burning the
[24:01] exposure of our of our element. But yeah, that looks good. One thing we can do here is we can
[24:07] also add another like fill layer. Let's add like a clouds layer. clouds. Let's play with the contrast
[24:17] here. And with the tiling. And we can also set this to multiply. So now this clouds are hiding
[24:25] certain parts of the coins again in a random way. So each coin gets a slightly different effect.
[24:30] And we can play around with how much like metal edge where we're seeing and again, it's not going
[24:34] to be a uniform metal edge where which is going to give us a very, very nice effect. I do feel
[24:38] like the roughness is a little bit up for this one still. So I'm going to bring the metal roughness
[24:42] a little bit up not too much because I do want to have this sort of like shiny, shiny effect. But
[24:47] we definitely need to to bring it up a little bit to to match what we have right here. Now I can see
[24:53] that this one's very, very, very damaged with with the rust effect. So we might want to bring this
[24:58] thing underneath the rust effect. And that's going to as you can see bring the tone down a little
[25:03] bit as well because the rust are like overriding that sort of effect. So I'll leave that up to you.
[25:09] Like if you guys want to have like a very shiny coin, or a very like old coin, this is this is
[25:15] where you could do something like this. Now I'm going to add a scratch layer as I've mentioned.
[25:20] So I'm going to add another like stylized thing right here. And I'm going to add a black mask.
[25:25] This is going to be a generator. It's going to be or sorry, not a generator. This is going to be a
[25:30] fill layer. And we're going to be using a scratch mask. This one right here. And of course, we're
[25:39] going to increase a little bit of the balance on the tiling especially. Let's go here on the balance.
[25:48] There we go. Let's bring the contrast up. There we go. So now as you can see, we're adding this
[25:56] scratches pretty much individually, like each individual coin is going to have slightly different
[26:00] scratch. One of the things that we could do is we could go here to the technical parameters
[26:05] and push the height position down. And as you can see, that's going to carve in into the coins.
[26:10] So we're going to get some interesting lines, like hitting the or giving us some depth that we
[26:16] did not sculpt. And all of this is procedurally generated. And again, it's going to make the
[26:20] coins look very interesting because we have variation. And if you have a player and he grabs
[26:26] all of the coins and he wants to analyze them, we're going to have enough variation on all of
[26:29] them to get a very cool effect. That's pretty much it, I think. Finally, I would say like maybe
[26:38] another pass of rust might be a good idea. So let me show you another technique that we can use.
[26:42] I'm going to use a metal rust again. And instead of using a generator, I'm going to use a fill layer
[26:49] and I'm going to use the ambient occlusion of the coins. So the ambient occlusion map, as you can
[26:54] see right here, is inverted. So to invert this, I need to add a levels and invert this. And now we
[27:00] can play and generate a very, very interesting effect only on the cavities of the of the element.
[27:08] So I'm going to go with a really, really high like a rust amount like this. Of course, the color
[27:13] of the rust is going to be like this or like green color. There we go. And it changes to an overlay.
[27:20] Now, really, overly destroys it multiplies fine. And then I'm going to go really low on the multiply
[27:26] effect right there. Now, one thing I'm going to do here is on the options of the rust, again,
[27:30] I just want to affect the color. So I don't want to affect the roughness, this is just going to be
[27:34] adding like a like an extra layer of color. And as you can see, the coins are going to look really
[27:38] nice, really, really old. And it just changes like the tone on certain areas of the coin,
[27:44] while still keeping everything else intact. So yeah, that's pretty much it. Now I am going to
[27:50] file save this before we lose anything. Let's call this coins. And I'm going to go file, and we're
[27:55] going to export the textures again, which is going to export them on the desktop for now.
[27:59] Later on, I'll clean the desktop and I'll place everything where they're supposed to be. And
[28:03] this are going to be on real engine for packed coins. So I'm just going to hit export.
[28:10] And that's it. So yeah, that's pretty much it, my friends. With this, we are pretty much done with
[28:16] the creation of this asset. So it's the whole like texturing and baking process. Let me know down
[28:23] here in the comments if you want me to show you how we can get this into Unreal. However,
[28:27] we have the low polys and we have the maps ready. So this could perfectly, perfectly fine,
[28:32] going to Unreal without any issues. So yeah, that's pretty much for this one, my friends.
[28:38] Thank you very much for watching. Please don't forget to subscribe. If you are not subscribed,
[28:41] we're missing like almost half of the people that see the videos are not subscribed. It could really
[28:45] help the channel grow. And if you want to see the full process of as I've shown you before,
[28:49] we got a vests course right here with the acts where we go over the whole process, modeling,
[28:53] sculpting, low polyrhythmology, baking, everything. So if you want to delve deep into the production
[28:58] pipeline of 3d assets, well, you know where to go. Make sure to join us in this core Twitter
[29:03] everywhere and I'll be happy to see you next time. Bye bye.



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
