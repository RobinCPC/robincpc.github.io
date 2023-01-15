---
title: Demonstration of PMC Robot Simulator
tags:
  - C++
  - Industrial
  - robot arm
  - robotics
  - serial manipulator
  - simulation
cover: https://img.youtube.com/vi/mwVbDKZQgiw/0.jpg
date: 2013-07-03 01:26:00
---

### Demonstration of PMC Robot Simulator

In Precision Machinery Research and Development Center (PMC), I also work on developing simulators for our industrial robots.

{% youtube mwVbDKZQgiw %}



It is also the human machine interface (HMI) of our industrial robot, such as serial robot arm, SCARA robot, Delta robot. 



| ![6-axis_HMI](https://1.bp.blogspot.com/-8OVRNBd76mU/VJXH0ZaGgvI/AAAAAAAACls/GlYQwwgJydM/s1600/6AXIS_HMI.jpg) |
| :----------------------------------------------------------: |
|                       Serial Robot Arm                       |

| ![SCARA_HMI](https://1.bp.blogspot.com/-XTYXIlNUycc/VJXIZoWbk8I/AAAAAAAACl0/eBNyimIJrX8/s1600/SCARA_HMI.jpg) |
| :----------------------------------------------------------: |
|                         SCARA Robot                          |

The simulator is written in C++, and its graphical user interface (GUI) is developed with MFC. The purpose of this simulator is to work as the teaching panel of commercial industrial robot arm, which include function like: 

- Jog control of each joint and end-effector
- Show information of robot (angle of each joint, position and orientation of end-effector)
- Read and execute PMC Robot Langue
- Render virtual robot arm. 

In order to render virtual robots and simulate motion of the robot, we use open source CAD kernel "Open CASCADE" to develop functions to read CAD file of robots and define rotating axis & position of each joint.



We also provide our simulator to our collaborator Prof. Kao-Shing Huang at NationalSun Yet-Sen University. They used it to demonstrate their research about inverse kinematics solutions for redundant robots.

{% youtube X-ON6uHaug0 %}



Reference:

[Open CASCADE](http://www.opencascade.org/)

<!-- more -->
