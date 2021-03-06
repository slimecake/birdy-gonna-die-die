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

### CONFIG File
The following variable can be found in the **script** on line **270**

	config_path = os.path.join(local_dir, r"CONFIG_FILE")

The config file is called **neatCONFIG.txt**. Replace the **CONFIG_FILE** in the script with the path of the **neatCONFIG.txt**

## Training

Training time can vary from 10 minutes to 10 microseconds. If you want to see the process of its training set the **pop_size** to **5**.

However if you do not want to see how it works and proggresivly gets faster set the **pop_size** to **100**.

	[NEAT]
	fitness_criterion     = min
	fitness_threshold     = 500
	pop_size              = 5
	reset_on_extinction   = False

Higher the **pop_size** the faster the training.

**pop_size** and other parameters can be changed withing the **neatCONFIG.txt** file.

A **pop_size** of **5** takes roughly **100 generations** until it is a good AI.
A **pop_size** of **100** takes roughly **1 generation** until it is a good AI.

## How It Works
The AI works by using a simple **neural network** with **3** inputs (**y_movement**, **height_of_top_pipe**, **height_of_bottom_pipe**) it could theoreticly work with just **2** input but that would require more computer power since the **neural network** would need to calculate the distance between each pipe therefore increasing training times. The **neurel network** only has **1** output, should the bird go **up** or **down**. The bird only needs to move **up** or **down** becasue it **does not** move forward instead the **environment** moves backward. The problem with this is that because the **neural network** so simple it can not play the game without dying in the first few seconds. To conquer this what the **script** gradually **adds** or **changes** **layers** and **neurons** it also adjustes the **weights** and **biasses** until you have a **neurel network** that has been perfectly made and with enough **training** would never loose at the game **flappy bird**.

## Extra Information
The game and easily be adjusted to be played by a **human** instead of a **neural network**

To do this you must make a function called anything you want and **comment out or delete** all code that relates to the **AI**. In the function you must create an **if statement** that when **space** is clicked call the **jump function**.

**This may help:**

	import keyboard

	if keyboard.is_pressed('a'):
		print('a key has ben pressed')

Try and figure out if you can get it to work when **space** is pressed instead of **A**



_Special thanks to **Tech With Tim**_