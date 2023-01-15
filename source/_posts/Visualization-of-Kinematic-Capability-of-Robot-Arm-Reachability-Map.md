---
title: 'Visualization of Kinematic Capability of Robot Arm: Reachability Map '
tags:
  - matlab
  - reachability map
  - robot arm
cover: https://img.youtube.com/vi/6ifMKsv41Ms/0.jpg
date: 2013-05-08 18:13:00
---

### Visualization of Kinematic Capability of Robot Arm: Reachability Map 

In order to analyze the capability of robot arms, such as PMC1 robot arm, I re-implement the method called Reachability Map in MATLAB.

{% youtube IsbBAy1am3k %}



This method, proposed by researchers in German Aerospace Center (DLR), is to analyze how well do robot arm can reach each local area of whole workspace in how many orientations. The concept is to divide whole workspace of robot arm into several subregion and use following step to compute the reachability of subregions.

| ![Visualization of subregion of PMC1 robot arm](https://1.bp.blogspot.com/-fN6LVnZjH5k/VJGsRmMcUqI/AAAAAAAACkg/0_FaTiDbi1I/s1600/PMC1_subspace.jpg) |
| :----------------------------------------------------------: |
|         Visualization of subregion of PMC1 robot arm         |

I fill the subregion with a inscribed sphere and equally distributed many points (such as 200 points) on the surface of the sphere. each point has different position and orientation. 

![sphere](https://1.bp.blogspot.com/-iTwUWxJipEg/VJGut-U8rhI/AAAAAAAACkw/M70GGhF-7mc/s1600/sphere.jpg)



Then, I compute the inverse kinematics (IK) of the robot arm in each point in each sub-region. Collecting the result of IK to visualize the reachability map of robot arm. 

![Reachability Map of PMC1](https://3.bp.blogspot.com/-K27t2YWgE0w/VJGu8HtiO7I/AAAAAAAACk4/kfoSQs3lLt0/s1600/PMC1_d30_n200.jpg)



The color of sphere stand for the reachability index (RI) of individual subregion. The spheres with cold color index possess more reachability, and spheres with warm color index are lack of reachability.


Furthermore, in order to design the configuration of a dual-arm robot, I adapted the reachability map to quantify the ability of two robot arms to cooperatively reach each position inside there workspace by adjusting the distance and the angle between two arms. Here is the cooperative reachability map of dual-arm robot:



{% youtube 6ifMKsv41Ms %}



Reference:
F. Zacharias, C. Borst, and G. Hirzinger, “Capturing robot workspace structure: representing robot capabilities,” in *2007 IEEE/RSJ International Conference on Intelligent Robots and Systems*, 2007, pp. 3229–3236.

<!-- more -->
