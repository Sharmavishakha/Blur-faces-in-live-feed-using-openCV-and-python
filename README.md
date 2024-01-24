# Blur-faces-in-live-feed-using-openCV-and-python
## Step 1 – Importing required libraries
* Importing cv2 for Image operations.
* Importing Numpy for array operations.
## Step 2 – Defining the Blur function
Here we are defining the Blur function.
It takes 2 arguments, the image and the blur factor (k).
Then we are simply calculating the kernel height and kernel width by dividing the height and width by the blur factor. The smaller the kw and kh, the higher the blurring will be.
Then we are simply checking if kw and kh are odd or not, if they are even then simply subtract 1 from them to make them odd.
Then simply we are applying the Gaussian Blur to our Image and return it.
## Step 3 – Defining pixelate_face function
This is a function that simply adds a pixelated effect to blurred Images.
## Step 4 – Let’s Blur faces in the Live feed
The factor here defines the amount of blurring.
Defining a cascade Classifier object to detect faces.
Download the haarcascade_frontalface_default.xml file.
Then simply run an infinite loop that reads the images from the webcam, detects faces in them, and then replaces that face part with pixelated faces.
