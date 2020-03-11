**FACE DETECTION BY HAAR CASCADE CLASSIFIER USING OPENCV PYTHON**

**TECHNOLOGY USED:** Python 3.x, Open CV, numpy, Haar Cascade Classifier

**IDE:** Jupyter Notebook

**AIM:** Detect the faces in an image and in a video.

**Motivation:** Computer vision is a field of study which aims at gaining a deep understanding from digital images or videos. Combined with AI and ML techniques, today many industries are investing in researches and solutions of computer vision. Think about the following example: many studies are being carried on to implement security cameras with object detection capabilities.

__Haar Cascade Algorithm:__ It is a machine learning object detection algorithm proposed by Paul Viola and Michael Jones in their paper “Rapid Object Detection using a Boosted Cascade of Simple Features”. It is a machine learning based approach where a cascade function is trained from a lot of positive and negative images (where positive images are those where the object to be detected is present, negative are those where it is not). It is then used to detect objects in other images. OpenCV offers pre-trained Haar cascade algorithms, organized into categories (faces, eyes and so forth), depending on the images they have been trained on. The idea of Haar cascade is extracting features from images using a kind of ‘filter’, similar to the concept of the convolutional kernel. These filters are called Haar features and look like that:

![image](https://user-images.githubusercontent.com/38240162/75839689-4cfde380-5dc1-11ea-9152-ce6483517eaa.png)

The idea is passing these filters on the image, inspecting one portion (or window) at the time. Then, for each window, all the pixel intensities of, respectively, white and black portions are summed. Finally, the value obtained by subtracting those two summations is the value of the feature extracted. Ideally, a great value of a feature means it is relevant.


![image](https://user-images.githubusercontent.com/38240162/75839916-dad9ce80-5dc1-11ea-89f4-efbd158b98fb.png)

**TASKS:**

__FACE DETECTION FROM AN IMAGE__
1. Importing necessary libraries.
2. Read an input image.
3. Build the Haar Cascade classifier. 
4. Detect multi scale faces from the image using the classifier.
5. For every face detected, draw rectangle around it.

__FACE DETECTION FROM A VIDEO__
1. Importing necessary libraries.
2. Capture the input video.
3. Build the Haar Cascade classifier. 
4. For every frame:
	4.1 Detect multi scale faces from the frame using the classifier.
	4.2 For every face detected, draw rectangle around it.
	
__Output__: A snapshots of the output

![image](https://user-images.githubusercontent.com/38240162/75840637-92231500-5dc3-11ea-833f-79247c4eaaf1.png)


[Click here for the code](https://github.com/ktyagi12/OpenCV_Py/tree/master/Face_Detection/code)

[Click here for the input](https://github.com/ktyagi12/OpenCV_Py/tree/master/Face_Detection/input)

[Click here for the output](https://github.com/ktyagi12/OpenCV_Py/tree/master/Face_Detection/output)

[Click here for the classifier](https://github.com/ktyagi12/OpenCV_Py/tree/master/Face_Detection/Classifier)
