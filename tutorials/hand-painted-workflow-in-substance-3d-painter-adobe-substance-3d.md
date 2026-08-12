---
title: Hand Painted Workflow in Substance 3D Painter | Adobe Substance 3D
source: YouTube
url: https://www.youtube.com/watch?v=8biEy1D30Bc
author: Adobe Substance 3D
ingested: 2026-08-12
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
frames_dir: tutorials/frames/hand-painted-workflow-in-substance-3d-painter-adobe-substance-3d/
frame_count: 0
frame_status: pending-selection
---

# Hand Painted Workflow in Substance 3D Painter | Adobe Substance 3D

**Source:** [YouTube](https://www.youtube.com/watch?v=8biEy1D30Bc)
**Author:** Adobe Substance 3D
**Duration:** 25m25s | 6 section(s)

---

## Raw Data (for Claude Code extraction)

Frames are not captured yet. Read the timestamped transcript below, pick moments
that actually show a technique/result worth a still (not blind percentages —
even within a named chapter, verify the real moment against its timestamps), then run:
  python select_frames.py hand-painted-workflow-in-substance-3d-painter-adobe-substance-3d <ts1> <ts2> ...
(seconds or mm:ss). This appends a "Captured Frames" section and updates the
frontmatter before you write the Structured Notes below.


### <Untitled Chapter 1> [0:00]
**Transcript (timestamped):**
[0:00] There is one secret to creating amazing textures for your characters.
[0:03] Values!
[0:03] If you build proper values for your characters, converting those values to a usable color map
[0:08] is very easy with Substance 3D Painter.
[0:10] In this video, I'll show you how to create a black and white value map for your characters
[0:14] and then transform that with colors using Substance 3D Painter gradients and stylization filters.
[0:19] And of course, we will talk about hand-painted stuff and how we can build up the values to get
[0:23] to this final result. Let's go!
[0:25] Everything, as we know, starts with the bigs. If we have good bigs, then the texturing process


### Efficient Bake Creation [0:27]
**Transcript (timestamped):**
[0:29] is going to be super simple. The great thing is that we now have a very cool tool here inside
[0:32] Substance 3D Painter, which is the AutoCage feature. I'm going to load in my high poly right here,
[0:37] and what I did with this particular character is that I took every single part of it, the teeth,
[0:42] the harpoons, the main body, and divided it into its own underscore, low poly, and underscore,
[0:47] high poly. This is very important because with this, we're going to be able to tell Substance
[0:50] that we only want certain areas to bake into each other.
[0:53] So I'm going to go here into my high poly. I'm going to, of course, bake at 4K. I want to have
[0:56] the maximum resolution for this particular character, and we're going to change the match to
[1:00] ByMeshName. You need to go check here by the matching ByName, make sure that every single
[1:04] object has its corresponding element. We're going to set the anti-eyelasing to 16x,
[1:08] and there's a new feature, as I've mentioned, the AutoCage feature, which is on by default,
[1:12] but you can also change this to automatic experimental, and as you can see, it's going to
[1:16] try to find the specific cage for each of the elements in your object. So what this will do
[1:20] is it should give us very tight bakes without any contamination between the islands, because, of course,
[1:24] we have the match by mesh name, and we should get a very nice result. We're going to, of course,
[1:29] have our normal map. We're going to have our ambient occlusion, curvature map, and the thickness,
[1:33] which I'm going to be showing you some cool tricks at the end. If we go into our main
[1:36] viewport, we're going to be able to see the bakes, and as you can see, they look quite,
[1:39] quite nice. Keep in mind that this is a very low poly mesh. I believe this is only at 7K
[1:43] triangles for the whole thing. So I'm keeping it quite, quite low poly, which is usually what we
[1:47] do for some game engine pipelines. You might see a little bit of contamination going on here with
[1:52] ambient occlusion, especially on the borders where two meshes intersect, that's very common,
[1:56] and you can fix it by going to the croissant, going to the ambient occlusion map, and just change the
[2:00] self occlusion to only same mesh name. However, in this particular case, I don't think we are
[2:04] going to be struggling too much with that thing. There we go. Super clean bakes, super fast, and
[2:09] now we're ready for building up our values. For the hand painted process, one of the things that's


### Value Construction with Generators [2:12]
**Transcript (timestamped):**
[2:13] very important in most of the pipelines, not all of them, is that we're going to be baking all of
[2:18] the information, the normal map information, all of the crevices, all of the information
[2:21] of our geometry into a single color map. So if I press letter C right now, I'm going to be jumping
[2:27] to the different channels, and I'm going to jump all the way to the base color channel right here.
[2:31] I'm going to add a fill layer, I'm going to call this main value, and this is going to be the value
[2:35] that I'm going to be starting with. I usually like to start with darker values such as this
[2:39] mid darker tone gray, and we're going to be using this to build up all of her volumes and make sure
[2:44] that our character looks 3D in a simple flat map. The first generator that I'm going to add,
[2:49] I'm going to add a black mask right here. And on the base color, I'm just going to go for an
[2:52] ambient occlusion map. What this will do is it will connect the ambient occlusion map that we
[2:55] baked into this layer. So now if I want to do or change anything on this base color,
[2:59] the only thing I need to do is right click at the levels right here, and we can play with
[3:03] levels to change how the ambient occlusion looks. So I'm going to push it a little bit more just
[3:06] to get you know, a little bit more punch right here. And the cool thing is we can set this
[3:10] layer to something like multiply. When you set a layer to multiply all of the white colors of
[3:15] the lighter values get pretty much erased, and we're only gathering or multiplying the darker
[3:19] values against the background, which in this case is our main value right here. Now, a very
[3:23] important thing about values is that you never want to push them to the extremes. I personally
[3:27] really like the impressionism sort of like style that we have right here on some of these examples,
[3:31] because if you take a look at that, if you study the colors, you're going to see
[3:34] that you don't need super dark colors or super bright colors to express shadows and lights.
[3:40] And a lot of new projects nowadays are using this for like more pastel looking color palette,
[3:45] to really imply all of the value differences without really crunching all of our elements.
[3:49] So what I'm going to do here is exactly that I'm just going to bring the overlay here or the opacity
[3:53] a little bit lower so that we don't have pure blacks on our element. The next layer that I'm
[3:57] going to add is a very nice layer that I love using, which is the light generator. I'm going to add
[4:02] a few layer here, black layer, add a black mask, right click at a generator, and we're going to use
[4:07] the light generator. I've talked about this generator before, as you know, substance 3D
[4:10] Painter has so many generators, but this one's pretty cool because we can use this knobs right
[4:13] here to push the direction of the light. And in this case, since it's the shadow, I'm going to
[4:17] push the knobs down here, and we can play with the highlight glossiness as well as the highlight
[4:22] level to really push the shadow and start giving us that volume that we perceive on the element.
[4:26] This one, I'm also going to set to multiply, and I'm also going to play a little bit with the
[4:30] multiplier here so that it's not super super dark. Again, we don't want to go to the extremes,
[4:34] because once you get to those extremes, there's no way to go even further if you want to push
[4:38] certain things more. So look at the big difference, just two layers, and we already have a lot of
[4:43] volume being described here on our character. But we definitely want to highlight some other
[4:47] elements a bit more. So what I'm going to do now is I'm going to add a new layer, I'm going to call
[4:51] this main light or light, and I'm going to right click, add a black mask, right click, add another
[4:55] generator, and we're going to again add our light generator. And with this one, I'm going to make
[4:59] sure that this is pointing up. I'm going to play a little bit with here with the highlight glossiness,
[5:03] just making sure that this blends a little bit better. Make sure you do don't overexpose things,
[5:07] you can see that when we overexpose, especially this upper area, we lose all of the beautiful
[5:11] detail that we had from the high poly. So we need to find a specific point where we see a little
[5:15] bit of this volume, but it's not overwhelming my element, I'm actually going to use a little bit
[5:19] of light attenuation here, so that we don't get light all the way down here onto the belly of
[5:23] the shark. And you can see how this one can really make everything pop quite quite nicely. I'm going
[5:28] to layer one more. And this is one of the things that I wanted to show you on this tutorial, the
[5:31] fact that you can combine as many of these generators as you want. Actually, let me just
[5:35] duplicate this thing right here. And what I'm going to do is I'm going to go back to the light
[5:38] generator. Here's a little trick that I like to do. I change the color to a very bright color
[5:42] to really see where this thing is affecting the shark. And if I go to the light generator,
[5:46] I can play for instance, a little bit with the highlight glossiness. So that now this
[5:49] second layer of white is only hitting the very highest points of my element, which is a little
[5:54] bit more, it's going to give me a little bit more of a shiny look to the whole thing. And then of
[5:57] course, we go back to the color, and we get it back to white and look at that difference right there.
[6:02] So from this to this, we can now see the different layers of values. And that's one very important
[6:07] secret about color theory. Pick any of your favorite classical artworks for me, Rembrandt,
[6:12] an amazing artist. And if you pick any of those artworks, bring it into Photoshop,
[6:16] and then desaturate the whole thing, you're still going to be able to see what's going on.
[6:20] So even though colors are super important to make images and all of our like works pop,
[6:25] they're not the most important thing. The most important thing, the thing that our eyes perceive
[6:29] and the things that we need to really understand an image are the values. Similar to how when we
[6:34] were talking about anatomy, we talked about form and proportions. Well, in terms of color and
[6:38] in terms of texturing, one of the things that you always need to look for are values, making sure
[6:42] that the values properly describe the surfaces and the volumes, of course, of your piece. So I
[6:47] really like how this one's looking. I'm definitely going to lower this just a tiny bit, usually the
[6:51] highlights I like to add at the very end of my process so that I can have full control over them.
[6:56] And the next thing that we're going to talk about is something called a local color values.


### Color Construction with Gradients [6:57]
**Transcript (timestamped):**
[6:59] So every single object will have a specific sort of like tone to it. And you can see it on myself
[7:04] right now. My face is a lot lighter than my shirt, even though they're experimenting the same light
[7:09] sources here on the studio, they have a different local color value. And therefore the way we perceive
[7:14] them are going to be slightly different. So I'm going to add, for instance, a darker tone right
[7:18] here, all desaturated at a black mask. I'm going to go to number four, which is my field object
[7:24] element. I'm going to grab this and I'm going to fill in my harpoon, my ropes, which is very easy.
[7:29] If your mesh is separate is another big advantage of what we did on the high poly low polys or
[7:33] like breakdown. And now the only thing I need to do is change this to something like a multiply.
[7:38] And this will inherit some of the light information from the previous layers. Of course,
[7:41] this is way way too dark. But if we set this to something like I don't know 50% or something like
[7:45] that, you're going to have a slightly different color than the rest of the shark. And this is
[7:49] important so that we can have a little bit of variation and people know where to look at when
[7:54] they're appreciating our work. We can do the exact same thing with our teeth. So I'm going to go
[7:58] add black mask right here, select number four, select all of these things and then press X and
[8:02] click on the body so that the body is not selected. This one though, I'm going to change instead of
[8:06] using multiply, which is not really going to do anything. I'm going to change this to linear
[8:10] dodge. Linear dodge is very similar to multiply, but it pushes values up. So if you have lighter
[8:15] colors, it's going to sort of like exponentially make them brighter. And of course, we're also
[8:19] going to sort of like bring this down a little bit so that we can still see some of the lower
[8:22] tones or other tones that we had before. This again is usually referred to as local color values.
[8:27] And it's how we can change the whole thing to generate a little bit more detail. I'm going to
[8:31] add two more layers here, two more layers to really bring this into life. And the first one is going
[8:36] to be a generator later. It's going to be a dark layer at the black mask. And this is going to be,
[8:40] of course, our very common and very familiar dirt layer. There we go. Look at that. Now,
[8:45] one thing I'm going to do is I'm going to get rid of the grunge amount. I really don't want any
[8:47] grunge, but I am going to push the dirt a little bit more. I'm going to make this a little bit more
[8:51] extreme and you're going to see why in just a second because now one of the things that I can
[8:54] do is I can right click at a filter. And I really like using the blur slope filter because it really
[9:00] breaks things down and gives this sort of like artsy feel to the whole thing. We're going to
[9:03] talk about filters a little bit more at the end of the video. I'm going to change the intensity
[9:06] divided to something like 10 so that the splotches or the breakpoints are not as big. And then, of
[9:11] course, we can set this to something like a multiply again and just lower the opacity a bit.
[9:15] Because yes, I want to introduce a little bit of variation on, for instance, the teeth and some
[9:19] of the gills and things like that, but not too much. You got at any point go back here to the
[9:23] color, for instance, and if the value is a little bit too low, we can also sort of like increase
[9:27] it a little bit so it's not overwhelming. Finally, I'm going to add one more layer and this is going
[9:31] to be a black mask generator as well. And we're going to go with a metal edgeware metal edgewares
[9:36] are also very nice because they're going to help me with the highlight of the borders. I'm going
[9:39] to increase the highlight level of this thing same stuff. I don't want grunge. So I just want to keep
[9:43] this very, very simple on the borders. And then what I'm going to do with this one is I'm actually
[9:47] going to use another generator. And this is going to be a position generator. So the position generator,
[9:52] remember, you can always press Alt and click on the mask to see what the mask is doing. The position
[9:56] generator is a very good generator to have, well, a gradient. And in this case, I just want that sort
[9:59] of like metal edgeware on the top part of my shark. So if I go here, I can set this to multiply.
[10:05] And as you can see, we're going to have more of this metal edgeware on the top parts of the shark
[10:08] and less of the metal edgeware on the bottom parts. Now, of course, this is a little bit too much.
[10:12] So I'm going to go here to my element, I am going to set it to linear dots so we get more color out
[10:16] of it. And then I'm going to bring it down. I usually like to keep this at something like 20%,
[10:21] 25%. So it's mainly just a guide and an indication to break up the silhouette a bit more with my
[10:26] whole thing here. So there we go with this, we've successfully completed the basic construction of
[10:31] our values. And now, even though we're in the base color, completely flat element, we can still see
[10:36] the volume and it looks like a three dimensional shape. So we're not going to be dependent on any
[10:40] lights or any normal map information to describe the form. And we can see this little guy swimming
[10:44] around and attacking us in the game. The next step, oh, you're going to like it. I'm going to grab all
[10:48] of the elements right here, control G to create a new group. And I'm going to call this group my
[10:53] values. At any point, I can add more generators, I can paint some layers in like if I want to bring
[10:58] some values up or bring some values down, it's very easy to just add more layers inside of this.
[11:03] And what I'm going to do is I'm going to right click on this thing, and I'm going to create an
[11:06] anchor point anchor points can also be created to groups. And this is very, very important because
[11:10] we can transfer information from one part of our project to another. So now that we have an anchor
[11:16] point that's called values, we can use that information to start coloring our shark. The way
[11:21] we're going to do this is by adding a new fill layer and instead of filling this layer with a
[11:25] uniform color, I'm going to click on base color, I'm going to go to anchor points and I'm going to
[11:29] sample the values anchor point that I have right here to make this clear. What I'm doing is I'm
[11:33] taking all of the layers that I have on the values folder, creating an anchor point that adds all of
[11:38] those layers. And now I'm pretty much merging them procedurally because at any point, I can go back
[11:43] and change the values here into this new main color layer. This is where the magic happens.
[11:49] When I right click on this thing, and I'm going to add a filter, and the filter that I'm going to be
[11:53] adding is only going to be affecting the color, and it's going to be the gradient filter. So the way
[11:57] the gradient filter works is it's going to take a specific amount of colors right now, it's set to
[12:02] three, but I'm actually going to set this to four, going to take a specific amount of colors, and
[12:06] then it's going to remap the values that we have right now to the new colors that I'm selecting.
[12:11] So for instance, if I grab the black colors, and I set this to red, you can see that all of the dark
[12:15] tones or all of the dark colors are now going to be set to red. If I do the exact same thing with
[12:20] the white colors, but let's say to green, we're going to see this gradient where we're going from
[12:24] again, this nice red to this nice green right here. Now color theory is a whole nother topic,
[12:29] we can maybe talk about that in another time. But right now, I'm going to select a very simple palette
[12:33] that follows this or like greenish bluish hues for the zombie shark. I'm going to go for the darkest
[12:38] tone and I'm going to go to this green bluish hues, I'm going to go dark and quite saturated,
[12:43] something like that. The next color is also going to be on this or like green, a little bit more
[12:46] desaturated, something like that. There you go. I really like that tone right there. And then the
[12:50] next one, of course, going to be close to this one, but we should be pushing a little bit higher.
[12:55] And normally what I recommend is shift your hue a little bit. In this case, I'm going to go a
[12:58] little bit more towards the blue colors, so that we have a little bit more of a juicy image, right?
[13:03] Like not everything is super monotone. And then the last one, I'm also going to sample this color,
[13:06] I'm going to push it up. I might go even a little bit closer to the teal colors or the blue colors.
[13:11] There you go. And again, don't go to the borders, don't go to limits. We're going to push that later.
[13:15] Once we have that, we can use this as lighters right here to really push some of the dark shadows
[13:20] or some of the mid values right here to showcase or get a little bit more of a grungy, intense gradient.
[13:25] So this is how you're going to be controlling this initial block out of the color. For instance,
[13:30] I'm going to go to this green right here and actually kind of want to go to a different tone.
[13:33] So I'm going to go for more of a blue hue instead. There we go. Maybe just a little bit less darks or
[13:39] something like that. Remember, this is grabbing the information that we had from our values and
[13:43] converting that into a color gradient. It kind of looks like a phantom shark. I like it. Be very
[13:48] careful not to go over the position of the colors. If this happens, what's going to happen is you're
[13:52] going to have some weird effects or weird artifacts occurring on some of the elements because you're
[13:56] pushing some of these values lower than the original one should be. So it should look a little bit
[14:00] more like a like a share step effect. If some of the values are a little bit too bright, we can
[14:03] always sort of like tone them down and anytime later on, we can of course modify those colors as well.
[14:08] We can repeat this process now with another element. For instance, the teeth. So I'm going to grab a new
[14:13] fill layer right here, go to the base color anchor points, grab my values, right click. I'm going to
[14:17] add a black mask right here. And what I want to do is of course, select only the teeth like that.
[14:24] So now if we go to this one, right click, add another filter, turn everything off and select
[14:29] our gradient, we're going to be able to do the exact same thing. So for instance, in this one,
[14:32] we're going to go for like a darkish brown for the root of the teeth. And then we're going to go
[14:37] like this beige color and then the highlights, why this fine, but again, I don't like using
[14:42] those extremes. I'm going to push a little bit more towards the yellows and keep it something
[14:45] like there and play with these ranges crunch the values a little bit so that we can see a
[14:49] little bit more of that effect showing through. And also use this to give a little bit of a
[14:54] better impression in the local color values that we were talking about, right? So as you can see,
[14:58] by adding a couple of extra gradient layers, we can completely colorize our element and have a
[15:02] base layer to work with. Now let's add a little bit more color. I'm going to add a couple of layers
[15:06] to sort of like bring this thing more to life, even though it's an undead shark first layer,
[15:11] a red layer, you know, some blood, a little bit of life, black mask generator, dirt generator.
[15:17] But I kind of like this color, it's looking quite quite nice, but I'm going to do a couple of changes
[15:20] here. Instead of using the multiply or the overlay that are very, very intense. And while not keeping
[15:25] the normal map, I want to set this to color. If you set this to a color blending mode, what's
[15:30] going to happen is it's going to try to keep most of your values in check. So it's not going to be
[15:34] super, super aggressive in this particular case. So I'm going to push this down, of course, I'm
[15:38] going to keep this at like a 31, 32%. And as you can see, this is already incorporating a little bit
[15:43] of life to the whole thing. Another layer that I love using is a little bit of thickness layer.
[15:48] So if we go here to our layer, I'm going to grab a color similar to what we already have. So this
[15:52] is like phantomish grayish or greenish color. I'll try to keep it really saturated for just
[15:57] one second. When I add a black mask, I'm going to add a fill layer. In this fill layer, I'm going
[16:01] to look not for the ambient occlusion, but for the thickness map, because the thickness, as we know,
[16:06] will tell us which parts of the element are thicker and which parts are thinner. What I want to do
[16:10] here, of course, is I'm going to add a levels, and I'm going to flip this so that we're going for the
[16:14] thin areas right there. And then if we set this to linear dodge, you're going to see how this
[16:19] elements start to glow very, very nicely. The cool thing again is we can play with some of the
[16:24] elements right here to make sure that this is only hitting some specific parts of my character.
[16:28] I'm actually going to try something else like a color again. Yeah, there you go. Color is actually
[16:33] giving us a nice vibe there because it's it's filling in where it's adding a little bit of color
[16:37] to some areas. I'm going to have it below the blood though. And that should add just a little bit
[16:41] of extra life to the whole thing. If you don't want something at any point, we can just go to
[16:45] something like a paint layer, just paint out some of the sections. For instance, here in the mouth,
[16:50] I'm definitely going to be using another type of like effect. But look at how cool our whole
[16:54] shark is looking now without the need to be doing anything hand painted so far. This is all just the
[17:00] construction of the values and the construction are fine. Our initial color blocking. Now at this
[17:05] point, we can use some new stuff. I'm going to control G all of her color. Keep in mind that
[17:09] all of this is procedural. So if at any point your art director or your client tells you, hey,
[17:13] we don't want the shark to be blue and gray, we want this to be a little bit different, a slightly
[17:17] different color. Just come back here, go to the colors and switch things around and everything's
[17:21] going to update in real time without you having to go and paint. Hopefully you guys can see how
[17:25] powerful that tool is. Now one thing that we're definitely missing is a little bit more variation,
[17:30] especially on the top part of the shark. Usually sharks are a little bit darker in terms of the
[17:33] skin on the top part and lighter on the bottom right now due to the way we're building the light.
[17:38] It's looking a little bit different. So I'm just going to add a new layer right here. I'm going to
[17:42] add a black mask. And the way I like to approach this type of like blockings is just worrying about
[17:47] the main things first, and then worrying about the colors. So for instance, here, using the black mask,
[17:52] and of course, using symmetry here inside the substance three, the painter, we're going to just
[17:55] move this thing a little bit towards the center. There we go. And we can paint all of this like
[18:00] upper layer of the shark. Once I have that, it's a lot easier to just go back here, select a nice
[18:05] green color that I want to use against probably going to be this dark green color and look for a
[18:09] specific blending mode that really helps me in this case. Again, I can try something like color,
[18:13] that's definitely going to be too much. You can try value. Oh, that looks interesting. But let's go
[18:17] for something simple like an overlay, and then just play a little bit with the opacity. That way,
[18:22] we still keep most of the values that we have, right, like this little brighter elements,
[18:26] while getting or winning a little bit more variation on the top. In the animal kingdom,
[18:30] we have what I call the giraffe principle, which means that if you want to add any type of pattern,
[18:35] it usually fades. It never just like abruptly stops. There's always a little bit of a fade.
[18:39] Like a look at the spots on the giraffe, and you're going to see that on the center mass of
[18:42] the giraffe, there's going to be big spots. And then as you go towards the legs, the spots become
[18:45] smaller and smaller until they pretty much fade into a lighter color. You're going to see this
[18:48] everywhere in the animal kingdom. So what I can do here is do something similar with a dots pattern.
[18:52] So I can start adding a little bit of dots here, and then just losing some of those elements,
[18:56] we can start with bigger dots, closer to the line where it starts generating this sort of like blend.
[19:01] I'm going to go even bigger and just to start up here so we get some big spots every now and then.
[19:06] And as you can see, the little spots that we have are going to help me blend that whole thing and
[19:10] generate a very interesting texture. Then of course, we can keep on playing with a little bit of the
[19:15] intensity here. I do feel like my colors are getting a little bit dark. So I'm going to go back
[19:19] to the initial gradients right here. And this meat tone, I'm just going to push it up a little bit
[19:24] so that we can see a little bit more of our shark. And this is again the beauty of the gradients and
[19:28] this value process that at any point, we can just go in here and modify some of these elements so
[19:33] that we can find something that looks a little bit nicer. And I have one more layer right here at the
[19:37] very top black mask and of course, going to select the eyes. And I think I want to go for some like
[19:41] ghostly look. So maybe something like this highlight blue right there. And of course,
[19:46] set to linear dots so that we can get a little bit of information, right? Some some glow effect
[19:51] right there. Now the final little thing that I'm going to show you right here are the new


### Stylization Filters Details [19:54]
**Transcript (timestamped):**
[19:54] stylization filter that we have. And even though they don't make the whole thing for you, like
[19:59] they're not going to solve all of your issues, they're not like a magic thing that we just
[20:02] wave around. And they're just magically going to give us perfect hand painted stuff. They do give us
[20:07] a lot of interesting texture and interesting patterns that we can use as a sort of inspiration
[20:11] and as a base to keep on pushing from there. Right click on the folder right here, add a new filter,
[20:17] make sure that this is only affecting the color information and grab this new stylization filter.
[20:22] What the stylization filter does is he takes the information in this case from all of the group
[20:27] and it converts it, it literally replaces what we have and gives it a little bit of this like
[20:32] artistic look. It looks a little bit blur right now, but there are some things that we can control
[20:36] to get a better result. The first thing is the preset. If we change some of the presets, for instance,
[20:40] if we go to this hand painted style, you're going to see that the way the brushstrokes look are going
[20:44] to be slightly different. I really like this one right here because he definitely tries to follow
[20:48] so like the shape or the direction of some of the brushstrokes that we have.
[20:52] Keep in mind that right now this is a stylization filter is set to replace, meaning that it's
[20:56] literally replacing everything inside of the folder and giving us this result. You can blend
[21:00] this. If you want to have a little bit of your original color, you can use this to blend things
[21:04] a little bit or you could even change this to something like a linear dodge or something
[21:08] like an overlay. Of course, this is going to be way way too dark, but it's a good way to sort of
[21:11] like generate a different result. If we go back here to the elements, we can reduce the stylization.
[21:16] What's going to happen is we're going to recover or get a little bit more for original colors and
[21:20] gradients and get rid of this sort of like stylization effect. In the brush stroke sessions,
[21:24] I really like to increase, for instance, the brush strokes amount and you can also bring
[21:28] the strokes scaled down so that the strokes are a little bit smaller. There's even interesting ones
[21:32] like this colorful strokes that will give us a lot of variation on the colors as well. Look at that.
[21:37] I didn't know that this is way too extreme, right? But again, if we start blending this with
[21:41] something like, I don't know, like a linear dodge and then play with the opacity of this thing,
[21:45] we might be able to incorporate an interesting set of tones here and there that we could use as
[21:49] an inspiration to add to our final handpainted approach. So I finally settled with this one right
[21:54] here and I'm using roughly half of the stylization filter. I got rid of the big lighting for this
[21:59] one, increase the strokes amount and decrease the scale. And as you can see, we get a nice result.
[22:04] Now, I know what you guys are going to say, you're going to say, but Dave, this is not handpainted.
[22:07] You've just been using filters and generators and all of these layers to create a picture that
[22:13] looks handpainted, but it's not exactly handpainted. And you are totally right. Keep in mind that with
[22:18] any of these workflows, there's a multiple ways to get to a desired result. In this particular case,
[22:22] I'm using all of these generators and this buildup to get me a base to then go in and actually do the


### Hand Painted Style Approach [22:28]
**Transcript (timestamped):**
[22:28] handpainting process. Now, I'm not going to be able to show you the whole process, but I want to show
[22:32] you the tools that I normally use when building my handpainted layers. First, I like to use my
[22:36] basic heart brush and I like to go to my alphas and change the alpha to a square alpha. This is
[22:41] so that I get a little bit more of a texture and something that looks a little bit more organic
[22:46] or interesting. I do remove the size, pen pressure right here. And I do turn on my pen pressure on
[22:51] the stroke opacity, bring the spacing as low as you can, and then bring the stroke opacity relatively
[22:57] low. Because I do feel like the opacity here inside of substance 3D painter can be a little bit
[23:01] heavy sometimes. Once you have this, it's very easy. Just hit P on a color, sample the color that you
[23:05] have right there, and you can start painting and adding a little bit of value. What we're going to
[23:09] be doing, of course, is we're going to be adding this value on specific areas of our element to
[23:14] build up the volumes that we want. If you want to bring this higher up, then the only thing we need
[23:19] to do is grab a little bit of a lighter color and then start building this elements right here.
[23:24] Of course, once we have this, we hit P again, start grabbing some of the mid values and we
[23:28] start blending. This is the time consuming part. This is, in my opinion, the most fun part of the
[23:33] whole process, which is to use what we've already created with the base of our element and using
[23:38] the tools that we have here within Substance 3D Painter, just build up all of the remaining layers.
[23:43] This right here is the result of one hour of painting. I went over and I started adding all
[23:47] of the values on the top areas of my element, all of the light colors, added more saturation on the
[23:52] teeth. And you can see a lot of the initial setup or a lot of the initial construction is still here.
[23:58] After roughly another hour of polishing, this is what I have right now. And I usually make folders
[24:02] with these stages so that I can go and tweak certain values depending on if I want to modify
[24:06] any of the elements. You can keep pushing this. You can keep adding more stuff, adding more layers,
[24:10] adding more generators and building up the desired result for whatever art direction you're following.
[24:15] I'm adding three final layers right here. The first one is a very basic light layer with a little bit
[24:20] of a brownish, sort of like warm color here on the belly, because I thought that the colors were
[24:24] looking a little bit too uniform and this sort of like breaks that down. It also gives me a little
[24:27] bit of a bounce light coming from the bottom, which I think works quite nicely with this character.
[24:32] This position layer is really interesting because what I'm doing with this position layer, if you
[24:35] take a look at the mask, is I'm actually desaturating some parts of the element. So at the further down
[24:41] we go, the more desaturated we get. And this helps me bring the attention to the upper parts of my
[24:46] character. I add this little highlight right here with another light generator just to punch the last
[24:51] little bits of highlights on my element. And finally, a final noise texture here on the top to
[24:56] break up some of the uniformity on the patterns and give me a nicer blend along the whole surface.
[25:00] So as you guys can see, we went from the bakes to the basic construction of our values,
[25:05] to the main gradient colors, to the paint and stage, and then of course, details and presentation.
[25:10] This is the workflow that we can use. And thanks to the tools within Substance 3D Painter,
[25:13] we can get there very, very quickly. I hope you liked this video, my friends. And I hope you learned
[25:17] a lot. And if you want to learn more about Substance 3D Painter, make sure to check more
[25:20] tutorials like this one here in Substance 3D Channel. I'll see you back on the next one.



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
