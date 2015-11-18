---
layout: post
title: "Low Poly Worlds - a good way to learn Blender and UE4"
excerpt: "Game Development, like any other craft, can get overwhelming very easily. With my \"daytime\" experience as software developer I know, that the best way to learn new things is to break them down to the most simple working prototype. Why? Because you need to learn the **fundamental concepts** and get a clue about a **possible workflow pipeline** first."
date: 2015-11-18 14:34:00
categories: articles
tags: [ue4,lowpoly,blender]
image:
  feature: lowpoly-trees-scene1.jpg
comments: true
share: true
---

## Low Poly Worlds – a good way to start learning

After my[ first steps inside Unreal Engine 4][1], I really wanted to start building my stuff! No standard assets or marketplace downloads&nbsp;just to have something to use. I would like to learn to build&nbsp;_my very own creations_.&nbsp;As coder (read: non-designer) the art style '[Low Poly][2]' is my&nbsp;possibility to create something on my own which still has the chance to look nice ;-)

![Low Poly Tree Scene][3]

This scene has only two different meshes.

&nbsp;

## **So what's the 'pipeline' I was writing about?**

To get my first basic scene in UE4 with self-made static meshes, I had to learn more about these topics:

* 3D Software (Blender)
* Sculpting Basic Models
* UV map and UV unwrapping
* Lightmap
* FBX Exporter
* Import meshes into Unreal Engine 4
* Base Material and Material Instances
* Blueprints to build new objects out of different static meshes to have some variation
* (Having fun!)

Overwhelming? Yes, indeed. I am going to break it down and link to the resources which got me started.

## 3D Software

While you can use your Gaming Engine to block out your levels with brushes or simple pre-made geometric objects, you really have to look into a 3D software to build your own objects (meshes). The big players on the market are software suits like [3D Max][4], [Maya][5]&nbsp;and [ZBrush][6]. But the licenses are rather expensive and nothing to "play around with". So my choice for now is&nbsp;[Blender][7], which is completely free to use!

[Download Blender][8] and build something!

## Sculpting&nbsp;Basic Models

![blender-lowpoly-baum-grid][9]Blender doesn't make it easy to start with. My first steps took ages with a lot of head scratching. To build my first tree out of an icosphere and a cylinder I used the wonderful [Secrets to Creating Low Poly Illustrations in Blender][10]&nbsp;tutorial. You get a step by step example with all the Blender keys and commands needed. But take your time. Better be slow with proper understanding and memorizing the steps for future usage!

## UV map and UV unwrapping

UV what? [Wikipedia][11]:

&gt; &nbsp;**UV mapping** is the 3D modeling process of making a 2D image representation of a 3D model's surface.

To place materials, colors, textures onto a 3D model, you have to build a UV map. The process of creating the 2D surface map is called "UV unwrapping". There are a lot of tutorials about this topic on the web, because the better your unwrapping is, the better your model will look in the end. As for my basic models I was able to use the built-in unwrap tool to place everything.

A big help was this blog post about [Basic UV Mapping in Blender][12]. Really worth&nbsp;the&nbsp;read!

![blender-lowpoly-baum-uvunwrap][13]

## Lightmap

![lightbulb][14]The Lightmap is technically a second UV Map. The Unreal Engine needs it to bake lightning information onto the model. You can have UE4 create the&nbsp;Lightmap on its own while importing the mesh but each source I read recommends&nbsp;to build your own on a second UV Map channel. Even with these simple meshes I had quirky outcomes with the automatic lightmap creator in UE4. To understand the problems and why something happens,&nbsp;these&nbsp;lightmapping basics are a lifesaver:

[18 Important Principles for Creating/Using Lightmaps][15]

(UDK infos are still valid for UE4)

## FBX Exporter and&nbsp;Import meshes into UE4

![fbx-import][16]Now we are getting closer to actually using our models withing the Game Engine *cheer*. UE4 can import 3D Objects with the FXB format and Epic Games was involved in the development of the newest fbx exporter inside Blender. The first thing to learn is, that both programms have different units / scales. Without any changes in Blender, you have to export your model with a scale of 100x to get the same result inside Unreal Engine 4.

These two posts kicked me in the right direction to get my meshes inside UE4:

[Static Mesh from Blender][17]&nbsp;(UE4 Wiki)

[Get From Blender to Unreal][18]&nbsp;(ROW&nbsp;VR Blog)

&nbsp;

![sm-tree-ue4][19]The process is straight forward. All thought I have attached materials to the Blender object, I don't import them. The material creation inside UE4 is way better with PBR (Physical Based Rendering). If you use more than one material, UE4 will create corresponding material nodes inside the object. Very handy!

If you created your own lightmap, be sure to deselect the "Generate Lightmap UV's" switch while importing. Otherwise you end up with 3 UV maps ;-)

## Base Material and Material Instances

After watching the&nbsp;[Introduction to Materials in UE4][20]&nbsp;(official UE4 Videos) playlist, I have a basic understanding of the Physical Based Rendering System. The last three videos are about Material Instances, which I used in my scene. I created just a basic material with parameter values instead of static values. This way I am able to instantiate it and just switch the color (e.g. via Blueprint). Want to try a new look? Just change the Base Material and your whole scene will change.

![material-editor][21]

## Blueprints

To build new objects out of different static meshes, I use Blueprints (BP) to have some variation and inheritance possibilities. With BP's you can change all actors with this BP in your scene at the same time. Further more you will be able to manipulate these actors with scripts later on.

![bp-editor][22]

## Having fun!

That's it for today.&nbsp;I made the first and rather long step,&nbsp;made something on my own and got it out of Blender into Unreal Engine 4. From this point on I can add more actors, different lightning, new meshes and so on and so forth. It is an important step to see your&nbsp;own progress and now I can adapt, change, play with it and continue learning.

![LowPoly Trees][23]

My first Low Poly Tree with some glossy fun ^^;

PS: If you wonder about the filenames of my assets, I try to follow the&nbsp;[Unreal Engine 4: Naming Convention][24] by [@t_looman][25]&nbsp;(Twitter).

If you like to know more about UE4 Development, I would like to recommend my post: [5 Sites every UE4 Beginner should know][26]

&nbsp;

## You have Successfully Subscribed!

[1]: http://nerd-time.com/howto-ue4-firstlesson/ "How to start with Unreal Engine 4 – my first session"
[2]: https://www.pinterest.com/CalaelenCom/low-poly-art/ "Low Poly Art on my Pinterest Board"
[3]: http://nerd-time.com/wp-content/uploads/2015/04/lowpoly-trees-scene1-1024x607.jpg
[4]: http://www.autodesk.de/products/3ds-max/overview
[5]: http://www.autodesk.com/products/maya/overview
[6]: http://pixologic.com/
[7]: http://www.blender.org
[8]: http://www.blender.org/download/
[9]: http://nerd-time.com/wp-content/uploads/2015/04/blender-lowpoly-baum-grid-150x150.jpg
[10]: http://cgi.tutsplus.com/tutorials/secrets-to-creating-low-poly-illustrations-in-blender--cg-31770
[11]: http://en.wikipedia.org/wiki/UV_mapping
[12]: http://rowvr.co/2015/01/03/basic-uv-mapping-in-blender/
[13]: http://nerd-time.com/wp-content/uploads/2015/04/blender-lowpoly-baum-uvunwrap-e1429187347686.jpg
[14]: http://nerd-time.com/wp-content/uploads/2015/04/lightbulb.jpg
[15]: http://www.worldofleveldesign.com/categories/udk/udk-lightmaps-01-basics-and-important-principles-for-creating-using-lightmaps.php
[16]: http://nerd-time.com/wp-content/uploads/2015/04/fbx-import-182x300.jpg
[17]: https://wiki.unrealengine.com/Static_Mesh_from_Blender
[18]: http://rowvr.co/2015/01/03/get-from-blender-to-unreal-engine-4-quick-workflow-tips/
[19]: http://nerd-time.com/wp-content/uploads/2015/04/sm-tree-ue4.jpg
[20]: https://www.youtube.com/watch?v=lngF4VVNER4&amp;list=PLZlv_N0_O1gbQjgY0nDwZNYe_N8IcYWS-
[21]: http://nerd-time.com/wp-content/uploads/2015/04/material-editor.jpg
[22]: http://nerd-time.com/wp-content/uploads/2015/04/bp-editor.jpg
[23]: http://nerd-time.com/wp-content/uploads/2015/04/lowpoly-trees-banner-980x415.jpg
[24]: http://www.tomlooman.com/ue4-naming-convention/
[25]: https://twitter.com/t_looman
[26]: http://nerd-time.com/ue4-beginner-resources/ "5 Sites every UE4 Beginner should know"
 
