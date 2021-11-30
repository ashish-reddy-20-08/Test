# Cheatsheet on Open CV Library

## Video Link : [Cheatsheet on Open CV Library]()

## Installing Necessary Packages
First you need to install python.

Now check the python version and install the openCV

## Reading Images & Videos
As the first step you have to get some images and videos and put it in folder named videos and images.

## Reading Images
We are going to use cv.imread function. What it does is it reads an image from a particular path and returns that image as a matrix of pixels.

If read an image with cv.imread you can use cv.imshow to display the image.

Then we want to add one more parameter which waits for the keyboard input to terminate the new window which is used for display. cv.waitKey(0) Here 0 is used so that the program will wait for an infinite amount of time to get an input from keyboard.


![image](https://user-images.githubusercontent.com/63282184/144033087-7230d4ad-bdfd-485f-a313-03ef03022efa.png)


## Reading Videos
Now about reading video, we will not be using cv.imread() instead we will create variable called capture with cv.VideoCapture(<argument>) function. Here the argument can be integer like 0, 1, 2 if you want to use your camera like webcam or another one. or you can give the path of the video you want to load.

  Since video is not a single frame we have to work on how to display it. Inorder to that we are going to create a while loop. Read the capture object and display them frame by frame.

  After that we make the waitKey wait either for 20 seconds or we specify a key (“d”) is pressed then also it should break out of the loop. After that we have to release the object and destroy all windows.
  
![image](https://user-images.githubusercontent.com/63282184/144033180-292b7708-691c-4f66-aae3-3c0d5e128307.png)


  
## Resize and Rescale
For re-scaling lets write a function that takes in the frame and scale factor. We then resize using cv.resize() function with input parameter frame, dimension .
Then we call the function in the previous read_video file.
