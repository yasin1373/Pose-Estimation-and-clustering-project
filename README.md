# Pose Estimation

This Jupyter notebook implements a pose estimation model using OpenCV, MediaPipe, scikit-learn, and other Python libraries.

## Overview

The notebook performs the following:

- Initializes a MediaPipe pose detection model to detect 33 anatomical landmarks.
- Captures video from a webcam and processes each frame.
- Detects pose landmarks in each frame using the MediaPipe model.
- Stores the landmark coordinates from each frame in a list. 
- Performs k-means clustering on the landmark coordinates to identify common poses.
- Saves the cluster labels to a CSV file.

## Requirements

The notebook requires the following Python packages:

- OpenCV
- MediaPipe
- scikit-learn
- pandas 

## Usage

To use the notebook:

1. Install requirements
2. Run the notebook cell-by-cell
3. Point webcam at different poses to capture data
4. Clustering will identify common poses
5. Cluster labels are saved to `pose_clusters.csv`

The resulting CSV file contains cluster labels for each frame's pose. This can be used as training data for a custom pose classification model.
