# Speed-Sign-Detection
This project involves detecting speed limit signs and overspeeding vehicles from a set of milestone images using various computer vision techniques. The project is divided into two milestones, each utilizing different methods for achieving the objectives.

# Milestone 1: Template Matching for Speed Limit Detection
## Objective
To detect speed limit signs from a set of milestone images using template matching and save the results to a CSV file.

## Methodology
  Load Milestone and Template Images: Read the milestone images from the specified directory.
  Template Matching: Use OpenCV's cv2.matchTemplate method to find the best match for each template image within each milestone image.
  Thresholding: Apply a threshold to determine if a speed limit sign is detected.

## Output: 
  Save the results to a CSV file with columns for the image name and detected speed limit.
  
## Results
  The results of this milestone are saved in M1_Output.csv, which contains the detected speed limits for each milestone image.


# Milestone 2: Keypoint Detection and Matching

## Objective
  To enhance the accuracy of speed limit detection by using keypoint detection and matching techniques (ORB and SIFT) and visualize the matching results.

## Methodology
  Load Milestone and Template Images: Read the milestone images from the specified directory.  
  Keypoint Detection and Matching: Use ORB and SIFT detectors to find keypoints and descriptors. Match these keypoints between milestone and template images.
  Homography and Filtering: Apply homography to filter matches and determine the best match for speed limit detection.
  Visualization: Visualize the keypoints and matches on the milestone images.

## Output: 
  Save the results to a CSV file with columns for the image name and detected speed limit.

## Results
  The results of this milestone are saved in M2_Output.csv, which contains the detected speed limits for each milestone image along with visualizations of the matches.


# Dataset
The dataset consists of two main directories:
  Milestone Images: Contains images of roads with potential speed limit signs.
  Template Images: Contains template images of different speed limit signs used for matching.
  
# Outputs
  M1_Output.csv: Output CSV for Milestone 1 with detected speed limits.
  M2_Output.csv: Output CSV for Milestone 2 with detected speed limits and visualizations.
  
# Prerequisites

Python 3.x
OpenCV
NumPy
pandas
matplotlib
pytesseract (for OCR functionality in future milestones)
