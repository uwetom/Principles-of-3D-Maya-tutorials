# Worksheet 3 - Textures
#### Worksheet length  - 1 hour

### Before you start

- All the machines in the lab have Maya installed, if you want you use your own machine follow the installation guide.

	https://www.uwe.ac.uk/study/it-services/software/specialist-software#autodesk_maya

- Make sure you have a mouse.


## Add colour

### Create a new scene

- Open up Maya
- Create a new Scene

  ![](images/worksheet_1/new_scene.jpg)

- Save the scene in the principles of 3d folder you created in workshop 1, or somewhere equally sensible.

### Add a polygon

- Create a polygon cube

	![](images/worksheet_1/create_cube.jpg)

### Add a material


- Select you cube, hold down the right mouse button and select 

	![](images/worksheet_1/new_material.jpg)
	
- Select **Maya > Standard Surface**

	![](images/worksheet_1/stingray_material.jpg)

- The Attribute editor will now appear
- First change the name to "cube material 1" and press enter. It is really important to name materials to avoid confusion later on.

	![](images/worksheet_1/cube_material_1.jpg)

- Change the colour of the material by double clicking on the box next to **Color**
- The cube in your scene should now have the colour, if it doesn't make sure the **textured** button is turned on in the viewport

	![](images/worksheet_1/textured_button.jpg)

- Experiment with the **Diffuse Roughness** and **Metallic** sliders to see how they change the look of the cube.
- If you loose your attribute editor panel, you can get it back by holding down the right mouse button on your object and selecting **Material Attributes**

	![](images/worksheet_1/material_attributes.jpg)

## Adding an image map

- Create another cube, move it next to the first and assign a new **Standard Surface** material just like we did above.
- This time, name it "giraffe_skin_material"
- Instead of a colour, we want to use an image.
- Download the giraffe print image from blackboard and save it in the same folder as your scene. this is really important as the image will be loaded in each time you open Maya. 
- Click the black and white button next to Color 

	![](images/worksheet_1/change_colour_map.jpg)

- The choose file

	![](images/worksheet_1/file.jpg)
	
- Then click on the folder icon and find the giraffe pattern you downloaded from blackboard earlier

	![](images/worksheet_1/choose_folder.jpg)

- You should now see the pattern applied to your cube

	![](images/worksheet_1/giraffe_texture_applied.jpg)


## UV mapping

### Import model from Blackboard

- Download the cactus.fbx file from blackboard
- Import the model into Maya by choosing File > import

	![](images/worksheet_1/import.jpg)

- Move the model so it is not on top of the cubes

	![](images/worksheet_1/move_cactus.jpg)

- Select the cactus and apply the giraffe skin texture by right clicking and choosing **Assign Existing Material** > **giraffe_skin_material**

	![](images/worksheet_1/existing_material.jpg)

- You should now see the material on the cactus, but it may look distorted and stretched. This is becase it has not been UV mapped.

	![](images/worksheet_1/stretched_material.jpg)

- The easiest solution to this is to use automatic mapping.
- With the cactus still selected, select UV > Automatic from the top menu

	![](images/worksheet_1/automatic_uv.jpg)

- This should do a fairly good job at UV mapping the cactus for you

	![](images/worksheet_1/automatically_mapped_cactus.jpg)

## Create your own texture

- We are now going to export the uv's and open them up in Photoshop and create our own textures.

### UV Editor

- With your cactus selected, choose **UV** > **UV Editor** from the top menu

	![](images/worksheet_1/uv_editor.jpg)

- This will open up the editor allowing you to see how Maya has laid out your UV's.
- You can select faces in the UV editor and see their corresponding face the perspective view

	![](images/worksheet_1/uv_selection.jpg)
	
- In this image you can see where the front of the cactus is.

### Create a snapshot

- In the uv editor, use the mouse to select all the uv's by drawing a square around them.
- Now Take a snapshot of the uvs by pressing the camera icon at the top of the editor.

	![](images/worksheet_1/camera.jpg)

- Save the snapshot somewhere sensible on your machine. make sure it is set to png and the edge colour is black.

	![](images/worksheet_1/save_snapshot.jpg)
	
### Open the snapshot in Photoshop

- Open Photoshop on your machine
- Use Photoshop to open the snapshot you just created.

	![](images/worksheet_1/open_photoshop.jpg)
	
- Create 3 new layers by clicking the plus button at the bottom right of the screen.

	![](images/worksheet_1/plus.jpg)

- Layer 2 is going to be our background, click on it to select it

	![](images/worksheet_1/base_layer.jpg)
	
- Choose a fill colour by double clicking the little black square at the bottom left of the screen

	![](images/worksheet_1/choose_colour.jpg)
	
- Press ctrl + g on the keyboard to select the fill tool
- Click anywhere on the screen to fill the layer.
- Click and drag layer 1 so that it appears above layer 2 in the list. 


### add a face


- Download the face image from blackboard
- Click on layer 3 in photoshop to select it.
- Drag the face image file into photoshop and drop it in the middle of the screen
- Drag and scale it so that is in the right position on the snapshot.

	![](images/worksheet_1/face_in_photoshop.jpg)
	
- We want to hide the initial snapshot image before we export, so press the eye icon next to layer 1 to hide it.

	![](images/worksheet_1/hide_layer_1.jpg)

- Export the image by selecting **File > Export > Quick Export as PNG** and save it in your principles of 3d folder. name it "cactus_with_face"

### Apply the next texture to your Cactus

- Go back into Maya
- Close the uv editor panel if it is still open
- Select your cactus
- Hold down the right mouse button and select **Assign new material**

	![](images/worksheet_1/material_attributes.jpg)

- Select **Maya > Standard Surface** as before
- Add the colour map you just created

	![](images/worksheet_1/change_colour_map.jpg)

### Look at your applied texture

- your finished cactus should look something like this

	![](images/worksheet_1/finished_cactus.jpg)

## What have I Learnt

- In this worksheet you have learnt
	- applying simple colour Textues
	- applying image Textues
	- remapping uvs using automatic mapping
	- editing textures using PhotoShop 
	
