**EYE DETECTION BY HAAR CASCADE CLASSIFIER USING OPENCV PYTHON**

**TECHNOLOGY USED:** Python 3.x, Open CV, numpy, Haar Cascade Classifier

**IDE:** Jupyter Notebook

**AIM:** Detect the eyes on the face in a video.

**Motivation:** Computer vision is a field of study which aims at gaining a deep understanding from digital images or videos. Combined with AI and ML techniques, today many industries are investing in researches and solutions of computer vision. Think about the following example: many studies are being carried on to implement security cameras with object detection capabilities.

__Haar Cascade Algorithm:__ It is a machine learning object detection algorithm proposed by Paul Viola and Michael Jones in their paper “Rapid Object Detection using a Boosted Cascade of Simple Features”. It is a machine learning based approach where a cascade function is trained from a lot of positive and negative images (where positive images are those where the object to be detected is present, negative are those where it is not). It is then used to detect objects in other images. OpenCV offers pre-trained Haar cascade algorithms, organized into categories (faces, eyes and so forth), depending on the images they have been trained on. The idea of Haar cascade is extracting features from images using a kind of ‘filter’, similar to the concept of the convolutional kernel. These filters are called Haar features and look like that:

![image](https://user-images.githubusercontent.com/38240162/75839689-4cfde380-5dc1-11ea-9152-ce6483517eaa.png)

The idea is passing these filters on the image, inspecting one portion (or window) at the time. Then, for each window, all the pixel intensities of, respectively, white and black portions are summed. Finally, the value obtained by subtracting those two summations is the value of the feature extracted. Ideally, a great value of a feature means it is relevant.


![image](https://user-images.githubusercontent.com/38240162/75839916-dad9ce80-5dc1-11ea-89f4-efbd158b98fb.png)

**TASKS:**

EYE DETECTION FROM A VIDEO

1. Import the necessary libraries.
2. Capture the input video and generate the output video object.
3. Build the Face and Eyes Haar Cascade classifier. 
4. Detect the faces in every frame of the video using the Face Haar Cascade Classifier.
5. For every face detected in the frame:
	
   5.1 Define the region of interest as the face by drawing a rectangle around the face.
	
   5.2 Detect the multi-scale eyes from the region of interest.
	
   5.3 Draw a rectangle around the eyes detected on the face of every frame.

[Click here for the code](https://github.com/ktyagi12/OpenCV_Py/tree/master/Eye_Detection/code)

[Click here for the input](https://github.com/ktyagi12/OpenCV_Py/tree/master/Eye_Detection/input)

[Click here for the output](https://github.com/ktyagi12/OpenCV_Py/tree/master/Eye_Detection/output)

[Click here for the classifier](https://github.com/ktyagi12/OpenCV_Py/tree/master/Eye_Detection/Classifier)
