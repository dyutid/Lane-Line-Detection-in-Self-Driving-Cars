# Lane-Line-Detection-in-Self-Driving-Cars
This project demonstrates a lane line detection pipeline using Python and OpenCV, designed to identify and highlight lane lines in images. Lane detection is a critical task in computer vision for applications such as autonomous driving and driver-assistance systems.

# Repository Structure

lane_line_detection.ipynb – Jupyter Notebook containing the full pipeline with code, explanations, and visualizations.

test_image.jpg – Sample image to test the lane detection pipeline.

images/ – Folder containing output images generated during each stage of the pipeline, such as grayscale, Canny edges, and final lane detection results.

# Pipeline Overview

The notebook implements a complete lane detection pipeline with the following steps:

1. Image Preprocessing

Convert the input image to grayscale for simplicity.

Apply a Gaussian blur to reduce noise and smooth the image.

2. Edge Detection

Use the Canny edge detection algorithm to identify strong edges likely representing lane lines.

3. Region of Interest (ROI)

Mask a triangular region of the image to focus only on the area of the road where lanes are expected.

4. Hough Transform

Detect straight lines in the ROI based on edge points.

5. Line Optimization

Average and extrapolate the detected line segments to form a single continuous line for the left and right lanes.

6. Overlay Lines

Overlay the optimized lane lines on the original image to visualize the results.

# Skills & Technologies

Python – Main programming language for image processing and pipeline implementation.

OpenCV – Core library for computer vision operations (grayscale conversion, Gaussian blur, Canny edges, Hough Transform).

NumPy – Efficient numerical operations on image arrays.

Matplotlib – Display and plot intermediate and final results.

Jupyter Notebook – Interactive environment for combining code, visualizations, and explanations.

# Highlights

Fully functional lane detection pipeline from raw images to optimized lane lines.

Demonstrates classic computer vision techniques used in autonomous driving systems.

Modular and easy-to-understand code suitable for learning and extending to more advanced projects, such as real-time video lane detection.
