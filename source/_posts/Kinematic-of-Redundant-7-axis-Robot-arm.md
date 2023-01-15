---
title: Kinematic of Redundant (7-axis) Robot arm
tags:
  - C++
  - kinematic
  - matlab
  - redundant
  - robot arm
  - robotics
  - serial manipulator
cover: https://img.youtube.com/vi/BZnzIHdAoGo/0.jpg
date: 2013-03-15 02:53:00
---

### Kinematic of Redundant (7-axis) Robot arm

For usual articulated (6-axis) serial robot arm, given the position and orientation of its end-effector,  we can get (at most) 8 possible Inverse kinematic solutions. 

While, for redundant (7-axis) robot arm, when the position and orientation of its tool center point (TCP) are given, it still has one DOF in its elbow to move arbitrarily for other purposes, such as avoiding obstacles. 



{% youtube BZnzIHdAoGo %}


In addition, the kinematic configuration of this kind of robot arms is adopted from the human arm kinematics, whose first three joints work as human's shoulder, the fourth joints works as human's elbow, and last three joints work as human's wrist.



![img](https://4.bp.blogspot.com/-foLMmaehrPc/VFUyg0peziI/AAAAAAAACdU/89aqVDWZtk4/s1600/kinematic%2Bmodel%2Bof%2Bredundant%2Brobot.jpg)



Here, I used PMC 22 robot arm, a 7-axis robot arm, as my research model. For inverse kinematics of PMC 22 robot arm, I used the closed-form method, which is proposed by Dahm, to find the inverse kinematics solution. I re-implement this IK method with MATLAB. The below is the demonstration of kinematic algorithm:

{% youtube hhS-WfOkxYk %}



From above the first figure, given position and orientation of its TCP, we first get the wrist position and derive the elbow circle, which are the possible positions of the elbow, from the vector between the wrist and the shoulder of the robot arm. Then, we choose one of the positions from the elbow circle, and the configuration of the robot arm is fixed by given all constraints on 7 DOFs (TCP and elbow). Finally, we were able to find all of the joint positions by the geometric relation between each joint.
In addition, I use C++ to rewrite this program, and the computing time for each closed-form Inverse Kinematic takes about 30 microseconds.



![img](https://1.bp.blogspot.com/-HBa3YbfjwlY/VFX6PrjqIzI/AAAAAAAACdk/yD8xuVTmbjQ/s1600/CF%2Bkinematic%2BUI%2Bin%2BMFC.jpg)

 

Reference:
P. Dahm and F. Joublin, “Closed form solution for the inverse kinematics of a redundant robot arm,” *Inst. Neuroinf, Ruhr-Univ. Bochum*, no. April 1997.

<!-- more -->
