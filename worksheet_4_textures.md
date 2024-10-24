# Worksheet 4 - Textures

## Add colour

### Create a new scene

- Open up Maya
- Create a new Scene

- Save the scene in a new folder, This is particularly important as we will be adding separate texture files which Maya will not find if you move them later.

### Add a polygon

- Create a polygon cube

![create cube button](images/worksheet_4/create_cube.jpg)

### Add a material

With the cube selected

- In the **Rendering** tab, select **Standard Surface Material**

![](images/worksheet_4/standard_surface.jpg)

The Attribute editor should open on the right of the screen showing the **StandardSurface2** tab open.

![](images/worksheet_4/standard_surface_2.jpg)

NOTE : You can see the material on any object by selecting it, then holding down the right mouse button and selecting **Material Attributes**

![material attributes button](images/worksheet_4/material_attributes.jpg)


#### Change the name

- Change the name to "cube material 1" and press **enter**. It is really important to name materials to avoid confusion later on when you have multiple materials.

![material name](images/worksheet_4/cube_material_1.jpg)

- Change the colour of the material by double clicking on the box next to **Color**

![](images/worksheet_4/new_standard_surface.PNG)

![](images/worksheet_4/choose_ss_colour.jpg)

- Press **Done** and Your cube should now appear as that colour.

- There are lots of options to adjust the material, you can adjust the metalness and roughness but the full effect will only become clear when we move on to lighting and rendering next week.

![](images/worksheet_4/metalness.PNG)

You can apply different materials to different faces.

- Select some faces and apply apply a new standard surface material.

![](images/worksheet_4/2nd_material.jpg)


### Adding an image map

- Create another cube, move it next to the first and assign a new **StandardSurface** material just like we did above.
- This time, name it "giraffe_skin_material"
- Instead of a colour, we want to use an image.
- Download the giraffe print image 

[Giraffe texture](./assets_for_worksheets/giraffe.jpg)

- Save it in the same folder as your scene. this is really important as the image will be loaded in each time you open Maya. 
- Click the black and white button next to Color 

![](images/worksheet_4/colour_file.PNG)

- Choose file

![file button](images/worksheet_4/file.jpg)
	
- Click on the folder icon and find the giraffe pattern you downloaded earlier.

![choose folder button](images/worksheet_4/choose_folder.jpg)

- Check the **textured** icon at the top of the panel is active.

![](images/worksheet_4/textured_button.jpg)

- You should now see the pattern applied to your cube

![giraffe pattern applied to cube](images/worksheet_4/giraffe_texture_applied.jpg)


### Change the scale

We now want to scale the pattern

- go back to the material attributes by **right clicking** on the cube and selecting **Material attributes**

![](images/worksheet_4/material_attributes.jpg)

press the image arrow next to the colour

![](images/worksheet_4/colour_arrow.jpg)

- Then the place2dTexture tab

![](images/worksheet_3/place_2d_texture.png)

- Then changing the Repeat UV values, it is a good idea to keep them the same to avoid stretching the texture.

![](images/worksheet_3/repeat_uv.png)


### Import a model

We are now going to apply a texture to more complex object.

- Download the cactus fbx file

[cactus fbx file](./assets_for_worksheets/cactus.fbx)

- Import the model into Maya by choosing **File > import**

![import button](images/worksheet_4/import.jpg)

- Move the model so it is not on top of the cubes.

![cactus next to textured cubes](images/worksheet_4/move_cactus.jpg)

## Prepare the model

To apply an image texture to a more complicated object we first need to prepare the model so that the textures appear correctly.

Part of this process is UV mapping which we will do shortly, but before this we need to clean it up.

### Delete history

The history keeps track of changes you make to your model but can make your outliner and uv mapping more complicated.

**- Important -** If you are working on your own model, save a copy before you delete the history so that you can go back if you need to.

- Delete the history of the cactus by selecting the pot and cactus and pressing the **Delete history** button in the Poly Modeling tab

![](images/worksheet_4/delete_history.jpg)

### Freeze transforms

When making your model you may have scaled some of the pieces. Before uv mapping, the scales all need to be reset to 1. To do this select the cactus and press the **Freeze transforms** button.

![](images/worksheet_4/freeze.jpg)

### Apply a material

- Select the cactus and apply the giraffe skin texture by right clicking and choosing **Assign Existing Material** > **giraffe_skin_material**

![existing material button](images/worksheet_4/existing_material.jpg)

You should now see the material on the cactus, but it may look distorted and stretched. This is because it has not been UV mapped.

![cactus with stretched material on it](images/worksheet_4/stretched_material.jpg)

## UV mapping

UV mapping should be done after you have completely finished modeling. If you make any changes to your mesh you may need to re-map all or part of your model.

The easiest solution to this is to use automatic mapping.
- With the cactus still selected, select **UV > Automatic** from the top menu

![automatic uving](images/worksheet_4/automatic_uv.jpg)

This should do a reasonable job at UV mapping the cactus for you

![cactus with correct texture on it](images/worksheet_4/automatically_mapped_cactus.jpg)


### UV Editor

- With your cactus selected, choose **UV** > **UV Editor** from the top menu

![uv editor button](images/worksheet_4/uv_editor.jpg)

This will open up the editor allowing you to see how automatic mapping has laid out your UV's.

- You can select uv faces in the UV editor and see their corresponding polygon face in the perspective view

![faces selected in uv mode](images/worksheet_4/uv_selection.jpg)
	
In this image you can see where the front of the cactus has been mapped to.

### Editing UV shells

Automatic mapping splits the surface of the model into different uv shells. It does a reasonable job,  however, it is not very smart and can splits the model into more uv shells than necessary. 

If you have a seamless texture you will see joints in the texture between shells.

![](images/worksheet_4/seams.PNG)

You cannot avoid joints entirely, however, if you manually uv map your model you have more control to hide the joint.

- If you would like to manually map your own model, please watch my UV mapping video on Blackboard (learning materials > Maya content >  extra videos)

For this worksheet we will continue with what the automatic mapping has given us.

## Create your own texture

We are now going to export the UV's and open them up in PhotoShop and create our own textures.

### Create a snapshot

Each piece is called a UV Shell.

- In the **UV editor** Press the **UV Shell Selection** button in on the right.

![](images/worksheet_4/uv_shell_mode.jpg)

- Use the mouse to select all the uv shells by drawing a square around them.

![](images/worksheet_3/select_all.gif)

- Now Take a snapshot of the UV's by pressing the camera icon at the top of the editor.

![snapshot button](images/worksheet_4/camera.jpg)

- Save the snapshot to the same folder as your scene. make sure it is set to png and the edge colour is black.

![save snapshot button](images/worksheet_4/save_snapshot.jpg)

### Open the snapshot in PhotoShop

- Open PhotoShop on your machine
- Use PhotoShop to open the snapshot you just created.

![open photoshop](images/worksheet_4/open_photoshop.jpg)

Layer 1 is your snapshot.
	
- Create 3 new layers by clicking the plus button at the bottom right of the screen.

![create 3 layers in photoshop](images/worksheet_4/plus.jpg)

- Layer 2 is going to be our background, click on it to select it

![base layer](images/worksheet_4/base_layer.jpg)
	
- Choose a green fill colour by double clicking the little black square at the bottom left of the screen and choosing a green colour.

![choose fill colour](images/worksheet_4/choose_colour.jpg)
	
- Press **alt and delete** on the keyboard fill the layer with green.

- Click and drag layer 1 so that it appears above layer 2 in the list. 

![](images/worksheet_3/layer_order.png)

### Add a face

- Download one of the following face image

[face image 1](./assets_for_worksheets/face_1.png)

[face image 2](./assets_for_worksheets/face_2.png)

[face image 3](./assets_for_worksheets/face_3.png)

[face image 4](./assets_for_worksheets/face_4.png)

[face image 5](./assets_for_worksheets/face_5.png)


- Click on layer 3 in PhotoShop to select it.
- Drag the face image file into PhotoShop and drop it in the middle of the screen
- Drag and scale it so that is in the right position on the snapshot.

![face showing in photoshop](images/worksheet_4/face_in_photoshop.jpg)
	
- We want to hide the initial snapshot image before we export, so press the eye icon next to layer 1 to hide it.

![hide layer 1](images/worksheet_4/hide_layer_1.jpg)

- Export the image by selecting **File > Export > Quick Export as PNG** and save it in your principles of 3d folder. name it "cactus_with_face"

### Apply the new texture to your Cactus

- Go back into Maya
- Close the UV editor panel if it is still open
- Select your cactus
- Assign a new **standard surface material** as you did before.

![](images/worksheet_4/standard_surface.jpg)

- rename the material

- Add the colour map the same way as you added the giraffe texture. (file)

![](images/worksheet_4/cactus_colour.jpg)

### Look at your applied texture

- Your finished cactus should look something like this

![finished cactus](images/worksheet_4/finished_cactus.jpg)

## Extra Challenges

- Find a seamless stone texture online and apply it to the cactus pot.

A good source of free textures is [ambientcy.com](https://ambientcg.com/)
- Texture your pear or robot from the previous worksheets.

## Final Challenge

- Watch the manual UV mapping video on Blackboard and try to manually map the cactus and reapply the texture.


