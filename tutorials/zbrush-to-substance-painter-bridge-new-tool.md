---
title: Zbrush to Substance Painter Bridge! NEW TOOL!
source: YouTube
url: https://www.youtube.com/watch?v=KzoJkdqyn7E
author: Abe Leal 3D
ingested: 2026-08-13
app: "Substance 3D Painter (receiving end) + ZBrush 2026.2 (sending end, via the ZBrush-to-Substance Bridge plugin)"
version: "ZBrush 2026.2 confirmed on screen; Painter version not stated (both apps must be updated to their latest version for the Bridge to work)"
tags: [baking, mesh-maps, high-to-low-poly, cage, id-map, udim, texture-set, uv, masks, ambient-occlusion, world-space-normal, curvature, thickness, height, normal-map, opacity, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/zbrush-to-substance-painter-bridge-new-tool/
frame_count: 10
frame_status: complete
frame_selection: content-anchored (manual timestamps chosen from transcript, not blind percentages)
---

# Zbrush to Substance Painter Bridge! NEW TOOL!

**Source:** [YouTube](https://www.youtube.com/watch?v=KzoJkdqyn7E)
**Author:** Abe Leal 3D
**Duration:** 15m42s | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frames captured — see "Captured Frames" section below.


### Full Content [0:00]
**Transcript (timestamped):**
[0:00] Hello everyone and welcome to this video here in the channel today. We're showcasing a very cool new tool that we have with Seabrush and Substance.
[0:06] This is of course the Seabrush to Substance Bridge. They gave us a sneak peek during GDC and now it's here.
[0:12] With this very cool tool, you're gonna be able to just click a button and send your object from Seabrush to Substance and of course go through the full texturing pipeline so that you can create amazing assets.
[0:23] There is a little bit of setup involved so let's go through some of the tools and things that you need to be aware of before you use this tool. Let's go.
[0:31] So we're inside Seabrush 2026.2 my friends and I made a little thing here for you guys. So this is just this model birdhouse my wife loves birds.
[0:40] So I wanted to, you know, do something that she might actually relate to and yeah, we did this thing right here.
[0:46] Now the way we're going to be working with the transfer to Substance does require a specific setup and this my friends is the low poly high poly setup.
[0:54] So as you can see right here, if I go to my geometry tab, you're going to see that I have a single sub tool just this birdhouse right here and every single plank piece and element is inside the sub.
[1:05] This is very important. You're going to see why in just a second. In this lowest subdivision of the element, we need to have UVs.
[1:13] There is an option and we're going to take a look at that in just a second. But by default, you're probably going to be working with UVs.
[1:17] You can make the UVs here inside of Seabrush with something like UV Master, for instance, but in this particular case, I actually went into RISM and did the UVs.
[1:25] So this is my UVs right here. So as you can see, everything is, you know, fairly well organized.
[1:31] I have a good sort of like a distribution of the elements and I have also of course my high poly right here.
[1:37] So if I go to my sixth subdivision level, I'm at all the way to 11.73 million polygons and I added, you know, just a little bit of detail damage and everything.
[1:45] Now, if we go to texture and we go down here, boom, we're going to have our texture bridge right here.
[1:50] I'm just going to dock this to the side. There you go.
[1:53] And as you can see, we have a couple of options here. First of all, everyone wants to click the button.
[1:57] That's fine. But we're going to just take a look at these things right here.
[1:59] What do we want to send in this particular case? Of course, it's just going to be all.
[2:02] It's just a single sub tool. And we're going to go here to where it says subdivision levels and make sure that this is set to low and high.
[2:08] What this button will do is it will automatically detect that the lowest subdivision is your low and your highest subdivision is of course your high.
[2:15] And you don't need to rename. You don't need to do anything. Everything leaves within one sub tool.
[2:19] Again, this is very important. And that's pretty much it.
[2:22] Texture set. As you can see, we're going to create one texture set for this sub tool.
[2:25] We could change this to per poly group. It's going to make it a mess.
[2:27] So in this case, I just want to do per sub tool and just click send to paint.
[2:30] Once I do this, substance manager is going to update. Of course, you need to have both seabrush and substance manager like updated to the latest version.
[2:37] And we just need to give substance a little bit of time to do the whole thing.
[2:40] So just let it load. And what this is going to do is it's going to include or import your low poly, import your high poly.
[2:46] And it's actually going to do the bakes by itself as well, because there's an option.
[2:50] I'm going to show you in just a second, instead of seabrush, where you can enable auto bakes.
[2:53] So that's it. No further input needed from you.
[2:56] You can go and get a cup of coffee or just wait a couple of seconds.
[2:59] And there we go. As you can see, even without this thing, let's close it.
[3:02] The bakes are happening already and we are good to go.
[3:05] Everything is already set up for you. So as you can see by default, it's going to be doing it at 2K.
[3:10] It's going to be using the automatic cage feature.
[3:12] You can see that it's using this seabrush template on the top.
[3:14] So there's going to be a couple of changes on the basic substance interface.
[3:18] But yeah, that's pretty much it. If you want to like re-bake this or do this again, you are free to do so.
[3:23] For instance, here, I probably want to push this, let's say to two by two.
[3:26] And I can change this to 4K as well to make sure that we get some really nice bakes.
[3:30] As you can see, this thing right here is saving the file, the high poly, into a temporary folder.
[3:35] That's very, very important. We are not going to be able to use the by mesh name, of course,
[3:39] because as you can see, even though we have matching by name, it's just one low poly and
[3:43] white high poly. It's not grabbing every specific planks.
[3:45] And again, you can just like hit bake again if we didn't like something from the first one and
[3:49] wait for this to finish.
[3:51] So if you like the content here on the channel, my friends, please leave us a like, share,
[3:54] subscribe. It really helps. We're really close to our next milestone.
[3:57] I didn't think we were going to get as close to 100K as we are now, but with your help, we can get that
[4:02] very, very soon. Let's continue. That's it. With that done, as you can see right here,
[4:06] our little birdhouse is ready. We are ready to jump into the texturing department and start
[4:10] like texturing everything that we need. But that's not all about the plugin. Let me show you.
[4:15] If we go back to Siebers, there's a couple of things that I know people are going to be asking
[4:18] about. And the first question that I had was, can we do UDems? And I'm not sure if this is intended
[4:23] or not, but you can actually do UDems. So again, if we go to the lowest subdivision and we morph
[4:28] this UB, you're going to see that we have this like single texture set UVs here for my element.
[4:32] What I'm going to do is I'm going to go to the top right here and I'm going to import and I have
[4:36] this little one right here called low test. I'm just going to say open. And what I just did right
[4:40] there is I'm replacing the low poly or the first level of subdivision with the new UVs that I have.
[4:47] This is very important. If you're going to be updating or changing your UVs, you do not change
[4:51] anything. Not a single vertex needs to move. No scale, no movement, no nothing. The only thing
[4:56] that you can change is UVs because if you change anything, the data is going to get mixed up.
[5:02] And when you try to import the OBJ back, it's not going to match anymore. You're going to know if
[5:05] you're doing this properly when you try to import the lowest level of your object and it gives you
[5:09] no warning. If it says that it wants to reproject all of the details, you made something like you
[5:13] change something and it's going to like make a mess. So in this particular case, as you can see,
[5:18] if I morph the UVs, all of the UVs are overlapped into each other because I'm actually using four
[5:23] units right here. Let me close substance real quick. And what I'm going to do is the same process.
[5:28] I'm just going to go to my little new substance rich right here and make sure that I'm sending
[5:32] all first up to subdivision level low and high. That's it. And I was going to say send to picture.
[5:37] The same process is going to happen here. I'm not going to bore you guys with like the whole thing.
[5:40] It's going to take a couple more minutes because now we're of course baking four units instead of
[5:44] one single one. It is going to be baking them at 4k. But yeah, that's pretty much it. And that's
[5:49] it. As you can see up here, we actually have four UV tiles. If we go to our paint layer right here,
[5:54] we're going to get this thing. So to me, it seems like you've been scanned indeed work
[5:58] instead of this new bridge. And again, we get a nice result. Last thing that I want to show you
[6:02] here, let's close this up since again, if we go back here and we delete the UVs, I'm going to say
[6:08] delete UVs right here. So now my element has absolutely no UVs. This is something you're
[6:12] probably only going to be using if you want like a quick render or like a quick texture,
[6:15] like it's not something that I would recommend you do or like actual production work, but it's
[6:19] going to be a good way to get something fast. And that's the fact that you can select this option
[6:23] that says force UV auto unwrap. When we do that, and we send that to paint, what's going to happen
[6:29] now is a substance painter, it's going to do it's little magic, and it's going to use the other UV
[6:33] options that it has to generate a bake. The more complex the object, the more like wonky your
[6:38] UVs might look, but you're going to see in just a second that the UVs that we get is actually
[6:42] not that bad, especially for this relatively simple asset that everything's very sort of like
[6:45] blocky. It should give us a relatively good result. So if we check the UVs on this thing right here,
[6:50] you're going to see that we get this. Now, interestingly enough, it's sort of like recognize
[6:54] that I want to have four UDEMs. I don't think it should have if it originally was just one UV,
[6:59] it should understand it's just one UV. But as you can see, we get this artist like perfect UVs,
[7:03] of course not. As you can see, we got like cuts and weird stuff all over the place. However,
[7:08] they did announce that on the new beta version of Substance, there are going to be some new
[7:12] improvements to the other UV functions that's going to try to help with this or like hard surface
[7:16] stuff. But even then you can see like, since all of this is being projected into the 3D mesh,
[7:20] you don't really see that much of an issue. So there you go. If you don't want to do UVs because
[7:24] you are lazy or you want to save a little bit of time there, or just want to get like a quick
[7:28] texture, not being lazy, it's just being efficient, right, to just quickly present something. Well,
[7:32] this is definitely going to be one option for you. Last but not least on the final options here
[7:37] that I want to show you is this, Send Polypane. So first thing I'm going to remove that stuff
[7:42] right there. Let's go back to the lowest subdivision level, import our single UV here. Again, we can
[7:47] quickly check. As you can see, that's just our single UV right there. And what I'm going to do
[7:51] is I'm going to go to the highest subdivision level, go to my paint brush right here. And let's
[7:56] just do a quick thing right here. I'm just going to go completely white. Actually, let's do something
[8:01] a little bit more fun. Let's say you wanted to create an ID mask and we want to use polypane
[8:04] for that. So one thing I can do is I can check my polygroups. And as you can see,
[8:08] every single element has a different polygroup. Then I can go to polypane. I'm just going to
[8:12] say polypane from polygroups. And what that will do, as you can see, is now every single mesh will
[8:17] have a slightly different color, slightly different element. So this has polypane information.
[8:21] I'm going to do the exact same thing, but I'm going to keep this Send Polypane option on and
[8:26] we send to painter. As you can see, painter is loading everything and he's going to be baking
[8:30] all of the information. Now, the interesting thing right here is that if we go here to our little
[8:36] element, boom, we get this. What is happening right here? Well, what is happening is this is
[8:40] not actually an ID map. This is just a polypane layer. What this thing is doing is creating a
[8:46] new paint layer and just filling in it with a texture that we should be able to find over here.
[8:51] There you go. So birdhouse single UV base color. So it just like bakes that information into the
[8:56] UV. And now we can use it that cool thing again, as I mentioned, is we can go here to the texture
[9:00] set settings and just drag and drop that into, for instance, our ID map right there. So now we
[9:06] can actually delete this thing right here. And let's say, we want to add like a very basic bark
[9:10] pine material only to the top layers. Of course, we could use like a mesh selection. But if we go
[9:15] here and add a black mask, and then add a color selection, we can just pick the colors and start
[9:22] picking all of this little guys right here. So very handy. Or if you like using polypane to
[9:26] actually like paint your character, and you want to import that information to use as a base layer,
[9:30] maybe you're doing hand painted or something like that. Well, that option is very, very useful.
[9:34] Pretty sure that's it for the main stuff right here. We did the substance rich. There's just two
[9:39] more things that I want to talk about. First, this subdivision level option. This is the current
[9:43] option. And this is the low high. Let's imagine we don't have a high version. So what I'm going to do
[9:48] here is I'm going to clone this element right here. Let's get rid of the polypane. We don't need
[9:52] it for now. And let's imagine for whatever reason, we don't have a low policy, I'm going to delete
[9:56] lower. We did not do like proper retopology or whatever. This is just the high poly, but we
[10:00] do have UV so this thing has the like the normal UVs. One of the things that we can do for instance,
[10:05] is we can go here to see plugging, we're going to use decimation master, keep UVs very important.
[10:11] And let's decimate this all the way down to 250k. So what this is going to do is it's going to grab
[10:17] this high poly and just convert it into a decimated version, right, like minimize the amount of
[10:21] triangles that we have while keeping or trying to keep the UVs as best as possible. Once we have
[10:26] that, we can take this into substance and texture directly the triangulated mesh. Is this something
[10:31] that you're going to use for production? Absolutely not. Maybe we are going to be doing something
[10:35] like nanite or things like that, some rocks and some other elements might work in that specific
[10:39] thing. But usually this is something that you might just want to do again, for a quick test,
[10:43] a quick like beauty render, like maybe some like a page or whatever. So it is just an option. It
[10:48] doesn't mean it's going to be an option that you're going to be using all the time, but it
[10:51] is an option. And the only thing that's going to change with this element is that instead of using
[10:54] a low and high, because we don't have a low and high, it's just like the single subdivision level,
[10:59] we need to change this to current and it's going to export the object exactly as it is,
[11:02] bring it into substance with the UVs that in this case would be heritant from the other mesh.
[11:07] And that's it. If you don't have UVs, we could just like let the auto bake function do its job
[11:11] and work with that. Let me wait for this to finish and I'll show this inside of substance.
[11:15] There we go. So as you can see right here, my friends, this thing is now very, very low poly,
[11:20] very, very decimated. And we can actually go here to the UV map and morph this into the UV.
[11:25] And you're going to see that all of the pieces are being well respected, right? Like we have the
[11:28] exact same thing or as best as possible with the exact same thing. I'm going to make sure that we
[11:33] don't want the other unwrap change this to current and just say send to painter. Now in this case,
[11:39] even though we don't have a low and high poly, you still need to do the bakes. I've talked about
[11:44] this extensively when we're doing texturing. Even if you don't have a high poly and a low poly,
[11:49] you still benefit a lot from doing the bakes because you're still going to get information
[11:52] like ambient occlusion, world position, world normals. Like there's a lot of information that
[11:57] the generators instead of substance are going to be using and you do want to be doing that.
[12:01] So I'm going to go here to the bakes and it did not do an auto bake. I'm guessing because it did
[12:05] not find the low poly, high poly, but you can still use this use low poly mesh as high poly
[12:09] and do your own bakes. And there we go. Of course, we're not going to have the exact same detail
[12:13] because this is like a decimated version, but you can still work with this. Like if you want to
[12:16] again, throw in some materials and just start like working and giving a quick texture to this
[12:20] thing, it is possible. Is this something that I'm personally going to be using a lot? Not really,
[12:24] but it's a good tool to have. Last but not least, and this is a little bit more of a technical
[12:28] thing, but I think it's quite, quite interesting. First of all, if we go here to texture sets,
[12:32] as you can see, because we're working with a single element, a single texture set,
[12:36] right now what's going to happen is all of the UMM apps is going to be in one single texture.
[12:40] If I were to change this to per poly group, what's going to happen is each one of this is going to
[12:44] be separated into a different element. But because they're sharing the same UV space,
[12:49] I find that to be quite wasteful because you're going to have tons and tons and tons of textures
[12:53] and it's not going to be possible. But there is a good thing or a good like process that we could
[12:57] use for this. So what I'm going to do here is I'm going to start isolating all of the different
[13:01] poly groups right here. Let's group this whole thing as a single one like that. And let's take
[13:08] all of this side panels out as well. Let's do the back one as well. Control W for that one as well.
[13:15] So as you can see now, we're still in a single sub tool, right? But we have three poly groups
[13:19] right here. If I keep this as per poly group, and I send this to painter again, we're using the
[13:25] we're now going to use the low to high, of course, because we want to use this one right here.
[13:29] When I send this to painter, what's going to happen is that we are now going to get
[13:33] three UV sets. Why could this be useful? If you want to have a little bit more control of which
[13:38] tools you turn on and off and just like keep them separate, even though they share the same UV,
[13:43] this could potentially be one of them. My personal recommendation is that if you're using UDEMS,
[13:48] or if you're going to have multiple sub tools, you pack everything properly so that you don't
[13:52] have to be wasting that much of UV space. But it's good to have the option to use poly groups as a
[13:56] sort of way to group the different UVs to get, again, more options. So there you go. As you can
[14:01] see, there's going to be again a couple of options or a couple of advantages of doing this. But in
[14:06] terms of the UV elements, because they all were sharing the same UV set, as you can see, yes,
[14:10] there's going to be a lot of wasted space. So we do split them into multiple parts. So that should
[14:15] allow us to work on specific elements a little bit more comfortably. But in the end, like you're
[14:20] probably going to want to merge all of this into a single texture so that you're not wasting that
[14:23] much space. Or in another option, go into your DCC application or intuosism and just group all of
[14:29] the things that are going to be in the same poly group so that they are part of the same scene.
[14:33] So this is it, my friends. This is the new Substance Bridge from Seabrush. I think it's
[14:38] going to be a really, really cool tool. If you plan things ahead, if you're using the traditional
[14:43] low poly, high poly, like subdivision method approaching Seabrush, this should be fairly,
[14:47] fairly easy to integrate into your workflow. However, keep in mind, you do need to have
[14:51] clean UVs. You do need to have those things, the low poly and the high poly. So there's a little bit
[14:55] of setup required, not just like a one click solution, if you want to keep things clean for a
[15:00] specific pipeline. But if you want to do like some quick texturing, because you really like the
[15:04] sculptor that you have so far, as you saw during the video, you can also just decimate the whole
[15:08] thing, do automatic UVs, do UV Master. It just opens up so many possibilities. I'm really enjoying
[15:14] this tool so far. I think it's a really, really great addition to both packages. Do make sure to
[15:18] have both of them updated to the latest version. And yeah, let's see how else they're going to
[15:22] be improving these new tools in the upcoming months. That's pretty much it for today, my friends.
[15:26] Don't forget to subscribe. We're really close to the next milestone here at the channel. And,
[15:30] as we always say, always learning, always improving. I'll see you back on the next one, my friends. Bye.



---

## Captured Frames

- [1:00] tutorials/frames/zbrush-to-substance-painter-bridge-new-tool/frame_000.jpg
- [1:55] tutorials/frames/zbrush-to-substance-painter-bridge-new-tool/frame_001.jpg
- [3:05] tutorials/frames/zbrush-to-substance-painter-bridge-new-tool/frame_002.jpg
- [5:55] tutorials/frames/zbrush-to-substance-painter-bridge-new-tool/frame_003.jpg
- [7:00] tutorials/frames/zbrush-to-substance-painter-bridge-new-tool/frame_004.jpg
- [8:40] tutorials/frames/zbrush-to-substance-painter-bridge-new-tool/frame_005.jpg
- [9:05] tutorials/frames/zbrush-to-substance-painter-bridge-new-tool/frame_006.jpg
- [10:10] tutorials/frames/zbrush-to-substance-painter-bridge-new-tool/frame_007.jpg
- [11:20] tutorials/frames/zbrush-to-substance-painter-bridge-new-tool/frame_008.jpg
- [13:20] tutorials/frames/zbrush-to-substance-painter-bridge-new-tool/frame_009.jpg

---

## Structured Notes

### Core Technique
Demo of the (then-new) **ZBrush-to-Substance Painter Bridge** plugin — a one-click send that replaces the traditional manual export/import-and-manually-configure-baking pipeline: ZBrush automatically detects a sub-tool's lowest subdivision level as the low-poly and highest as the high-poly, sends both into a freshly configured Painter project, and (optionally) triggers the mesh-map bake automatically, with no manual Baking dialog setup required on the Painter side.

### Summary
Required ZBrush-side setup: a single sub-tool containing every mesh piece (all planks/elements of the demo birdhouse asset live in one sub-tool, not separate ones), UVs present on the **lowest subdivision level** (authored here in RizomUV, though ZBrush's own UV Master works too), and sculpted detail built up through subdivision levels (up to 11.73M polygons on the highest level in this demo). The **Substance Bridge** panel (Tool → Substance Bridge, dockable) exposes: **Subdivision Levels** (Low & High — auto-detects lowest/highest sub-tool subdivision as low-poly/high-poly respectively, no manual renaming needed), **Texture Sets** (Per SubTool = one texture set for everything vs. Per PolyGroup = a separate texture set per poly group — the latter warned against by default since it wastes UV space when groups share the same UV layout), **Send PolyPaint**, **Smooth Normals**, **Auto-Bake Maps** (bakes mesh maps automatically on arrival in Painter, no manual Baking-dialog trip needed), **Force UV Auto-Unwrap**, and the **Send to Painter** button itself. On arrival, Painter auto-configures using a ZBrush-specific project template, sets bake resolution to 2K by default (adjustable, e.g. up to 4K), uses the **Automatic Cage** feature, saves the high-poly mesh to a temporary folder (meaning **Match by mesh name** cannot be used for this kind of single-combined-sub-tool send — bakes rely on the whole low mesh vs. whole high mesh, not per-part name matching), and mesh maps can be freely re-baked from within Painter afterward at a different resolution if needed. **UDIM support**: confirmed working (though possibly not an officially-designed feature) — replacing the low-poly's UV layout with a 4-UDIM-tile version and resending produces a Painter project with genuine multi-UV-Tile texture sets; the only hard rule when swapping UVs is that **no vertex may move, scale, or change** between sends — only UV coordinates — otherwise Painter's OBJ-vs-OBJ matching breaks and it will demand to reproject all sculpted detail (a visible warning at import time is the tell that something besides UVs changed). **Force UV Auto-Unwrap**: an option for skipping UV authoring entirely for quick tests/renders (not recommended for production) — Painter's own auto-unwrap generates a workable but visually rough UV layout (visible cuts/seams in the 2D UV view) that reads acceptably in the 3D viewport for a blocky asset like this; Adobe has stated further auto-unwrap improvements, particularly for hard-surface content, are coming in a Painter beta. **Send PolyPaint**: bakes ZBrush PolyPaint color data (demoed here from **Polygroups from PolyGroups**, giving each mesh element a distinct flat color) directly into Painter as a new Paint layer holding a baked texture resource (named `<object>_SingleUV_BaseColor` or similar) — the resulting texture can then be **dragged from the Assets panel directly into the Texture Set Settings' ID map slot**, after which a normal `Add Mask with Color Selection` mask (right-click a layer's mask → Color Selection, pick a polygroup's color) works exactly like a baked ZBrush-PolyPaint-to-ID-map workflow, letting you mask individual mesh parts (e.g. isolating just the roof planks for a bark/pine material) without a separate dedicated ID-map bake pass. **Subdivision Level = Current** (instead of Low & High): for sub-tools that only have one subdivision level (e.g. after using ZBrush's **Decimation Master** with Keep UVs enabled to convert a high-poly-only asset into a UV-preserving decimated low-poly, useful for quick renders/tests, not recommended for production unless targeting something like Nanite) — sends the mesh as-is with its own inherited UVs; since there's no separate high-poly reference, Auto-Bake does not fire automatically, but a manual bake ("use low poly mesh as high poly mesh") is still strongly recommended even without true high-to-low detail transfer, since baking still produces AO/world-position/world-normal data that Painter's generators depend on. **Per-PolyGroup texture sets**: isolating parts into distinct poly groups (e.g. roof separated from walls/base) before sending with Texture Sets = Per PolyGroup produces multiple independent UV sets/texture sets in Painter sharing the same underlying UV space — useful for toggling/isolating specific parts' work independently, but wastes UV space if the parts share UV real estate; the creator's general recommendation is to properly UV-pack everything (or group elements together in the DCC app) rather than rely on this split for production.

### Key Steps
1. ZBrush-side prerequisites: keep every mesh piece inside **one sub-tool**; author UVs on the **lowest subdivision level** (RizomUV, UV Master, or any UV tool); build detail up through higher subdivision levels normally.
2. Open the **Substance Bridge** panel (Texture tab in ZBrush), set **Subdivision Levels = Low & High** (auto-detects lowest/highest sub-tool subdivision — no manual renaming of anything required, since everything lives in one sub-tool).
3. Set **Texture Sets = Per SubTool** for one combined texture set (recommended default; Per PolyGroup fragments into many texture sets sharing the same UV space, which is wasteful).
4. Click **Send to Painter** — Substance/Painter needs a moment to import the low-poly, import the high-poly, and (if **Auto-Bake Maps** is enabled) run the mesh-map bake automatically with no manual Baking-dialog setup.
5. In Painter, adjust bake resolution afterward if needed (default 2K, bump to 4K etc.) and re-bake — note the high-poly was saved to a temporary folder by the Bridge, so **Match by mesh name** isn't applicable here (it's a whole-low-vs-whole-high match, not per-part).
6. For UDIMs: replace the low-poly subdivision level's UVs with a multi-tile UV layout (Import a new OBJ at that subdivision level) — the only permitted change is UV coordinates; **no vertex may move, scale, or shift**, or Painter's OBJ matching breaks and it will prompt to reproject all detail (a clean re-send shows no such warning).
7. For quick/non-production texturing with no UVs at all: delete the sub-tool's UVs, enable **Force UV Auto-Unwrap** in the Bridge panel, and send — Painter auto-generates a workable (if visually rough, seam-heavy) UV layout suitable for blocky/simple assets.
8. For an ID-map-style masking workflow without a dedicated ID bake: in ZBrush, generate **Polygroups from PolyGroups** (or paint PolyPaint directly for hand-painted base work), enable **Send PolyPaint** in the Bridge panel, and send — Painter receives the PolyPaint data as a baked texture inside a new Paint layer.
9. Drag that baked PolyPaint texture from the Assets panel directly into **Texture Set Settings' ID map slot**, then use standard `Add Mask with Color Selection` (right-click a mask → Color Selection, pick a polygroup color) to mask individual parts — equivalent to a full ZBrush-PolyPaint-to-ID-map export/bake pipeline, done inline.
10. For a high-poly-only asset with no true low-poly: use ZBrush's **Decimation Master** (with **Keep UVs** enabled) to generate a UV-preserving decimated version, set the Bridge's **Subdivision Level = Current** (not Low & High, since there's only one level now), and send — inherits UVs from the original mesh.
11. Even without a true high-to-low-poly relationship, still run a manual bake ("use low poly mesh as high poly mesh") in Painter — worthwhile for the AO/world-position/world-normal data Painter's generators depend on, even without real detail transfer.
12. For independently-toggleable per-part texture sets sharing one UV layout: isolate mesh parts into separate ZBrush poly groups before sending with **Texture Sets = Per PolyGroup** — produces multiple UV sets/texture sets in Painter; generally recommended only for quick iteration, not production (properly UV-pack or DCC-side-group elements instead, to avoid wasted UV space).

### Layers / Tools / Settings
- ZBrush **Substance Bridge** panel: Subdivision Levels (Low & High / Current), Texture Sets (Per SubTool / Per PolyGroup), Send PolyPaint, Smooth Normals, Auto-Bake Maps, Force UV Auto-Unwrap, Send to Painter
- Painter Baking: **Automatic Cage**, ZBrush-specific project template, resolution (2K default, adjustable), `Match by mesh name` not applicable to Bridge-sent single-combined-mesh sends
- `UV Tiles` (UDIM) support confirmed working via the Bridge
- `Add Mask with Color Selection` fed by a Bridge-sent **PolyPaint** texture dragged into the **ID map** slot in Texture Set Settings
- ZBrush **Decimation Master** (Keep UVs) for a UV-preserving high-to-low conversion when no true low-poly exists

### Difficulty
Intermediate — mostly plugin/UI operation, but requires understanding of the underlying low/high-poly-baking and UDIM/UV concepts to use correctly (matching-vertex rule when swapping UVs, why Match-by-mesh-name doesn't apply here, why baking still matters without a true high-poly).

### App & Version
ZBrush 2026.2 confirmed on screen; Substance 3D Painter version not stated (both apps explicitly required to be updated to their latest version for the Bridge to function).

### Tags
`baking` `mesh-maps` `high-to-low-poly` `cage` `id-map` `udim` `texture-set` `uv` `masks` `ambient-occlusion` `world-space-normal` `curvature` `thickness` `height` `normal-map` `opacity` `intermediate`

---

## Related Tutorials
- [Preparing Models for Substance 3D Painter in Blender](preparing-models-for-substance-3d-painter-in-blender-adobe-substance-3d.md) / [...in Maya](preparing-models-for-substance-3d-painter-in-maya-adobe-substance-3d.md) / [...in 3DS Max](preparing-models-for-substance-3d-painter-in-3ds-max-adobe-substance-3d.md) — same underlying concepts (Texture Sets, ID Maps, geometry-to-Painter handoff) explained for other DCC apps' manual export/import pipelines, which this ZBrush Bridge plugin automates end-to-end.
- [Substance Painter Tutorial: Texturing the Coin](substance-painter-tutorial-texturing-the-coin.md) — different creator (Abe Leal 3D); a small-prop baking-and-masking pipeline sharing this video's creator, useful for comparing manual vs. Bridge-automated baking setup.
- [Complex Wooden Medieval Door Tutorial in Substance 3D Painter](complex-wooden-medieval-door-tutorial-in-substance-3d-painter.md) — same creator (Abe Leal 3D); a multi-UDIM production project using the traditional manual Auto-Cage baking pipeline this Bridge plugin is designed to streamline.
