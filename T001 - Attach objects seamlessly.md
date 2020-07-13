# T001 - Attach objects seamlessly

### Introduction

This Tutorial will show you how to create your own mesh stickers and put them on anything you want!



### 1. Align the object to the origin.

0. Build your mesh

1. Go into `Edit Mode`

2. Move the whole object on the `Z Axis` so the lowest point will match with the origin point.

   ![Image of urmom](https://github.com/rcv4/tutorials/blob/master/t001/t001_align_origin.gif?raw=true)

   

   

### 2. Make the sticker area.

1. Extrude the bottom edge.

2. Create a loop cut with about 4 new loops.

3. Create a bevel between the base and your new extruded mesh

4. Done   

      

### 3. Assign vertex weights

1. Select the outer loop (4th) of the extruded sticker area
2. Press `CTRL + G` to create a new vertex group
3. Go to the `Vertex Groups` Panel in the `Object Data Properties` Tab
4. Select the 3rd loop.
5. Set the weight to `0.800` and click assign
6. Now select the 2nd loop and change the weight to `0.600`
7. Click assign.
8. Now select the 1rst loop and change the weight to `0.400`
9. Now select the next loop, set the weight to `0.200` and click assign



### 4. Preparation.

0. Get your target object.

1. Enable `Snap` in the Viewport

2. Change "Snap to" to `Face` 

3. Change "Snap with" to `Active`

4. Check `Align Rotation to Target` 

5. Move your object onto the target

   

### 5. Attaching it to the Target

1. Add a `Shrinkwrap` modifier and set the Target
2. Select the created Vertex Group
3. Add a `Data Transfer` modifier and set the Source (the source is the target in the shrinkwrap)
4. Check `Face Corner Data`
5. Click `Custom Normals`
6. Select your Vertex Group on the bottom of the modifier
7. DONE!

