# birdy-gonna-die-die
Python implementation of the game Flappy Bird, played by a neural network

## Files
In the script there are some areas which need to be filled in because they are specific to my file locations, however the script will not run unless they are changed to your specific file locations.

	BIRD_IMGS = [pygame.transform.scale2x(pygame.image.load(os.path.join(r"IMAGE_FOLDER",r"BIRD_1"))),
			pygame.transform.scale2x(pygame.image.load(os.path.join(r"IMAGE_FOLDER", r"BIRD_2"))),
		pygame.transform.scale2x(pygame.image.load(os.path.join(r"IMAGE_FOLDER", r"BIRD_3")))
	]

The image folder is called imgs, to insert the location of the image folder you must locate to it and press the shift key on your keyboard and then right click. Once that is done select copy as path and return back to the script. Once you are in the script delete the part that says "IMAGE_FOLDER" and replace it with the folder path that you just copied. To insert the path press ctrl and v on your keyboard or alternitivly right click and select paste.