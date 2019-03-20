# **Finding Lane Lines on the Road** 
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

<img src="examples/laneLines_thirdPass.jpg" width="480" alt="Combined Image" />

Overview
---

The following project is the first project of the Udacity- Self-Driving Car Engineer Nanodegree. The aim of this project was to implement a pipeline to detect lanes on the road. The pipeline was first tested on a series of images and then on a video stream.

The following pipeline was used to obtain a satisfactory and annotated video of lanes on an highway.

1. Image is read using OpenCV
2. The image is converted in Grayscale
3. Gausian Filter is applied on the grayscale image.
4. Canny edge detection is performed on the image.
5. A region of interest is selected and a mask is created from it.
6. Using hough transform lines are detected on the image.
7. The lines obtained are interpolated to mark the lanes properly.
8. The pipeline for single image is applied on a video which is just series of images.


### Software Requirements:

* [Jupyter Notebook](https://jupyter.org/install.html)
* [Python 3](https://www.python.org/downloads/)
 

### Python Libraries

* Matplotlib
* OpenCV
* Numpy 
* MoviePY
* Ipython

## Functions and Algorithms used

1. [Gaussian Blur](https://docs.opencv.org/3.1.0/d4/d13/tutorial_py_filtering.html)
2. [Grayscaling Image](https://docs.opencv.org/3.0-beta/doc/py_tutorials/py_gui/py_image_display/py_image_display.html)
3. [Creating mask on region of interest](https://stackoverflow.com/questions/25074488/how-to-mask-an-image-using-numpy-opencv)
4. [Hough Transform](https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_imgproc/py_houghlines/py_houghlines.html)

