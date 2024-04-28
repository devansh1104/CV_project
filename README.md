## Intoduction
SLAM aims to simultaneously estimate the robot's pose and map the environment, while visual odometry focuses solely on estimating the camera (or robot) motion using visual sensor data. While visual odometry can be a component within a SLAM system (e.g., for motion estimation), SLAM provides a more comprehensive solution for robotic localization and mapping tasks. Since we did not have any real world hardware we have an odometer component which can be plugged into a SLAM algorithm for motion estimation and an autonomous guiding system. The most basic difference between visual odometry and vSLAM is of loop closing and global optimisation which is also incorporated in the provided code.
## Problem Statement
Develop a Visual Simultaneous Localization and Mapping (vSLAM) system capable of providing real-time trajectory adjustments for an autonomous agent navigating through outdoor environments. The system must utilize fundamental computer vision techniques for feature extraction, feature matching, motion estimation, and localization to achieve its objectives Provide code implementing the visual odometry and vSLAM algorithms, along with documentation for usage and integration.
## Helper files
Bag_of_words.py : Python code for implementing Bag-of-Words (BoW) image matching using the ORB feature detector and KMeans clustering. BoW is a popular technique in computer vision for image recognition and retrieval tasks.


data_structure.py: Python code for constructing a 3D graph from 2D keypoints obtained from image frames and tracking 3D points using affine transformations


bundle_adjustment_solution.py: Python implementation of a bundle adjustment algorithm, commonly used in computer vision and photogrammetry to refine the parameters of a 3D reconstruction, such as camera parameters and 3D point coordinates, to minimize the reprojection error between observed 2D points and their corresponding 3D points.



## Installations
You can install the required libraries from requirements.txt using the following command
```pip install -r requirements.txt```

## Inferencing
Run the python file for inferecing using the following command.
```python stereo_visual_odometry_w_bundle_adjustment.py```