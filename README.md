# linear-graph-slam
This project was the third and final for completing the Udacity Computer Vision Nanodegree.  

## Landmark Detection & Robot Tracking (SLAM)

</b>Project Overview

</b>In this project, you'll implement SLAM (Simultaneous Localization and Mapping) for a 2 dimensional world! 
You’ll combine what you know about robot sensor measurements and movement to create a map of an environment from only sensor and 
motion data gathered by a robot, over time. SLAM gives you a way to track the location of a robot in the world in real-time and 
identify the locations of landmarks such as buildings, trees, rocks, and other world features. 

This is an active area of research in the fields of robotics and autonomous systems.

## Initialize Constraints

One of the most challenging tasks here will be to create and modify the constraint matrix and vector: omega and xi. In the second notebook, you saw an example of how omega and xi could hold all the values the define the relationships between robot poses `xi` and landmark positions `Li` in a 1D world, as seen below, where omega is the blue matrix and xi is the pink vector.

<img src='images/motion_constraint.png' width=50% height=50% />


In *this* project, you are tasked with implementing constraints for a 2D world. We are referring to robot poses as `Px, Py` and landmark positions as `Lx, Ly`, and one way to approach this challenge is to add *both* x and y locations in the constraint matrices.

<img src='images/constraints2D.png' width=50% height=50% />

