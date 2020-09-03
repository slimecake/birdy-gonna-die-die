# birdy-gonna-die-die
Python implementation of the game Flappy Bird, played by a neural network

## Files
In the script there are some areas which need to be filled in because they are specific to my file locations, however the script will not run unless they are changed to your specific file locations.

### Bird Files
The following list can found in the **script** on line **13**:

	BIRD_IMGS = [pygame.transform.scale2x(pygame.image.load(os.path.join(r"IMAGE_FOLDER",r"BIRD_1"))),
		    pygame.transform.scale2x(pygame.image.load(os.path.join(r"IMAGE_FOLDER", r"BIRD_2"))),
		    pygame.transform.scale2x(pygame.image.load(os.path.join(r"IMAGE_FOLDER", r"BIRD_3")))
	]

The image folder is called **imgs**, to insert the location of the image folder you must locate to it and press the **shift key** on your keyboard and then **right click**. Once that is done select **copy as path** and return back to the script. Once you are in the script delete the part that says **IMAGE_FOLDER** and replace it with the folder path that you just copied. To paste the path press **ctrl and v** on your keyboard or alternitivly **right click and select paste**. **BIRD_1**, **BIRD_2** and **BIRD_3** are all located in the **imgs** folder. do what you did with the **imgs** folder before to **BIRD_1**, **BIRD_2** and **BIRD_3**.


### Pipe Files
The following variable can be found in the **script** on line **14**.

	PIPE_IMG = pygame.transform.scale2x(pygame.image.load(os.path.join(r"IMAGE_FOLDER", r"PIPE_IMAGE")))

The image folder is called **imgs**, to insert the location of the image folder you must locate to it and press the **shift key** on your keyboard and then **right click**. Once that is done select **copy as path** and return back to the script. Once you are in the script delete the part that says **IMAGE_FOLDER** and replace it with the folder path that you just copied. To paste the path press **ctrl and v** on your keyboard or alternitivly **right click and select paste**. **PIPE_IMAGE** is located in the **imgs** folder. do what you did with the **imgs** folder before to **PIPE_IMAGE**.


### Base Files
The following variable can be found in the **script** on line **15**

	BASE_IMG = pygame.transform.scale2x(pygame.image.load(os.path.join(r"IMAGE_FOLDER", r"BASE_IMAGE")))

The image folder is called **imgs**, to insert the location of the image folder you must locate to it and press the **shift key** on your keyboard and then **right click**. Once that is done select **copy as path** and return back to the script. Once you are in the script delete the part that says **IMAGE_FOLDER** and replace it with the folder path that you just copied. To paste the path press **ctrl and v** on your keyboard or alternitivly **right click and select paste**. **BASE_IMAGE** is located in the **imgs** folder. do what you did with the **imgs** folder before to **BASE_IMAGE**.

### Bg Files
The following variable can be found in the **script** on line **16**

	BG_IMG = pygame.transform.scale2x(pygame.image.load(os.path.join(r"IMAGE_FOLDER", r"BG_IMAGE")))

The image folder is called **imgs**, to insert the location of the image folder you must locate to it and press the **shift key** on your keyboard and then **right click**. Once that is done select **copy as path** and return back to the script. Once you are in the script delete the part that says **IMAGE_FOLDER** and replace it with the folder path that you just copied. To paste the path press **ctrl and v** on your keyboard or alternitivly **right click and select paste**. **BG_IMAGE** is located in the **imgs** folder. do what you did with the **imgs** folder before to **BG_IMAGE**.