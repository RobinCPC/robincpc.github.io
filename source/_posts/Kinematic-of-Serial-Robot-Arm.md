---
title: Kinematic of Serial Robot Arm
tags:
  - C++
  - kinematic
  - matlab
  - robot arm
  - simulation
cover: https://img.youtube.com/vi/MVmwI4psIFo/0.jpg
date: 2012-11-15 23:29:00
---

### Kinematic of Serial Robot Arm

This is my first work in Precision Machinery Center. I follow the instruction in [1] to write a MATLAB program to demonstrate the forward & inverse kinematic of 6-jointed robot arm.

In this program, user can enter the D-H parameter of the robot on upper left side. By Homogeneous Transformation Matrix, it can do forward kinematic to get the position and orientation of articulated type robot. The result is shown in lower right side.

User also can insert the desired position & orientation and press "IK enter" to get 8 possible solutions of serial robot arm. The result are shown in right side. 

| ![img](https://3.bp.blogspot.com/-YGbJMuzoYuY/VFUST6oynhI/AAAAAAAACck/OZkSg97WW9Q/s1600/kinematic%2BUI.jpg) |
| :----------------------------------------------------------: |
|              GUI of Kinematic Computing Program              |


Furthermore, when user do forward or inverse kinematic, this program will show the configuration of serial robot arm (as match stick) in graph, as below.



![img](https://3.bp.blogspot.com/-4Amal4Zg71A/VFUYMR0CfGI/AAAAAAAACc0/PF18IZO3D0w/s1600/kinematic%2Bgraph.jpg)


Here is the demonstration of this kinematic computing program:

{% youtube MVmwI4psIFo %}



In addition, I also re-implement this program in C++ with MFC.

![img](https://3.bp.blogspot.com/-1bzxTjddLCM/VFUYMQmzFrI/AAAAAAAACc4/F-yNEouLXb4/s1600/kinematic%2BUI%2Bin%2BMFC.jpg)



**Reference**
[1]. Robot Analysis: The Mechanics of Serial and Parallel Manipulators by Lung-Wen Tsai



<!-- more -->
