---
title: Complex Wooden Medieval Door Tutorial in Substance 3D Painter
source: YouTube
url: https://www.youtube.com/watch?v=cRKK4YOXLtQ
author: Abe Leal 3D
ingested: 2026-08-12
app: "Substance 3D Painter"
version: "11.0.0+ (confirmed by feature combination: experimental Auto-Cage baking, Auto-update for modified/linked assets, and the Bevel Smooth filter — all introduced in 11.0.0 per release-notes-painter-11.0.md; likely 11.0.x-11.1.x)"
tags: [layers, fill-layer, paint-layer, masks, generator, anchor-point, blend-mode, baking, mesh-maps, ambient-occlusion, curvature, thickness, world-space-normal, position-map, high-to-low-poly, cage, udim, texture-set, procedural, tri-planar, alpha, height, roughness, metallic, basecolor, MatFX, advanced]
extraction_status: complete
frames_dir: tutorials/frames/complex-wooden-medieval-door-tutorial-in-substance-3d-painter/
frame_count: 8
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Complex Wooden Medieval Door Tutorial in Substance 3D Painter

**Source:** [YouTube](https://www.youtube.com/watch?v=cRKK4YOXLtQ)
**Author:** Abe Leal 3D
**Duration:** 20m40s | 8 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Intro [0:00]
**Transcript (timestamped):**
[0:00] Adding detail to our models can be a little bit tricky, but it doesn't have to be that way.
[0:03] In this video, I'm going to be showing you how to create the detail for this door right here,
[0:07] without having to do any sculpt on the high poly and keeping it procedural so that we can change it
[0:12] anytime we want. This video is sponsored by Adobe Substance 3D Painter and I'm very happy to be
[0:16] showcasing all of these techniques because as we know, Substance 3D Painter is the best software
[0:20] out there to texture our assets for commercial work, for our games, for our films, for anything 3D
[0:25] related. So let's go. This is the model that we're going to be working with. It's a very simple,


### Baking [0:26]
**Transcript (timestamped):**
[0:29] low poly. Of course, I have the high poly and we're going to go through the baking process
[0:32] real quick. And I am going to be using a high amount of resolution. I have four UDEMs for this
[0:37] particular door because I want to make sure that you guys see all of the detail, but you can adapt
[0:41] all of the techniques that we're going to be looking at to any resolution that you're going to be
[0:44] working with. Let's jump real quick to the croissant right here. And I'm going to of course load my
[0:48] high poly and there's a very cool new feature that we have inside Substance 3D Painter, which is the
[0:52] AutoCage feature. So now every single one of my elements, you can see I split all of my different
[0:57] beams and sections into its own high poly and low poly. All of them are generating the cage and
[1:01] they're expanding the cage to the specific size that they need for the details that we want to
[1:06] bake down. We can still play around with the max frontal distance and the max rear distance if you
[1:10] are having some issues with your bakes, but it should give you a closer bake for all of your
[1:14] different parts. I'm going to set the match to buy mesh name and I'm going to change the anti-aliasing
[1:18] to 16x and then we can start baking. Of course, we're going to see our normal map, that world
[1:22] space normal, very important for some specific textures, our ambient occlusion, which is one of
[1:26] the most important maps to add all of the dirt and grunge to our element. We also have our curvature
[1:31] map for the nice edges and the little crevices that we're going to be adding. Finally, the position
[1:35] and of course the thickness map, which I'm going to show you a little secret at the end to add just
[1:39] that little extra detail to the color. Once our bake is done, we can check it out here in the main


### Materials [1:42]
**Transcript (timestamped):**
[1:44] viewport and as you can see, everything looks very, very clean. We're not really getting any
[1:48] contamination between the different beams and all of the detail has been baked down quite, quite nice.
[1:52] Now before we start with the height carving, which is a very cool technique that I'm going to show
[1:56] you, I do want to add a very simple wood material so that we have an idea of how the door is going
[2:00] to look. Now, if you've been living under a rock, the assets library is now available inside of
[2:05] Substance 3D Painter and if you have an active subscription, then it doesn't require any sort
[2:09] of credits to download any of the assets models or HDRIs that you might need. So I can literally go
[2:14] to this tab right here, look for wood pine, just download that one right there. I'm actually going
[2:19] to download this one instead. I want to use the aged pine wood right there. I'm going to go to
[2:23] assets and there we go. I'm just going to drag and drop this into my element and look at how
[2:26] nice that looks. First thing I'm going to do is I'm going to change the tiling to two to get a
[2:30] little bit more fibers because it's supposed to be a very big door and I'm going to rotate all of
[2:34] this to 90 degrees. This is very, very important. I built this asset specifically because I wanted
[2:39] to make sure that all of the UBS of the beams were going in a nice straight direction and as you can
[2:43] see by doing that, all of my UBS for this dialable materials are going to be following the grain of
[2:47] the wood. I do feel like the height information is a little bit too high and just lower this to
[2:51] something like 10%. We haven't even started and we already have a very, very nice base for this
[2:56] door right here. I want to make it a little bit browner. So I'm going to add a new fill layer
[3:00] right here, grab a reddish orange color and on the color information right here, I'm going to change
[3:05] this to multiply and then I can lower the intensity right here and this is a way for me to sort of
[3:10] like darken the colors. I usually like to start with dark tones and then work my way up to the
[3:14] highlights of our element. You could of course also go here to the wood element, switch the
[3:18] hue a little bit or play with any of the properties like the wood color variation, the
[3:22] Bain's contrast, even the roughness right here. This is the magic of procedural materials, the
[3:26] fact that you can change so many things and every single asset that you do is going to be slightly
[3:29] different. Keep in mind, we always have the seed option right here that we can click and every time
[3:34] we click it, we're going to have a slightly different variation on the color. So if there's a
[3:37] couple of wood grains or wood elements that you don't like, just click on this seed until you
[3:40] find something that looks a little bit better. This one, for instance, I really, really like. Now
[3:44] we're going to go to one of the big tools that I want to show you in this video and that is
[3:47] height carving. So I'm going to grab here a fill layer and I'm going to set this fill layer to white
[3:52] for now. I'm going to turn on the height and I'm going to push the height all the way to the bottom
[3:56] section right here. I'm going to call this layer carvings and I'm going to control G to group it.
[4:00] This one's going to be called height layers. So anything that I'm going to be doing height related,
[4:04] it's going to be on this folder right here. I'm going to right click and add a black mask and
[4:08] what's going to happen now is if I grab any of my brushes and I start going across some parts of
[4:13] the wood, you can see that it's going to look like we're actually carving into the wood because
[4:17] all of this is height information. We're pushing the illusion of the surface up and down,
[4:20] thanks to the height map that eventually is going to be converted to a normal map
[4:23] so to keep this sort of like effect. Now here's where things get very, very fun. I'm going to go
[4:28] to Photoshop and I'm going to have this interesting pattern things looking here. Like what is this?
[4:32] Well, what I did is I went ahead and I use the UB layout of my door to start planning how I want
[4:39] this patterns to be carved into my door. So instead of having to go to my high poly and sculpt
[4:44] everything and then having to make changes or decide for other patterns, I can do it in a very
[4:48] easy file right here, which is the black and white masks. Once we have exported that PSD file,
[4:53] we just bring it in here, we just import it normally and I'm going to right click on my mask,
[4:57] I'm going to add a fill layer and I'm going to drag and drop this one right here. And as you can see,
[5:01] the patterns appear on the door and we're using this layer to drive the height information. So
[5:07] instead of having to hand draw everything or move things around, I can just plan things ahead of time
[5:11] here on my Photoshop file, make sure that I plan things really, really nicely and then just bring
[5:16] that into substance. Now, this is not all. If we go here to our assets folder or assets panel,
[5:22] we can go down here to the little arrow and we can activate the automatic updates for our assets
[5:27] panel and for the resources used in this project, such as the texture that we have right here. So
[5:31] now if I go back to Photoshop and I change the patterns or add more stuff to the whole thing,
[5:36] the only thing I need to do is save this file and boom, it's going to automatically update
[5:40] whatever it is I did in my Photoshop file and apply it here to the carvings that we're working on
[5:46] this height layers. It's very efficient and it's an excellent tool if you're working again in a
[5:49] studio environment where we're with a client and they're constantly telling you to modify or move
[5:54] things around. Imagine having to do all of these sculpts inside of another sculpting software and
[5:58] then you need to go back, erase, re-sculpt and re-change like no, no, no, that's not a smart
[6:03] way to approach a lot of iteration elements like the ones that we're doing right here. So with a
[6:07] little of addition magic right here, I'm adding this tree, this pattern and all of these elements
[6:12] to my Photoshop file. I'm just going to save my file, jump back into substance and boom,
[6:16] we get all of the information again automatically updated thanks to this new feature, the auto
[6:21] updater for Substance 3 Painter. Now this is not it, we're just starting with the whole process.
[6:25] I'm going to go back to the color and I'm going to grab a darker color so that it looks like we
[6:29] are actually burned this thing into the wood. I'm going to change this to overlay, that looks pretty
[6:34] cool. So as you can see, this is what my mask is doing right now, but there's a couple of things
[6:38] that I want you to look at. First of all, some of the textures that I used to build this pattern
[6:41] are not really high quality. There's some like compression issues and some general things that
[6:46] we can fix by using some filters. So the first filter I'm going to be using is blur filter right
[6:50] here. I'm going to use the blur filter and that's going to soften everything up. And again, if we go
[6:54] to the material, you're going to see that yes, it's going to look a little bit nicer, it's going to
[6:57] look a little bit smoother. We're going to get a more intense curvature there on the carving,
[7:00] because instead of having a very intense cut, right, black and white, we actually have a little
[7:04] bit of a gradient, but I don't particularly like the effect that we're getting right here. So I'm
[7:08] going to use the blur, but I'm going to use it very softly. And now I'm going to show you a new
[7:12] filter that we have that's very, very cool. And this filter is called bevel smooth. So the bevel
[7:16] smooth will do a very, very cool process where every single black and white element you can see
[7:22] right here is going to be smoothed and beveled at the same time. I'm going to definitely bring the
[7:26] distance down. So something like this, I'm going to bring this moving down a little bit as well,
[7:31] but you can really see the difference. Look at the big changes that we have right here. This is
[7:34] how we started with just a very basic element. The blur gives us more depth. And then the bevel
[7:39] smooth sharpens all of the elements, all of the corners and all of the points to really make it
[7:43] seem like a carving. We're going to be playing with a little bit of this things, we can be used a
[7:47] little bit of the curve offset, for instance, to make sure that we get more of the values of our
[7:50] element. But this bevel smooth guys, a really, really, really powerful tool, again, to do all of
[7:55] these elements procedurally without having to worry about the high poly of our element. That's
[8:00] not all. I want to add one more little detail here to this height layer, right click, add a filter,
[8:04] and now we're going to be adding of course, the blur slope. The blur slope is a very damaging or
[8:08] very crazy filter that breaks up all of the edges of our mask. First of all, I'm going to change the
[8:13] intensity divider to 10 so that the damage is a lot smaller. And I'm going to change the blending
[8:18] mode so that it does not use a blur, but rather max. What max will do is it will only affect the
[8:24] outer edges of our element, right, like the maximum points. If we change this to men, what's
[8:28] going to happen is going to go to the inside of the element. And I want to affect or carve out
[8:32] the outer edges of the objects. I'm going to go here to max. And if we go over here, look at that,
[8:36] we get this very nice interesting chip defect across all of the different elements of our door.
[8:41] Every single carving, all of them are getting this very nice filter effect in a procedural way,
[8:47] in a non destructive way that we can at any point go into Photoshop, change our main element,
[8:52] and modify the result that we're going to be seeing here. This is why this process is so magical.
[8:56] Now, let's start building a couple of layers. We have a nice construction right here. I'm actually
[9:00] going to reduce the amount of color that we have right here. And I'm going to be building this in
[9:04] new layers. So I'm going to start with a very basic dirt layer. Let's go once more here to our substance
[9:09] 3d assets. And let's look for some dirt. And I want to use this loose dirt scramble. So I'm just
[9:14] going to download that directly into my assets folder. Now we just drag and drop this in the top


### Dirt Generator [9:19]
**Transcript (timestamped):**
[9:19] stack. I'm going to set this to multiply as well. Multiplies are very nice filter because it darkens
[9:23] the values. This layer has a very light value. It's going to multiply it against the values of
[9:26] the door. And it's going to make it darker. Look at the texture right there. Very, very cool texture.
[9:30] Right click, add a black mask, right click, add a generator. And we're going to add, of course,
[9:34] our dirt generator. We all love the dirt generator. And this is immediately going to make our whole
[9:38] thing look a lot nicer. But you might notice something interesting. The carvings that we have
[9:42] are not really affecting the dirt generator. If we turn them off, you can see that the dirt is
[9:46] not really affecting or going into the crevices of the elements. To do that, we need to use anchor
[9:50] points. And one thing that you guys might not know is that you can actually generate an anchor point,
[9:54] not only from layers, but from folders as well. So I'm going to go to the folder right here. And
[9:58] I'm just going to generate an anchor points going to be called hide layers. And now if I want to add
[10:02] more layers, let's say I do a different set of carvings, or I do any sort of like cuts or elements,
[10:07] anything that lives inside of this folder will generate a new anchor point with the hide layer
[10:13] information and all of the information for that matter. If we go back to the dirt layer,
[10:16] the only thing we need to do is go here to micro normal, go to anchor points, select our hide layers,
[10:21] change the reference channel to hide because that's the information that we want.
[10:25] Go to micro height, anchor points, hide layers, change the information again to hide, and then
[10:30] go up here to micro detail and turn this both on. And there you go. Look at that. So now as you can
[10:35] see, all of the hide information from this folder is actually affecting this dirt generator that
[10:40] we have up here, making it look way more realistic. Don't make the mistake that everyone does when
[10:44] using this generator, always try to break it up a little bit. I'm going to show you my traditional
[10:49] technique was just add a field layer right here. I'm going to add something like a clouds filter,
[10:53] press Alt and click on the mask to see what's going on, increase the balance, increase the contrast,
[10:57] play a little bit with the scale, and then multiply this against the previous layer.
[11:01] So as you can see, what we're doing here is we're using this dark spots of the clouds to break up
[11:06] some of the dirty information right now. I feel like the contrast might be a little bit too much.
[11:09] So let's soften it up. Let's increase the balance a little bit. And we can always play a little bit
[11:13] with the overlay right here. So that's it. You can see that the clouds layer can really help us
[11:17] break up that effect and allow us to have something that looks a little bit more believable. I'm still
[11:21] going to push the multiply layer a little bit lower here because that that amount of dirt is way,
[11:25] way too much. Now for the middle edge where we're going to do a very similar process, I'm going to
[11:28] go here to my base layers, grab one of the base colors, usually a light color like that one right
[11:33] here. Let's call this edges, right click, add a black mask, right click, add a generator. And
[11:38] we're going to add of course our middle edge where we're going to have the exact same issue right
[11:41] now. The middle edge where is being applied only to the edges and it's not really going into all
[11:45] of the nice carvings that we did with the height layers that we have over here. Go down here,
[11:49] micro no more anchor points, height channel, micro height, anchor points, height channel,
[11:54] micro details and turn this to on. There we go. So now as you can see, we are going to be affecting
[11:59] the elements the way we would expect the only issue as we already know, this is affecting things
[12:04] too uniformly, we're not really getting a nice result right click, add a few layer, let's add
[12:08] the clouds to again, all 10 click, I'm going to change this to try planner projection and multiply
[12:13] this that way as you can see the middle edge where it's not going to be present everywhere.
[12:16] And as with all of the things that we've done so far, all of this is procedural to at any point I
[12:20] can play here with the balance or with the contrast of the clouds noise and generate more or less
[12:25] detailed depending on what I want. This one I like to set to linear dodge because it really
[12:29] punches the color to the high points and then bring the opacity down that way it's not too
[12:33] overwhelming. I still feel like my dirt might be a bit much so lower that a bit because if you do
[12:38] things with too much crunch, it becomes too noisy, right? Like people don't really know where to look
[12:41] at and we already have a lot of detail going on thanks to this elements right here. So definitely
[12:45] you need to change that. So this to me would be the basic construction of the door, but we're not


### Moss Generator [12:46]
**Transcript (timestamped):**
[12:49] finished yet. We're going to go all in with this one. The next couple of layers that we're going to
[12:53] be adding are going to help us to push this asset to a more interesting level. And the first thing
[12:58] that I want to do is I want to do a little bit of ground dirt from our element. I'm going to grab
[13:01] the same dirt material that we used before, but I'm going to change the color. Instead of having
[13:04] this brown color, I want this to be more like moss or some sort of like organic matter growing on the
[13:10] bottom part. So I'm going to go for this sort of like dark greenish color, very desaturated moss is
[13:14] a lot more desaturated than what my things. I even like the little leaves that we have right there.
[13:17] I feel like they're going to add a nice effect. And this one I'm going to try overlay first. Look
[13:20] at that very nice dark intense green going on right there. And we're going to build our masts
[13:25] again in a very simple way. I'm going to add a black mask. The first mask that I want to add is
[13:30] going to be a generator and it's going to be a position generator. The position generator uses
[13:35] one of the maps that we have the world space normal and position gradient to know what parts of the
[13:40] object are closer to the ground and what parts of the object are closer to the ceiling. So if we
[13:43] flip this right here with the global invert, as you can see, we're going to have this very nice
[13:47] effect going from the bottom part of our element to the top part, which is very realistic. We see
[13:51] this in structures in the outside world. If we click alt and click on the mask again, you're going to
[13:55] see that it's relatively boring, right? So let's break it up a little bit. Now the interesting thing
[14:00] is we can actually break this up with some of the generators that we already have. So I would expect
[14:05] there to be a little bit more of this grunge on the inner edges, right? Like on the crevices. So I
[14:09] can add a generator right here at the metal edge where generator play a little bit with the where
[14:14] level and then multiply this against the first layer and look at that. We're now going to have
[14:18] a little bit more of that damage on the inside part of our object. We're actually doing it the
[14:22] opposite way. So I need to invert this and we can play again with all of the processes or the elements
[14:27] that we have right here to get an interesting effect where some of the edges are a little bit
[14:30] more protected than others, right? Like this or like moss is not growing everywhere. This is not
[14:34] where we should finish. I always recommend that you add a paint layer and using a brush like the
[14:38] dirt brush, for instance, you manually remove or add some of the elements that you might want. So
[14:43] for instance, since the door is going to be used a little bit more, it might not have as much damage
[14:47] as some of the other parts. So the outer pillars that are exposed to the elements a bit more might
[14:52] have more of this effect. And if, for instance, we see a piece of wood that recently fell off in
[14:56] this part, well, we might expect not to see that much damage on that particular point. This specific
[15:01] artistic decision is one of the most important things that people often overlook when creating
[15:06] their assets. Because if you let the software do everything, it's going to do a really good job,
[15:09] but it will never achieve that artistic touch that like deliver a decision of why we want certain
[15:15] elements to be missing. So adding again, this little details here and there, like making sure that you
[15:19] have the final artistic say on where we're going to have this dirt and these elements is really
[15:24] going to elevate your assets to the next level. I'm probably going to turn the opacity down just


### Light Generator [15:26]
**Transcript (timestamped):**
[15:29] a bit. I do want to have a high contrast, but maybe not that much. Another very common thing that we
[15:33] can do here is use a light generator to add a little bit more importance or a little bit more
[15:39] detail to the top part of our element. I'm going to add a new layer right here. And I'm going to
[15:42] imagine that there's like a warm light hitting our element from the top. I'm going to go for this
[15:46] sort of like orangey bife, right click, add a black mask, right click, I'm going to add a generator.
[15:51] And this is going to be my light generator. I love the light generator because literally like
[15:55] shining a light into our object. And we can use those little sliders right here to tell this thing
[15:59] where we want the light to be hitting. It also looks like a layer of dust, which can look quite,
[16:03] quite nice in this particular case. I'm going to decrease the highlight glossiness because as you
[16:07] can see, I want to have sort of like a soft gradient going into the bottom parts. And then I'm going
[16:11] to set this to linear Dutch. And what linear Dutch will do is it will multiply the colors and it
[16:15] will brighten up those elements. This one I usually keep very, very low, something like 5%, 10% at most.
[16:21] But you should see a little bit of a change there on the values on the element. Let's increase the
[16:25] linear Dutch so that we can see the effect a little bit more. The door is going to look a little bit
[16:29] lighter on the top and of course a little bit darker on the bottom. We can go a little bit
[16:33] grungier. So I'm going to use one of my favorite layers or one of my favorite materials, which is
[16:36] the rust material. I'm going to add a rust material right here. Add a black mask. And I'm going to
[16:41] use another generator, which is going to be an ambient occlusion generator. This is going to
[16:44] hit the ambient occlusion parts of our element. Invert this. I really don't want to use any of the
[16:49] cavity information right now. This is just like a general shadow that I want to add.
[16:53] Set this to overlay. I'm going to use this to darken the whole thing a little bit and get that
[16:57] sort of like interesting effect on the corners of our elements. Definitely going to change the color
[17:01] to a little bit of a darker, more desaturated brown. Actually, let me show you another generator
[17:05] that's very cool. It's relatively new as well. I'm going to add a new layer. I'm going to go for
[17:09] like a dark color as well, something like that. Black mask. And what I'm going to do is I'm going
[17:13] to add a paint layer. And have you ever seen those like places where you have a little bit of like
[17:18] dirt and rust and it's all like drips down. So I'm going to go to some of the corners of the door,
[17:22] not all of them. Now that we have those spots right there, I'm going to Alt and click so that we can
[17:26] see the mask, right click. I'm going to add a new filter. And this is called the blur directional.
[17:31] This is very, very cool because the blur directional, as you can see right here,
[17:35] will try to blur the element following a specific angle. In this case, I want to blur it so that
[17:40] it goes down like that. And we can increase the intensity. And you can see how it shifts it in
[17:45] this case in the direction of the UVs. So some of these lines are going on a different direction.
[17:49] We can clean them up in just a second, but it gives us very nice or like some mere defect to the
[17:52] whole thing that this do something like multiply and play a bit with the opacity. Now we really
[17:57] haven't done any changes to the roughness. That's another pass that we definitely need to add. I'm
[18:01] going to go all the way down to my field layer on my height maps. I'm going to turn on the roughness
[18:05] on this one. And I probably want this to be a little bit glossy. So like if they added paint or
[18:09] something, there you go. So now as you can see, when the light shines through the object, we're
[18:13] going to have a little bit of an interesting glint happening on some of the crevices of our element.


### Bolds [18:17]
**Transcript (timestamped):**
[18:17] I'm going to do some bolts. I'm going to grab a dark material right here, turn on metallic,
[18:21] make this very metallic, add a black mask right here, go to our brushes, like the basic heart
[18:26] brush right here. And I'm just going to start painting some bolts that I want to add. I'm going
[18:30] to go back to the material, use hide information as well, and push this hide information up. And
[18:35] we can use again some of the filters that we just saw. So I'm going to use filter and let's try a
[18:40] bevel smooth, definitely decrease the distance, decrease the smoothing, push the color up a bit.
[18:44] Let's turn on roughness. I don't want to make them a little bit rough and everything's procedural.
[18:48] So we can at any point go to the mask and change the size of those bolts if they're too big or too
[18:52] small. Once we turn on the bevel smooth, it should give us a little bit more of an interesting detail
[18:56] right there. Now, remember I told you I was going to show you a very cool trick with the thickness


### Thickness Map [18:57]
**Transcript (timestamped):**
[19:00] map. Well, wood has a property similar to skin where there can be a little bit of surface scattering.
[19:05] I'm going to add a new field layer. But this layer, I'm going to fill it with a very bright yellow
[19:08] right here. I'm going to add a black mask. I'm going to add a field layer. And on this field
[19:12] layer, I'm going to look for the thickness map. I'm going to add right click at the levels and
[19:15] just invert this thing. And look at this, all of the thin areas of my wood are getting this
[19:20] role like yellowish tint. We can push this values right here to make sure that only the
[19:25] sharpest lines get that particular effect like so. And once we have this, we can set this again to
[19:31] something like linear dodge and bring this all the way down to just brighten up the corners
[19:36] a little bit. It's almost nothing. But without having to go to complex shader stuff, it can
[19:40] really add a bit of life to the whole thing. And we can't even change the colors. You can try
[19:44] something a little bit more orangey, for instance, and you can see how it really affects and changes
[19:49] the whole sort of like vibe that we're getting from the object. A simple layer, but a very powerful
[19:54] layer. So that's it, my friends. This is the end of the tutorial. Hopefully you learned a lot of
[19:59] very cool tips and tricks for your own work. And hopefully you can see the power of working this
[20:03] way procedurally with mask with layers, making sure that at any point we can go back, change
[20:08] something and it will automatically update and affect every single thing we've done so far.
[20:12] Thank you once again to our friends at Substance 3D Painter. And please, please make sure to check
[20:16] their channels. They are sharing a lot of very cool information there as well. Make sure to check
[20:20] again Substance 3D Painter, download it, use it and texture amazing assets for your projects.
[20:25] That's it for now, my friends. I really hope you enjoyed this tutorial. Let me know in the
[20:28] comments what you think and don't forget, always learning, always improving. I'll see you back on
[20:33] the next one.



---

## Captured Frames

- [0:52] tutorials/frames/complex-wooden-medieval-door-tutorial-in-substance-3d-painter/frame_000.jpg
- [3:00] tutorials/frames/complex-wooden-medieval-door-tutorial-in-substance-3d-painter/frame_001.jpg
- [4:00] tutorials/frames/complex-wooden-medieval-door-tutorial-in-substance-3d-painter/frame_002.jpg
- [7:16] tutorials/frames/complex-wooden-medieval-door-tutorial-in-substance-3d-painter/frame_003.jpg
- [8:36] tutorials/frames/complex-wooden-medieval-door-tutorial-in-substance-3d-painter/frame_004.jpg
- [10:21] tutorials/frames/complex-wooden-medieval-door-tutorial-in-substance-3d-painter/frame_005.jpg
- [13:20] tutorials/frames/complex-wooden-medieval-door-tutorial-in-substance-3d-painter/frame_006.jpg
- [19:20] tutorials/frames/complex-wooden-medieval-door-tutorial-in-substance-3d-painter/frame_007.jpg

---

## Structured Notes

### Core Technique
Adobe-sponsored showcase of a fully non-destructive, height-map-driven "carving" workflow: instead of sculpting ornate medieval door carvings on the high-poly mesh, the pattern is authored as a black-and-white mask in Photoshop (planned directly against the door's UV layout), imported as a height-driving fill layer, and sculpted procedurally with filters (Blur, Bevel Smooth, Blur Slope) — kept live-linked so edits in Photoshop auto-update inside Painter.

### Summary
A multi-UDIM (4 UDIM tiles) medieval door asset, textured with zero high-poly sculpting for its carved ornamentation. Baking uses Painter's Auto-Cage feature (each beam/section split into its own high/low-poly pair, cage auto-expanded per element, matched by mesh name, 16x anti-aliasing) to bake Normal, World Space Normal, Ambient Occlusion, Curvature, Position, and Thickness. A base wood material is pulled live from the in-app Substance 3D Assets library (no credits needed with an active subscription), rotated 90 degrees to align UV-driven wood grain along the beams, tiling and height-intensity tuned down, then darkened with a Multiply-blend reddish-orange fill layer. The video's signature technique is height carving: a white Fill Layer with Height pushed to maximum, grouped into a dedicated "Height Layers" folder, masked with a black-and-white pattern authored in Photoshop against the door's UV layout and imported as a mask-driving fill layer — with the project's Assets-panel auto-update toggle on, saving the PSD instantly re-applies changes inside Painter with no re-import step. The raw imported pattern is refined with a light Blur (softens compression/quality artifacts), then the Bevel Smooth filter (bevels and smooths every black/white edge simultaneously, distance/smoothing tuned down) to read as an actual carved bevel rather than a flat cutout, and finished with a Blur Slope filter set to Max blending (chips/breaks up only the outer edges of the carved shapes) for a convincing worn-chip-damage look. A folder-level Anchor Point (generated from the whole Height Layers folder, not just one layer, referencing its Hide channel) is then wired into downstream Ambient Occlusion-driven dirt and Metal Edge Wear-driven edge-wear generators' Micro Normal / Micro Height / Micro Detail slots so those generators correctly read into the carved crevices instead of ignoring them — each broken up further with a Clouds-filtered fill layer in Multiply. A moss/ground-dirt layer uses the Position generator (position + world-space-normal-derived height gradient, Global Invert) for bottom-to-top placement, refined with a Metal Edge Where-generator pass and finished with manual paint-layer touch-ups for artistic control over exactly where growth should or shouldn't appear. A warm top-down Light generator layer (Linear Dodge, kept subtle at 5-10%) simulates directional highlight; an AO-generator-driven Overlay darkening pass and a hand-painted corner drip-stain layer (Blur Directional filter for a downward streak look) add further grime. Roughness gets a glossy pass on the height-carving fill layer for crevice highlights. Metal bolts are hand-painted with a hard round brush on a metallic material, their own mask pushed into the Hide channel and refined with the same Bevel Smooth filter. Finishes with the video's signature "secret" trick: a bright-yellow fill layer masked by the inverted, contrast-pushed baked Thickness map in Linear Dodge blend, brightening only the thinnest/sharpest wood edges for a subtle simulated subsurface-scattering glow.

### Key Steps
1. **Bake with Auto-Cage:** split the high-poly into per-element (per-beam) high/low-poly pairs so each generates and auto-expands its own cage to the size it individually needs; set `Match` to `By mesh name` and `Anti-aliasing` to `16x`; bake `Normal`, `World Space Normal`, `Ambient Occlusion`, `Curvature`, `Position`, and `Thickness`.
2. **Pull a base wood material live from the in-app Substance 3D Assets library** (no credits consumed with an active subscription) and drag-drop directly onto the element; rotate the material 90 degrees to align its baked-in grain direction with the door beams' UV layout (the asset was purpose-built with straight UVs so this works cleanly); tune `Tiling` up (more fiber detail on a large door) and `Height` intensity down (~10%).
3. **Darken the base with a Multiply color pass:** new Fill Layer, reddish-orange color, Base Color blend mode `Multiply`, opacity lowered — establishes the "start dark, build up to highlights" value-building philosophy stated explicitly.
4. **Height-carving setup:** new Fill Layer filled white, `Height` pushed to maximum, grouped (Ctrl+G) into a dedicated `Height Layers` folder so every carving-related layer lives in one place; add a black mask to the group.
5. **Author the carving pattern in Photoshop against the door's own UV layout**, planning exact carving placement/shape as a black-and-white mask file rather than sculpting — explicitly framed as the smart alternative to re-sculpting/re-baking every time a client requests a design change.
6. **Import the Photoshop pattern as a mask-driving fill layer** (right-click the mask -> add Fill Layer -> drag in the imported PSD) so the pattern directly drives the Height Layers group's height output.
7. **Enable Assets-panel auto-update for the linked PSD resource:** toggle on automatic updates in the Assets panel for that specific texture resource — from this point, saving further edits in Photoshop instantly re-applies inside Painter with no manual re-import.
8. **Color the carving as "burned" wood:** darker color on the carving layer, blend mode `Overlay`.
9. **Clean up compression artifacts with a light `Blur` filter** on the mask — softens jagged/low-quality edges from the source pattern file (used sparingly; too much blur was explicitly rejected as looking wrong).
10. **Apply the `Bevel Smooth` filter for a true carved-edge look:** bevels and smooths every black/white shape edge simultaneously; `Distance` and `Smoothing` brought down from default; described as transforming a flat cutout pattern into something that reads as an actual carved bevel — flagged as "a really, really powerful tool" for procedural carving without touching the high-poly.
11. **Add a `Blur Slope` filter for chip/wear damage on carving edges:** `Intensity Divider` raised (e.g. to 10) to shrink the damage scale; blend mode changed from the default `Blur` to `Max` so only the outer edges of each shape are affected (vs. `Min`, which would erode inward) — produces a convincing chipped-edge-of-a-carving look, applied uniformly and procedurally across every carved element at once.
12. **Generate an Anchor Point from the whole Height Layers folder (not a single layer)** — new to some viewers per the creator's callout: folders, not just individual layers, can be the anchor-point source, so any future layer added inside that folder automatically feeds the same anchor reference.
13. **Wire the folder anchor point into downstream generators via Micro Normal / Micro Height / Micro Detail:** on both a dirt layer's `Dirt` generator and an edge layer's `Metal Edge Wear` generator, set Micro Normal -> Anchor Points -> the Height Layers anchor -> reference channel `Hide`; repeat for Micro Height with the same anchor and `Hide` channel; enable `Micro Detail` — without this step, generators ignore the carved crevices entirely and only affect the flat surrounding surface.
14. **Break up generator uniformity with a Clouds-filtered fill layer:** new fill layer with a `Clouds` filter, Alt-click the mask to preview, tune `Balance`/`Contrast`/`Scale`, blend `Multiply` against the generator layer below — standard technique repeated on both the dirt pass and the (tri-planar-projected) metal-edge-wear pass to avoid the generator's default too-uniform coverage.
15. **Moss/ground-growth layer via the Position generator:** reuse the same dirt material with a desaturated dark-green "moss" color tint; mask built from a `Position` generator (uses baked Position + World Space Normal to infer proximity to the ground) with `Global Invert` toggled to flip growth direction bottom-to-top; broken up further with a `Metal Edge Wear` generator (inverted, `Multiply`) so moss favors protected crevices over open faces, matching real-world moss growth patterns.
16. **Manually art-direct the moss/dirt with a paint layer:** explicitly recommended as a mandatory finishing step, not optional — hand-remove or add dirt/moss/damage based on in-world logic (a frequently-touched door surface gets less grime; a recently-broken-off wood piece shouldn't show old weathering) — called out as one of the most commonly skipped steps that separates procedural-only results from art-directed ones.
17. **Add a warm directional Light generator pass:** new layer, orange/warm tint, `Light` generator with sliders for light direction/angle, `Highlight Glossiness` lowered for a soft top-to-bottom gradient, blend mode `Linear Dodge` kept very subtle (5-10% opacity) to simulate light grazing the top of the object.
18. **Add general grime via an inverted Ambient Occlusion generator:** new dark desaturated-brown layer, `Ambient Occlusion` generator inverted (explicitly not using cavity information — intended as a broad shadow pass, not crevice detail), blend mode `Overlay`.
19. **Hand-paint corner drip/rust stains with a `Blur Directional` filter:** paint a dark color onto select corners only (not all), then apply `Blur Directional` on the mask to streak the paint downward at a controllable angle/intensity, blend `Multiply` — simulates dirt/rust runoff.
20. **Add a Roughness pass on the height-carving fill layer:** enable and raise Roughness slightly on the carving layer so light catches a subtle glossy glint inside the carved crevices specifically.
21. **Hand-paint metal bolts:** dark metallic material (Metallic enabled/maxed), black mask, hard round brush, painted freehand at bolt locations; push the same mask into the `Hide` channel and apply `Bevel Smooth` again for a beveled bolt-head shape; mask can be resized per-bolt at any time since the whole approach stays procedural.
22. **Finishing "secret" trick — thickness-driven simulated subsurface glow:** new bright-yellow fill layer, masked by the baked `Thickness` map run through `Levels` with Invert checked (so thin geometry reads bright), levels pushed further to restrict the effect to only the sharpest/thinnest edges, blend mode `Linear Dodge` at very low opacity — adds a subtle warm edge-glow evocative of light passing through thin wood, without any shader-side subsurface scattering setup.

### Layers / Tools / Settings
- **Bake maps:** `Normal`, `World Space Normal`, `Ambient Occlusion`, `Curvature`, `Position`, `Thickness`; `Auto-Cage` (per-element cage generation, `Match: By mesh name`, `Anti-aliasing: 16x`)
- **Asset source:** in-app `Substance 3D Assets` library (Aged Pine Wood base material, Loose Dirt Scramble dirt material — reused for both dirt and moss passes with recolor)
- **Height-carving filter chain (on the imported Photoshop mask):** `Blur` (light, artifact cleanup) -> `Bevel Smooth` (Distance/Smoothing reduced) -> `Blur Slope` (Intensity Divider raised, blend `Max` for outer-edge-only chip damage)
- **Anchor point mechanic:** folder-level Anchor Point (generated from the whole `Height Layers` group, referencing its `Hide` channel) wired into other layers' generator `Micro Normal` / `Micro Height` / `Micro Detail` settings so generators read into procedurally-carved crevices
- **Generators used:** `Dirt`, `Metal Edge Wear` (used twice: edge-wear pass and moss-crevice-favoring pass, inverted), `Position` (with `Global Invert` for bottom-to-top moss placement), `Light` (direction/angle sliders, `Highlight Glossiness`), `Ambient Occlusion` (inverted, broad shadow pass)
- **Breakup technique (repeated across multiple layers):** `Clouds` filter fill layer, Alt-click mask preview, `Balance`/`Contrast`/`Scale` tuning, `Multiply` against the generator layer it's breaking up
- **Blend modes used throughout:** `Multiply` (darkening, breakup layers, drip stains), `Overlay` (carving burn color, AO grime), `Linear Dodge` (light generator, thickness-glow finish)
- **Filters:** `Blur`, `Bevel Smooth`, `Blur Slope` (Max/Min modes affect outer vs. inner edges), `Blur Directional` (angle-controllable streak/drip effect), `Levels` (Invert, used on Thickness map)
- **External tool:** Photoshop, used to author the carving pattern directly against the door's UV layout, live-linked via Painter's Assets-panel auto-update toggle
- **Finishing "secret" trick:** bright-yellow Fill Layer + baked `Thickness` map (Levels-inverted, pushed to isolate thinnest edges) + `Linear Dodge` at low opacity — simulated subsurface-scattering edge glow with no shader work

### Difficulty
Advanced — assumes comfort with generators, anchor points (including the less-common folder-level anchor point), multi-filter mask chains, and a Photoshop-to-Painter live-linked asset workflow; the payoff (fully non-destructive, art-director-friendly ornamental carving) is a genuinely advanced production technique, not a beginner topic, despite each individual filter being simple to apply.

### App & Version
Version pinned via feature combination, all confirmed on-screen: the `Auto-Cage` baking option (labeled "experimental" in-UI), the Assets-panel automatic-update toggle for linked/modified resources, and the `Bevel Smooth` filter are all first introduced in **Painter 11.0.0** per this skill's own release-notes backfill (`references/release-notes-painter-11.0.md`) — same version floor independently confirmed by the "How to TEXTURE EVERYTHING in Substance Painter" tutorial's Bevel Smooth usage. Likely 11.0.x-11.1.x given no 11.1.0-specific features (e.g. the Ribbon tool) appear on screen.

### Tags
layers, fill-layer, paint-layer, masks, generator, anchor-point, blend-mode, baking, mesh-maps, ambient-occlusion, curvature, thickness, world-space-normal, position-map, high-to-low-poly, cage, udim, texture-set, procedural, tri-planar, alpha, height, roughness, metallic, basecolor, MatFX, advanced

---

## Related Tutorials
- [How to TEXTURE EVERYTHING in Substance Painter](how-to-texture-everything-in-substance-painter.md) — different creator (J Hill); shares the same Bevel Smooth-filter version floor (11.0.0+) and a similar anchor-point-as-single-control-mask philosophy (one anchor referenced by multiple downstream effect layers), applied there to paint chips/leather cracks/decals rather than procedural height carving.
- [SUBSTANCE PAINTER: Building Masks Explained](substance-painter-building-masks-explained.md) — different creator (Jared Chavez); shares the core masking-primitive toolkit (generators, anchor points, tri-planar procedural breakup) applied to a creature mask rather than hard-surface wood carving.
- Cross-link to other Abe Leal 3D tutorials in this knowledge base (`Substance Painter Tutorial: Texturing the Coin`, `Zbrush to Substance Painter Bridge`, `Optimizing Textures - How to Pack Masks Like a Pro`) once ingested — same creator, shared procedural/anchor-point/generator vocabulary expected.
- [Stylized Asset Setup in Painter: Auto-Cage, PSD Workflows & Smart Detailing](stylized-asset-setup-in-painter-auto-cage-psd-workflows-smart-detailing-adobe-su.md) — Adobe-official video confirming the same two 11.0.0 features together (Auto-Cage baking + Bevel Smooth filter), applied there to project foundation-setup and rim ornamentation rather than procedural door carving.
- [Texturing a Cyberpunk Building in Substance 3D Painter – Project Breakdown](texturing-a-cyberpunk-building-in-substance-3d-painter-project-breakdown-adobe-s.md) — same Adobe-official anchor-point-driven engraved-height-to-dirt-mask pattern (Micro Height/Micro Normal referencing), applied there across a whole building's concrete panels instead of a single door.
