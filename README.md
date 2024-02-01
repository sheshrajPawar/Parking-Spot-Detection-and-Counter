# Parking-Spot-Detection-and-Counter
This repository contains a Python script for detecting parking spots in a video feed and keeping a count of available spots. The script leverages computer vision techniques, connected components analysis, and machine learning to determine the occupancy status of each parking spot.

# Features
1. Connected Components Analysis:
Utilizes OpenCV's connectedComponentsWithStats function to identify connected components in a provided mask, highlighting parking spot areas.
2. Machine Learning Model:
Incorporates a pre-trained machine learning model for classifying parking spot occupancy.
The model is loaded from a pickle file and applied to cropped spot images to determine whether a spot is empty or occupied.
3. Real-time Video Processing:
Reads video frames from a specified path and processes them in real-time.
Implements a step-wise approach to analyzing parking spots and updating their occupancy status.
4. Visualization and Counting:
Annotates the video frames with rectangles representing parking spots, colored based on occupancy status (green for empty, red for occupied).
Displays a dynamic count of available parking spots in the video feed.
5. Utility Functions:
Includes utility functions for calculating differences between frames, extracting parking spot bounding boxes, and determining spot occupancy.
6. Dependencies:
The code relies on popular libraries such as OpenCV, NumPy, and scikit-image.
A machine learning model (stored in a pickle file) is used for spot occupancy classification.


# How it Works:
1.Connected Components Analysis:
The provided mask image undergoes connected components analysis to identify distinct parking spots.

2.Machine Learning Classification:
A machine learning model is applied to cropped spot images to classify each spot as empty or occupied.

3.Real-time Processing:
Video frames are processed in real-time, and parking spots are analyzed at specified intervals.

4.Counting and Visualization:
The script dynamically updates the count of available parking spots and visualizes the occupancy status in the video feed.

5.User Interaction:
The user can exit the video feed display by pressing the 'q' key.

# Model and Utility Functions:
The machine learning model is loaded from a pickle file (model.p).
Utility functions (calc_diff, empty_or_not, get_parking_spots_bboxes) are employed for various operations.




