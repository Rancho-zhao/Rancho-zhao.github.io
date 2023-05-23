---
title: "A Robot Grasping System Using RGB-D Data Based on Depth Completion and 6D Pose Estimation"
collection: projects
type: "Projects"
permalink: /projects/2021-06-05-project-grasp
date: 2021-06-05
---

I design a robot grasping system using RGB-D (D means depth) data based on depth completion and 6D pose estimation.

As the following figure shows, this system includes three modules: Information Process, Planning Execution, and User Interaction.

## Information Process

The function of this module is to provide the pose of grasped objects to the planning execution module based on the RGB-D input from Real-Sense camera.

### Depth Completion

The main information we capture is RGB-D data. However, due to the physical limitations of existing sensors, invalid or distorted noise often appears in the obtained depth data, which can seriously affect the subsequent use of depth information. Therefore, it is necessary to consider improving the obtained data information, and deep completion methods can effectively improve the depth information.

I have studied a method based on ClearGrasp, as shown in the following figure. Firstly, the input color image is used, and normal estimation, edge detection, and object segmentation networks are used to obtain information including surface normals, occluded boundaries, and object masks; Then, according to this set of information and the initial depth map, global optimization is carried out to obtain the completed depth map.

Although the ClearGrasp method is very good, on the one hand, it is targeted at transparent objects, and on the other hand, it requires a large dataset for training and a high workload. Therefore, I conducted a secondary development suitable for this project. The main steps are raw data processing, modifying depth information, estimating surface normal vectors and edges, and applying the depth2depth algorithm.

- Firstly, adjust the size of the input color map and depth map to the set values. Afterwards, set the invalid points, noise points, etc. in the depth information to zero. At the same time, limit the points in the depth map that are not within this range based on the set maximum and minimum depth values. 

- Then, segment the target object on the input color information, and set the points on the depth information that correspond to the target object as null values based on the obtained results. From this, a depth map of the position of the target object with some voids was obtained, and a certain degree of filtering processing was performed to remove pixels closer to the camera.

- After the above processing steps, the next step is to use the information extracted from the aligned color map to complete the depth map, which is to estimate the surface normal vector and occluded boundaries based on the color information. 

- After the above two information (surface normal vector and occluded boundary) are obtained, they are combined with the depth information, and global optimization is carried out using the depth_depth algorithm. Then, Bilateral filter is carried out to obtain the completed depth map.

### 6D Pose Estimation

To obtain the objects' pose, I opt to use DenseFusion, the SOTA method recently, and improve it in some details to suit my project.

The main network of DenseFusion is an RGB-D fusion network, which inputs color information and performs object instance segmentation to obtain image blocks and point clouds containing the target object. Then, the image blocks and point clouds are processed separately to obtain color embedding and geometric embedding. The fused information is used to estimate the initial pose of the target object. Then, an iterative optimization network is used to perform more refined optimization on the initial pose.

The original method selected the pose estimation value with the highest confidence as the output, which resulted in a certain degree of dependence on a single confidence level. Therefore, my improvement for it is to select a set of confidence levels within a certain range and weighted sum the attitude estimates corresponding to each confidence level within the set. In specific applications, the selection of a certain range is based on the highest confidence level to set the threshold.

## Planning Execution

I use a python package named ***urx*** to control UR5 robot.

## User Interaction

I designed a visual interface for human-computer interaction, mainly including start button, select button, display depth completion results, instance segmentation results, and pose estimation results.

## Module Communication

For communication between various modules, a combination of ROS and socket is used due to the use of two hosts, UR5 robots, and docker containers. The specific relationship between each node is shown in the figure.