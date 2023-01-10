---
permalink: /
title: "About Me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
<div style="text-align: justify"> 
Hi! I am a MS Robotics Student from the ECE department at Northeastern University. My net of interests is cast in wide areas mainly around topics robot perception, motion planning and Visual based SLAM techniques.The cornerstones of my work have always been based on solid mathematical foundations and, efficient and robust coding methodologies. 
</div>

My Background 
---
### My Work in Robotics:


### Reasearch:
<div style="text-align: justify">
My undergraduate studies helped me develop excellent fundamentals in applied mathematics,especially in <b>numerical methods</b> for ordinary differential equations and optimization techniques. I applied these skills in my research for solving non-linear ordinary differential equations that represented the continuity, momentum, and energy equations of a nanofluid. I modeled two nanonfluids under conditions like electro-osmosis, magneto-hydrodynamics and
porous medium. I developed my interest in analytical study and gained skills in using MATLAB to solve non- linear equations.
</div>

![Nanofluid](https://user-images.githubusercontent.com/117113574/211640149-5247a47e-2400-47e4-a751-399eb74458dc.png)


<div style="text-align: justify">
<b>Optimization</b> algorithms introduce efficient methods to find optimal parameters for complex equations helpful in studying the dynamics of a robot. I researched developing a new constraint handling method that challenges different evolutionary algorithms used to maximize or minimize objective functions subject to constraints. Using the socio-inspired algorithm of Cohort Intelligence and a modified probability distribution approach, and vectorized coding
adapted from Machine Learning algorithms, I developed an efficient algorithm. I tested this algorithm and compared with different Evolutionary Algorithms for solving advanced manufacturing problems that showed considerable improvement in run-time and for finding the optimal values for the parameters under consideration. The work added to my research experience and improved my skills in MATLAB programming.
</div>



Current Projects
------

### [ICP implementation in C++](https://github.com/aryaman-patel/MobileRobotics5550#scan-matching-using-iterative-closest-point)

Make sure your system has the latest library for [Eigen](https://eigen.tuxfamily.org/index.php?title=Main_Page) and [PCL](https://pointclouds.org/) installed. 
To run the source file `ICP.cpp` use the following commands:
```
g++ -std=c++17 -I/usr/include/eigen3 ICP.cpp -o ICP -O2 -DNDEBUG
```
Here, the flags: `-O2` used in the compiler to optimize the genrated code for the maximum performance. Thie flag enables a number of optimization options that can improve the speed and efficiency. The flag `-DNDEBUG` tells the compiler to disable debugging information. This improves the performance of the code by eliminating the checks and other overheads that are not necessary to build. 
 
The `ICP.cpp` code creates a resultant file called `result.txt` that stores the resultant points of the pointcloud.

In order, to visualize the point cloud I have written an implementation using the [PCL](https://pointclouds.org/) library. Run the following commands:
For the code to run make sure to move a copy of `pclX.txt`, `pclY.txt` and `result.txt` file to the `build` folder.

```
cd build
cmake ..
make
./point_cloud_visualization
```
The resultant point cloud in comparision to the original ones looks like this:
![PCL](https://user-images.githubusercontent.com/117113574/210670258-9c4e113f-fc7f-473a-b349-026e137d9d5f.png)





