**ROAD LANE DETECTION FROM AN IMAGE AND VIDEO USING OPENCV PYTHON**

**TECHNOLOGY USED:** Python 3.x, Open CV

**IDE:** Jupyter Notebook

**MOTIVATION:** Identifying lanes of the road is very common task that human driver performs. This is important to keep the vehicle in the constraints of the lane. This is also very critical task for an autonomous vehicle to perform. And very simple Lane Detection pipeline is possible with simple Computer Vision techniques

**AIM:** Detect the road lanes from an image and a video input.

**TASKS:**

ROAD LANE DETECTION FROM AN IMAGE
1. Importing needed libraries.
2. Read the road image.
3. Detect the edges of the road using Canny Edge Detector.
	Canny Edge Detection: It is an algorithm that detects edges based on gradient change. Not that the first step of Canny Edge detection is image smoothing with default kernel size 5.
4. Define the region of interest. Mask the road except the region of interest.
	Even after applying Canny Edge Detection, there are still many edges that are detected which are not lanes. Region of Interest is a polygon that defines area in the image, from where edges we are interested
	
5. Draw line on the detected edges using the Probabilistic Hough Lines Transform.
	Hough Transform is the technique to find out lines by identifying all points on the line. This is done by representing a line as point. And points are represented as lines/sinusoidal(depending on Cartesian / Polar co-ordinate system). If multiple lines/sinusoidal pass through the point , we can deduce that these points lie on the same line.
	
**Output**: Stepwise images for detecting the lanes
![image](https://user-images.githubusercontent.com/38240162/75841587-03fc5e00-5dc6-11ea-9fba-0ea17a547813.png)


![image](https://user-images.githubusercontent.com/38240162/75841606-11194d00-5dc6-11ea-852b-613de40d1dc0.png)


![image](https://user-images.githubusercontent.com/38240162/75841621-1b3b4b80-5dc6-11ea-92be-fa6f5a8af958.png)


![image](https://user-images.githubusercontent.com/38240162/75841646-27bfa400-5dc6-11ea-9ee1-61576fee2bad.png)



ROAD LANE DETECTION FROM A VIDEO
1. Importing needed libraries.
2. Capture the input video and generate the output video object.
3. For every frame:
	
      3.1 Detect the edges of the road using Canny Edge Detector.
	
      3.2 Define the region of interest. Mask the road except the region of interest.
	
      3.3 Draw line on the detected edges using the Probabilistic Hough Lines Transform.

__Output__: Detecting the lanes from a video.

![image](https://user-images.githubusercontent.com/38240162/75842265-c567a300-5dc7-11ea-97a9-9bf596b1ac95.png)

[Click here for code](https://github.com/ktyagi12/OpenCV_Py/tree/master/Road_Lane_Detection/code)

[Click here for input](https://github.com/ktyagi12/OpenCV_Py/tree/master/Road_Lane_Detection/input)

[Click here for output](https://github.com/ktyagi12/OpenCV_Py/tree/master/Road_Lane_Detection/output)
