**MAGIC CLOAK**

**PROGRAMMING LANGUAGE USED:** Python 3.x, Open CV

**IDE:** Jupyter Notebook

**AIM:** To make the panda invisible from the frame. 

__Note__: Stay away from frame until video window pops up for the background image to be created.

__TASKS:__
1. Importing needed libraries and generate the output video
2. Capture and store the background for each frame.
3. Detecting the blue portion in each frame
4. Replacing the blue portion with a mask image in each frame
5. Producing the invisible output

__How the Code is implemented__: 

The code has been written to recognize BLUE color as cloak for now.

You can change the color bound according to yourself.The color range for HSV value are available here. For HSV, Hue range is [0,179], Saturation range is [0,255] and Value range is [0,255]. Different softwares use different scales. So if you are comparing OpenCV values with them, you need to normalize these ranges.

* Key Feature: Masking
  ```
  mask1 = cv2.inRange(hsv, lower_range, higher_range)
  ```
The above forms a mask of the area we want to make invisible to frame-feed.

* The next major task is to extract the above mask from the frame, background and foreground.

__Output__: Snapshot of the output video

![image](https://user-images.githubusercontent.com/38240162/75841371-7a4c9080-5dc5-11ea-890d-92d36aa0b6a6.png)

![image](https://user-images.githubusercontent.com/38240162/75841467-b253d380-5dc5-11ea-8d13-7fbbc71bbfea.png)



[Click here for code](https://github.com/ktyagi12/OpenCV/tree/master/Magic%20Cloak/code)

[Click here for output](https://github.com/ktyagi12/OpenCV/tree/master/Magic%20Cloak/output)

REFERENCES: https://github.com/asr-aditya/Harry-Potters-Invisible-cloak?files=1
