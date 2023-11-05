---
permalink: /
title: "About Me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi! I'm Aryaman Patel, a robotics engineer pursuing my MS in Robotics at Northeastern University. I currently work as a research assistant at [NEURAL](https://neural.lab.northeastern.edu/) ([Northeastern University Robust Autonomy Lab](https://neural.lab.northeastern.edu/)) headed by [Prof. David Rosen](https://david-m-rosen.github.io/) where my focus is on improving visual SLAM systems for autonomous robots.

Specifically, I have been working extensively on building Factor Graphs for Bundle Adjustment Problems for computationally efficent mapping in large environments for a multi-camera based visual-inertial navigation system. I also implemented a Bag of Words based visual place recognition module for long-term data association and loop closure detection in a multi-sensor navigation system.

Outside of my core research, I enjoy working on computer vision projects related to image restoration, intrinsic image decomposition, and 3D scene understanding. These include image deblurring, shadow decomposition, stereo depth mapping, and more. I am passionate about pushing the boundaries of visual perception to enable reliable autonomy in the real world. You can view some of my work on [GitHub](https://github.com/aryaman-patel) or learn more about my current robotics research at [NEURAL](https://neural.lab.northeastern.edu/).

I will complete my MS in Robotics in 2024 and continue pursuing my dream of developing autonomous systems that can operate safely and effectively in complex, unlabeled environments.

![Screenshot-from-2023-10-02-18-15](https://github.com/aryaman-patel/aryaman-patel.github.io/assets/117113574/094c4e0d-8dbe-48a9-86dd-f7f379582ce5)

## Latest Work

### Multi-Camera Visual Interial Navigation

This project was in collaboration with Toyota Research Institute. The deigned system is capable of mapping an environment and use the generated maps for precise heading estimation for the downstream tasks of control. Our team used a multi-camera, IMU and GPS fusion to obtain an order of magnitude sparse map of the environment. The part that enable this precise localization is due to the accurate Visual Place Recognition System with loop closure that reduces the drifts during the mapping secession. To optimize with computational efficiency over large environments, I implemented reduced camera model, which is an elimination procedure corresponding to the Schur complement, which allows the solving of linear system in a subset of variables



### Scan matching using ICP in C++ [GitHub](https://github.com/aryaman-patel/MobileRobotics5550#scan-matching-using-iterative-closest-point)

Implementing the Iterative Closest Point (ICP) algorithm, and use it to estimate the rigid transformation that optimally aligns two 3D pointclouds. The given two pointclouds $X,Y \subset \mathbb{R}^{d}$ have an initial guess $(t_0,R_0) \in SE(d)$ for the optimal rigid registration $y = R_x + t$ aligning $X$ to $Y$.

This is the resultant point cloud -

![IPC](https://user-images.githubusercontent.com/117113574/211952055-67412be5-07ea-4b9a-ad75-f353488a2d84.png)
