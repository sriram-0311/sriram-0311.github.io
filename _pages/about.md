---
permalink: /
title: "About Me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<p align="justify"> 
Hi! I am a MS Robotics Student from the ECE department at Northeastern University. My net of interests is cast in wide areas, mainly around topics of robot perception, motion planning, visual based SLAM techniques and, certifiably correct algorithms. The cornerstones of my work have always been based on solid mathematical foundations and, efficient and robust coding methodologies.
<br>
I am accustomed to coding languages like C++ and in the use of ROS software. Currently, I am actively learning topics like Multiple View Geometry, Visual inertial fusion, bundle adjustment and vision algorithms for mobile robotics.
<br>
This website/portfolio is a detailed representation of some of my work, feel free to browse around! The tab below is kind of a notice board/bulletin of my current work.
</p>

Current Project I worked on -
-------
### [Scan matching using ICP in C++](https://github.com/aryaman-patel/MobileRobotics5550#scan-matching-using-iterative-closest-point)
This is a personal project I wished to try. In this I have implement the Iterative Closest Point (ICP) algorithm, and use it to estimate the rigid transformation that optimally aligns two 3D pointclouds. The given two pointclouds $X,Y \subset \mathbb{R}^{d}$ have an initial guess $(t_0,R_0) \in SE(d)$ for the optimal rigid registration $y = R_x + t$ aligning $X$ to $Y$. 

This is the resultant point cloud -

![IPC](https://user-images.githubusercontent.com/117113574/211952055-67412be5-07ea-4b9a-ad75-f353488a2d84.png)

In this implementation I have used a library I was fascinated by while going through ORB-SLAM's source code, this library is called [Eigen](https://eigen.tuxfamily.org/) which is a C++ template for linear algebra! 
