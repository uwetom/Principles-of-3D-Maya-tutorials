# Worksheet 4 - Textures

## Add colour

### Create a new scene

- Open up Maya
- Create a new Scene

![new scene button](images/worksheet_4/new_scene.jpg)

- Save the scene in a new folder, This is particularly important as we will be adding separate texture files which Maya will not find if you move them later.

### Add a polygon

- Create a polygon cube

![create cube button](images/worksheet_4/create_cube.jpg)

### Add a material

- Select you cube, **hold down the right mouse button** and select  **Assign New Material...**

![new material button](images/worksheet_4/new_material.jpg)
	
- Select **Arnold > AiStandardSurface**

![](images/worksheet_3/ai_standard_surface.png)

The Attribute editor will now appear.

If you loose your attribute editor panel, you can get it back by first making sure your object is selected, and then holding down the right mouse button and selecting **Material Attributes**

![material attributes button](images/worksheet_4/material_attributes.jpg)

- Change the name to "cube material 1" and press enter. It is really important to name materials to avoid confusion later on when you have multiple materials.

![material name](images/worksheet_4/cube_material_1.jpg)

- Change the colour of the material by double clicking on the box next to **Color**

![](images/worksheet_4/new_standard_surface.PNG)

Your cube should now appear as that colour.

- Experiment with the **Roughness** and **Metallic** sliders to see how they change the look of the cube.

![](images/worksheet_4/metalness.PNG)

### Adding an image map

- Create another cube, move it next to the first and assign a new **AiStandardSurface** material just like we did above.
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

- You should now see the pattern applied to your cube

![giraffe pattern applied to cube](images/worksheet_4/giraffe_texture_applied.jpg)

- If you cannot see it, check the **textured** icon at the top of the panel is active.

![](images/worksheet_4/textured_button.jpg)

 
### Change the scale

To scale the pattern, press the image checkerboard button again

![](images/worksheet_4/colour_file.PNG)

- Then the place2dTexture tab

![](images/worksheet_3/place_2d_texture.png)

- Then changing the Repeat UV values, it is a good idea to keep them the same to avoid stretching the texture.

![](images/worksheet_3/repeat_uv.png)


### Import a model

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

- Delete the history of the cactus by selecting your model and pressing the **Delete history** button.

![](images/worksheet_5/delete_history.png)

### Freeze transforms

When making your model you may have scaled some of the pieces. Before uv mapping, the scales all need to be reset to 1. To do this select the cactus and press the **Freeze transforms** button.

![](images/worksheet_5/freeze.png)

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

- You can select faces in the UV editor and see their corresponding face the perspective view

![faces selected in uv mode](images/worksheet_4/uv_selection.jpg)
	
In this image you can see where the front of the cactus is.

### Editing UV shells

Automatic mapping splits the surface of the model into different uv shells. It does a reasonable job,  however, it is not very smart and can splits the model into more uv shells than necessary. 

If you have a seamless texture you will see joints in the texture between shells.

![](images/worksheet_4/seams.PNG)

You cannot avoid joints entirely, however, if you manually uv map your  model you have more control to hide the joint.

- If you would like to manually map your own model, please watch my UV mapping video on Blackboard (learning materials > Maya content >  extra videos)

For this worksheet we will continue with what the automatic mapping has given us.

## Create your own texture

We are now going to export the UV's and open them up in PhotoShop and create our own textures.

### Create a snapshot

- In the UV editor, use the mouse to select all the uv shells by drawing a square around them.

![](images/worksheet_3/select_all.gif)

- Now Take a snapshot of the uvs by pressing the camera icon at the top of the editor.

![snapshot button](images/worksheet_4/camera.jpg)

- Save the snapshot somewhere sensible on your machine. make sure it is set to png and the edge colour is black.

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

### Apply the next texture to your Cactus

- Go back into Maya
- Close the UV editor panel if it is still open
- Select your cactus
- Hold down the right mouse button and select **Assign new material**

![](images/worksheet_4/new_material.jpg)

- Select **Maya > AiStandardSurface** as before
- Add the colour map you just created

![change color map button](images/worksheet_4/change_colour_map.jpg)

### Look at your applied texture

- Your finished cactus should look something like this

![finished cactus](images/worksheet_4/finished_cactus.jpg)

## Extra Challenges

- Find a seamless stone texture online and apply it to the cactus pot.
- Texture your pear or robot from the previous worksheets.

## Final Challenge

- Watch the manual UV mapping video on Blackboard and try to manually map the cactus and reapply the texture.


