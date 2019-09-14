# Automatic-Helmet-Detection-from-a-Bike-Rider
This project built for detecting bike riders who are not wearing helmets and Sends automated tax bill for violating traffic rules by detecting their number plates of the bike
			Automatic Helmet detection
Requirements:
	Opencv(3.4.2.16)
	Dlib
	Imutils
	Numpy
	Skimage
	PIL
	keras

Process Flow:
	detect bike riders from the video
	Run python Object_Detection.py 
	cropped images will be stored in “video_to_image” folder
	Cluster Images
	Run python compare_two_images.py
	Similar images are clustered with user groups
	Crop head part only
	Run python crop_1_by_4.py
	It will Crops the head part the images.
	This scripts creates new folder in every group with name “Cropped/” and stores the all the head parts of the group.
	Helmet detection
	Now test the each group with “helmet_detection_model.hdf5”.
	You can refer “helmet detection.ipynb” file detection of a helmet from an image.

Future work:
	Number plate detection
	Creating GUI to automate the tax payments