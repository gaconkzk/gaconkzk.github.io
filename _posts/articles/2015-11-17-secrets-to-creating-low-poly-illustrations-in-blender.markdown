---
layout: post
title:  "Secrets to Creating Low Poly Illustrations in Blender"
excerpt: "Low poly style illustrations are a hot trend these days and we see them everywhere – books, animations, music videos, apps, etc. and today you'll learn how to create one in Blender. This tutorial will focus more on how to achieve the style, rather than learning illustration theory or modeling anything in particular. We will create one example illustration and learn the steps to achieve the desired result."
date:   2015-11-17 00:00:00
categories: articles
tag: [blender]
image:
  feature: Blender_LP_Illustration_Preview.jpg
comments: true
logo: false
---

[Source](http://cgi.tutsplus.com/tutorials/secrets-to-creating-low-poly-illustrations-in-blender--cg-31770 "Permalink to Secrets to Creating Low Poly Illustrations in Blender")

* * *

## 1. Secret Ingredients

### Flat Shaded Models

One of the main requirements to achieve this style, is that the models must be flat shaded. This will give a blocky looking result, which a smooth shaded surface does not produce.

![Blender_LP_Illustration_s01][2]

* * *

### Low Poly Models

Another prerequisite for this style is that the models must be low poly (obviously!). The forms must be drawn close to basic geometric shapes. For organic models, if you find it difficult to built them using less triangles, then don't worry. You can construct the model as you want and later crunch those polys down with the help of the Decimate Modifier. You can also import and use your existing mid-poly models, and then use the Decimate Modifier to reduce the polygons.

![Blender_LP_Illustration_s02][3]

* * *

### Triangles

For better results, it's sometimes good to triangulate the mesh. Triangles are something we typically avoid while modeling, as we like to keep everything in quads. But no problem, every quad or square are two triangles combined together, so we don't have to build the models thinking only in triangles. Just construct the models as you usually would, and in edit mode we can triangulate the mesh.

![Blender_LP_Illustration_s03][4]

* * *

### Lighting

Lighting is the most important part of producing a good render. The scene should be properly lit according to the composition, and we must use Ambient Occlusion and Global Illumination. Photo-realistic rendering will produce the best result, otherwise the scene will look like a render from a 3D game from the 90's. This lighting and shading are what set it apart from a bad looking render.

![Blender_LP_Illustration_s04][5]

* * *

Now we will create a scene and learn how to apply the above points to achieve the desired style.

## 2. Rough Sketch and Layout

### Step 1

First draw a rough sketch of the illustration. This is necessary as it will serve as a blueprint and you won't feel lost later. Although everything is constructed in 3D, the illustration itself is 2D Art. Everything is arranged for a 2D frame, be it cinema, photography or 3D illustrations. The final result is shown on a monitor, TV screen or cinema screen, which are all 2D surfaces. So the layout or frame, must be properly balanced and arranged.

![Blender_LP_Illustration_r01][6]

* * *

## 3. Modeling The Terrain

### Step 1

In a new file press **Shift-A** and add a **Plane**.

![Blender_LP_Illustration_001a][7]

Press **TAB** on the keyboard to enter into **Edit** mode. Then Press **S** and drag the mouse to scale the **Plane** up.

![Blender_LP_Illustration_001b][8]

* * *

### Step 2

While in the **Edit** mode and with the mouse pointer in the 3D view, press **W** and select **Subdivide**, to subdivide it.

![Blender_LP_Illustration_002a][9]

Do this several times. Three to four times would be sufficient, don't make it too dense.

![Blender_LP_Illustration_002b][10]

* * *

### Step 3

Press **A** to deselect all the vertices. Now to create the mountain ridge, select _two_ vertices as shown in the following image. **Right Click** on any vertex to select it, and then _hold_** Shift **and** Right Click **on another vertex to select multiple vertices. Here I have pressed **5** on the Numpad to get into **Perspective** mode. To Rotate the view, click and drag using the **Middle Mouse Button**.

![Blender_LP_Illustration_003][11]

* * *

### Step 4

While in **Edit** mode, press **O** on the keyboard to enable the **Proportional Editing Tool** (Soft selection), and make sure that **Smooth** falloff is selected.

![Blender_LP_Illustration_004a][12]

* * *

### Step 5

Now drag the Arrow Widget to move the vertices upward (Z axis). Or press **G** and then **Z** to move the vertices along the **Z** Axis only. Move them up just a little bit, not too much. You can increase or decrease the area of influence with the **Mouse Wheel**.

![Blender_LP_Illustration_005][13]

Now select _only_ one of the verts and pull it upwards. Again you can either use the Arrow Widget, or press **G** and then **Z** and move your mouse, to move the vertex up.

![Blender_LP_Illustration_005b][14]

* * *

### Step 6

Press **A** to select all the vertices, and then Press **Control**-**T** to triangulate the mesh.

![Blender_LP_Illustration_006][15]

* * *

### Step 7

Press **A** again to deselect the mesh. Now select **Random** Falloff mode.

![Blender_LP_Illustration_007][16]

* * *

### Step 8

Select a few of the peak points and move them upwards (hold **Shift** and then **Right Click** to select more than one vertex.) You will see that the mountain is now taking shape, but take care that the ground is not being affected too much. You can also tweak the points individually to achieve the desired effect.

![Blender_LP_Illustration_008][17]

* * *

### Step 9

Again select all the vertices by pressing **A,** and then press **W** to bring up the **Specials** menu. Select **Shade Flat **to give it a flat look and then press **TAB** to exit **Edit** mode. The mountain is now ready. So press **Control-S **to save the file.

![Blender_LP_Illustration_009][18]![Blender_LP_Illustration_009b][19]

* * *

## 3. Assigning Materials to the Mountain

### Step 1

With the **Mountain** object selected, click on the **Materials** button in the **Properties **window and press the **New** button.

![Blender_LP_Illustration_mm01][20]

Name the new material "Green" or "Ground", and set the **Diffuse** color to a warm green. Reduce the **Specular** **Intensity** to **0.0**, as we want to have a non-shiny material.

![Blender_LP_Illustration_mm01b][21]

* * *

### Step 2

Here we will learn how to assign multiple materials to a single object. Press **TAB** to enter into **Edit** mode and then press **Z** for **Wireframe** mode, so that while selecting we are able to select the faces and vertices which are behind and nothing will be left out. Press **Control-TAB** and select **Face** in the **Mesh Select** mode menu. Now press **B** and drag to select the part of the mountain which is above the ground. If you miss some faces, manually select them by holding down the **Shift** key and **Right Clicking** on them.

![Blender_LP_Illustration_mm02][22]

* * *

### Step 3

Click on the **+** button to add a new material slot and then press the **New** button.

![Blender_LP_Illustration_mm03][23]

* * *

### Step 4

Name the new material, and give it a nice stone color or make it brown. Again, reduce the **Specular** **Intensity** to **0.0**.

![Blender_LP_Illustration_mm04][24]

Finally, click **Assign** to assign the new material to the selected faces.

![Blender_LP_Illustration_mm04b][25]

* * *

### Step 4

Now we will create some snow on top of the mountain. So select the top few faces and create a new material (just as we did to create the second material.) Press the **+** button to add a new slot, click on the **New** button, change the color to White and reduce the **Specular** **Intensity** to **0.0**.

![Blender_LP_Illustration_mm05][26]

Finally, press **Apply** to apply the material to the selected faces.

![Blender_LP_Illustration_mm05b][27]

* * *

## 4. Modeling the Trees

### Step 1

**Left Click** on an empty space to bring up the 3D cursor. Press **Shift-A &gt; Mesh &gt; Icosphere** to add a sphere to the scene.

![Blender_LP_Illustration_t01][28]

* * *

### Step 2

Press **.** (period) on the numpad to make it centered and **3** (on the numpad) to get into the _Right_ view (Press **5** to turn off Perspective view.) Press **Shift-A** and add** Mesh &gt; Cylinder**.

![Blender_LP_Illustration_t02][29]

Press **T** to bring out the **Tool Shelf** (if it's not already there) and reduce the **Vertices** to **6**.

![Blender_LP_Illustration_t02b][30]

* * *

### Step 3

Press **TAB** to enter into **Edit** mode. Select all the vertices by pressing **A**, and press **S** to scale them down to make the trunk of the tree.

![Blender_LP_Illustration_t03][31]

* * *

### Step 4

Deselect all the vertices with the **A** key. Then press **B** to drag select _only_ the top vertices and then pull them up along the **Z** axis, by dragging the Arrow Widget or by hitting the **G** key and then **Z**, moving the mouse and finally clicking to confirm.

![Blender_LP_Illustration_t04][32]

* * *

### Step 5

With the _top_ row of vertices selected, press **S** and scale them down to give the trunk a nice shape (you can also press **Z** to preview it in Solid mode.)

![Blender_LP_Illustration_t05][33]

* * *

### Step 6

Now we will reduce the polygons for the leaves. Select the object (icosphere) by **Right Click****ing**, and then click on the **Modifiers** button in the **Properties **window, and select **Decimate**.

![Blender_LP_Illustration_t06][34]

Reduce the **Ratio** according to how low poly you want the tree to look.

![Blender_LP_Illustration_t07][35]

Finally click **Apply**.

![Blender_LP_Illustration_t07b][36]

* * *

## 5. Creating Materials for the Tree

### Step 1

With the leaves selected, click on the **Materials** button on the **Properties** panel and add **New**.

![Blender_LP_Illustration_mt01][37]

* * *

### Step 2

Name the new material "Leaves" and choose a nice green color. Reduce the **Specular** **Intensity** to **0**.**0**.

![Blender_LP_Illustration_mt02][38]

* * *

### Step 3

Now select the **Trunk**, and in the **Material **properties click on **New**.

![Blender_LP_Illustration_mt03][39]

* * *

### Step 4

Name the new material "Brown" (or whatever you like.) Choose a nice brown color for the **Diffuse** and reduce the **Specular** **Intensity** to **0.0**.

![Blender_LP_Illustration_mt04][40]

* * *

## 6. Making the Tree a Single Object

### Step 1

Select _both_ objects (hold **Shift** and **Right Click** on the objects) and then press **Control-J** to join them, and make them a single object. The tree is now ready.

![Blender_LP_Illustration_t08][41]

* * *

## 7. Modeling a Different Tree

### Step 1

Press **Shift-A** to add a **Cylinder**. In the **Tool** shelf, reduce the **Vertices** to **5** or **6**.

![Blender_LP_Illustration_tb01][42]

* * *

### Step 2

Press **TAB** to enter into **Edit** mode, and select all the vertices with the **A** key. Press **S** to scale them down.

![Blender_LP_Illustration_tb02][43]

**Scale** them again along the **Z** axis. Press **S** and then **Z** to scale vertically. Select the _top_ row of verticies with the **B** key, and **Scale** them down to give it a nice form.

![Blender_LP_Illustration_tb02b][44]

* * *

### Step 3

Select all the vertices by pressing the **A** key. And then press **Shift-D** to duplicate the selection. Click anywhere to confirm.

![Blender_LP_Illustration_tb03][45]

* * *

### Step 4

Press **R** to **Rotate** the mesh to form a branch. **Scale** the new mesh down with the **S** key.

![Blender_LP_Illustration_tb04][46]

* * *

### Step 5

With the new mesh selected, press** Shift-D** to duplicate it.

![Blender_LP_Illustration_tb05][47]

Press **R** to **Rotate** it, and then **TAB** to exit **Edit** mode.

![Blender_LP_Illustration_tb05b][48]

* * *

### Step 6

Click on an empty space near the new trunk, press **Shift-A **and add an **Icosphere**.

![Blender_LP_Illustration_t06][34]

* * *

### Step 7

With the sphere selected, click on the **Modifiers** button in the **Properties** window, and add a **Decimate** modifier.

![Blender_LP_Illustration_t07][35]

Reduce the **Ratio** amount to achieve a nice low poly look.

![Blender_LP_Illustration_t07b][36]

Finally click **Apply**

![Blender_LP_Illustration_tb07c][49]

* * *

### Step 8

Select the **Icosphere** by **Right Clicking**, and press **Shift-D** to duplicate it, and then click again to confirm. Place it on the second branch (Press **G** to move) and scale it with the **S** key (to **Rotate**, press **R**). You can adjust both spheres to give the tree a nice shape. Our second tree is now ready.

![Blender_LP_Illustration_tb08][50]

* * *

## 8. Assigning Materials to the New Tree

### Step 1

**Right Click** on the **Sphere** to select it. And in the **Material** properties, assign the already created **Leaves** material to the **Sphere**.

![Blender_LP_Illustration_tb09][51]![Blender_LP_Illustration_tb09b][52]

* * *

### Step 2

Similarly assign the corresponding materials to the rest of the parts.

![Blender_LP_Illustration_tb09c][53]

* * *

### Step 3

Select all the objects of the new tree, and press **Control-J** to combine them into one single object. The second tree is now ready.

![Blender_LP_Illustration_tb10][54]

* * *

## 9. Creating the Clouds

### Step 1

Press **Shift-A** and add another **Icosphere**.

![Blender_LP_Illustration_c01][55]

* * *

### Step 2

Press **TAB** to get into **Edit** mode, and select all the vertices by pressing the **A** key. Press **Shift-D** to duplicate the mesh and click again to confirm the position. With the new mesh selected, press **S** and scale it down, and **G** to move the selected mesh into the right position.

![Blender_LP_Illustration_c02][56]

* * *

### Step 3

Similarly, duplicate the sphere again to complete the cloud, and press **TAB** to exit **Edit** mode.

![Blender_LP_Illustration_c03][57]

* * *

### Step 4

With the cloud selected, click on the **Modifiers** button in the **Properties** window, and select **Decimate**.

![Blender_LP_Illustration_c04][58]

Reduce the **Ratio** amount to achieve a low poly look, but not too much that it loses its shape.

![Blender_LP_Illustration_c04b][59]

* * *

### Step 5

With the cloud selected, click on the **Materials** button in the **Property** window, and then click on the **New** button.

![Blender_LP_Illustration_c05][60]

Name this material "White" or "Clouds", and set its **Diffuse** color to white, and reduce the **Specular** **Intensity** to **0.0**.

![Blender_LP_Illustration_c05b][61]

* * *

## 10. Bringing it All Together

### Step 1

Now lets arrange all the objects together to make the scene. Press **3** on the numpad to get into a side view. Switch to **Ortho** view by pressing **5** on numpad (if you are in **Perspective** view). Now select the tree by **Right Clicking **on it, and then press **G** to move it to the desired position. **Scale** it as needed with the **S** key.

![Blender_LP_Illustration_a01][62]

* * *

### Step 2

Press **7** on the numpad to get into the **Top **view. Select the** Tree** and press **Shift-D** to duplicate it. Place it alongside the mountain and repeat this process to create a nice landscape.

![Blender_LP_Illustration_a02][63]

* * *

### Step 3

Now we'll add the camera. Press **Shift-A** and add a **Camera** and place it according to your composition. Press **G** to move and **R** to rotate the camera, and press** 0** on the numpad to change to the camera's view.

![Blender_LP_Illustration_a03][64]![Blender_LP_Illustration_a03b][65]

* * *

### Step 4

You can **split** the 3D view and assign one for the camera, one for the top and one for the side view. Move the mouse over the corner of the 3D view, and when it changes, pull to split the window. Move you mouse over any of the views and press **7** on the numpad to get a **Top** view, **3** (numpad) for a side view and **0** on the numpad for the **Camera** view. Now you can adjust the position of your objects, and see the arrangement in the camera view. While in the camera view, you can press **Shift-F** to move the camera to adjust the frame in a fly-through mode.

![Blender_LP_Illustration_a04][66]![Blender_LP_Illustration_a04b][67]

I have set a new size for the frame according to my needs in the **Render** panel. You can adjust yours, or leave it at the default.

![Blender_LP_Illustration_a04c][68]

* * *

### Step 5

Now lets add some light. Press **Shift-A** and add a **Sun**. Place it on one side, and adjust its direction by rotating it with the **R** key.

![Blender_LP_Illustration_a05][69]

With the **Sun** selected, click on the **Light** **Properties**. Change the color to a light yellow and turn on the **Ray Shadows **option.

![Blender_LP_Illustration_a05b][70]

Now press **F12** to render the scene.

![Blender_LP_Illustration_a05c][71]

* * *

### Step 6

Click on the **World** settings in the **Properties** panel and set the **Sky** color to blue and check the **Blend Sky **option, so that we get a nice gradient with the zenith color. Turn on **Ambient Occlusion** so we get realistic shadows, and also turn on** Environment Lighting** and choose **Sky Color** as the light source. In the **Gather Panel**, increase the** Samples **to** 10**, and finally turn on **Stars**.

![Blender_LP_Illustration_a06][72]

Hit **F12 **to render and you'll see the effect of the sky color and Ambient Occlusion.

![Blender_LP_Illustration_a06b][73]

* * *

### Step 7

I have added a **Plane** on the opposite side of the sun, so that the scene doesn't get much light from that side. Make sure it doesn't show in the camera view.

![Blender_LP_Illustration_a07][74]![Blender_LP_Illustration_a07b][75]

* * *

### Step 8

In the **World** panel, Change the **Ambient Color** to dark purple. This will give a nice tint to the image.

![Blender_LP_Illustration_a08][76]

## Conclusion

Hit **F12** and see the magic! I hope you enjoyed this tutorial.

![Blender_LP_Illustration_a08b][77]

* * *

[1]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_Preview.jpg
[2]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_s01.jpg
[3]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_s02.jpg
[4]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_s03.jpg
[5]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_s04.jpg
[6]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_r01.jpg
[7]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_001a.jpg
[8]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_001b.jpg
[9]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_002a.jpg
[10]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_002b.jpg
[11]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_003.jpg
[12]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_004a.jpg
[13]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_005.jpg
[14]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_005b.jpg
[15]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_006.jpg
[16]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_007.jpg
[17]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_008.jpg
[18]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_009.jpg
[19]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_009b.jpg
[20]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_mm01.jpg
[21]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_mm01b.jpg
[22]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_mm02.jpg
[23]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_mm03.jpg
[24]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_mm04.jpg
[25]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_mm04b.jpg
[26]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_mm05.jpg
[27]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_mm05b.jpg
[28]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_t01.jpg
[29]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_t02.jpg
[30]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_t02b.jpg
[31]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_t03.jpg
[32]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_t04.jpg
[33]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_t05.jpg
[34]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_t06.jpg
[35]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_t07.jpg
[36]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_t07b.jpg
[37]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_mt01.jpg
[38]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_mt02.jpg
[39]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_mt03.jpg
[40]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_mt04.jpg
[41]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_t08.jpg
[42]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_tb01.jpg
[43]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_tb02.jpg
[44]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_tb02b.jpg
[45]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_tb03.jpg
[46]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_tb04.jpg
[47]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_tb05.jpg
[48]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_tb05b.jpg
[49]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_tb07c.jpg
[50]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_tb08.jpg
[51]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_tb09.jpg
[52]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_tb09b.jpg
[53]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_tb09c.jpg
[54]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_tb10.jpg
[55]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_c01.jpg
[56]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_c02.jpg
[57]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_c03.jpg
[58]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_c04.jpg
[59]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_c04b.jpg
[60]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_c05.jpg
[61]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_c05b.jpg
[62]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a01.jpg
[63]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a02.jpg
[64]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a03.jpg
[65]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a03b.jpg
[66]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a04.jpg
[67]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a04b.jpg
[68]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a04c.jpg
[69]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a05.jpg
[70]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a05b.jpg
[71]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a05c.jpg
[72]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a06.jpg
[73]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a06b.jpg
[74]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a07.jpg
[75]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a07b.jpg
[76]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a08.jpg
[77]: https://cdn.tutsplus.com/cg/uploads/2014/01/Blender_LP_Illustration_a08b.jpg
  
