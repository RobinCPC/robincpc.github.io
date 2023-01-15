---
title: PMC 14-axis Industrial Dual-Arm Robot
tags:
  - dual-arm
  - Industrial
  - redundant
  - robot
  - robot arm
cover: https://img.youtube.com/vi/C8_pQGrsqw8/0.jpg
date: 2014-08-11 01:12:00
---

### PMC 14-axis Industrial Dual-Arm Robot

This is a 14-axis Industrial Dual-Arm Robot created by Precision Machinery Research & Development Center (PMC). It is also the first industrial robot built from Taiwan. It has humanoid arms to accomplish complicated tasks with high flexibility targeted for industrial use. 

{% youtube C8_pQGrsqw8 %}


This newly designed robot, PMC 14-axis dual-arm robot, has exhibited in 2014 “Taiwan Automation Intelligence and Robot Show” (TAIROS, the biggest exhibition in Taiwan).

![img](https://3.bp.blogspot.com/-zCtweFH_qY0/VJWurlMeVsI/AAAAAAAAClI/NsciluSU5Us/s1600/PMC%2Bsync.jpg)


In this project, I developed closed-form inverse kinematic algorithm for redundant (7-axis) robot arm in order to let each robot arm has a high degree of freedom like the human arm.([detail](http://chienpinchen.blogspot.tw/2013/03/kinematic-of-redundant-7-axis-robot-arm.html)) 

![img](https://2.bp.blogspot.com/-foLMmaehrPc/VFUyg0peziI/AAAAAAAACdY/Lt8bTqFpnIM/s1600/kinematic%2Bmodel%2Bof%2Bredundant%2Brobot.jpg)


The reachability map was adapted here to design the configuration of a dual-arm robot by adjusting the distance and the angle between its two arms. The reachability map, published by the researchers in German Aerospace Center (DLR), is a method to quantify the ability of a robot arm to reach each position inside its workspace.([detail](http://chienpinchen.blogspot.tw/2013/05/visualization-of-kinematic-capability.html))

![img](https://3.bp.blogspot.com/-IHriPmiiE2Y/VIND-U6ICxI/AAAAAAAACfU/pYLlC4XK-Qg/s1600/Reachability%2BMap%2Bof%2BDual-arm%2BRobot.jpg)


I also worked on developing the multi-robot control cooperative functions in the real-time system for our dual-arm robot. The cooperative functions include:

**Synchronization**



- Program Synchronization


**Geometric Coupling**



- Load Sharing

{% youtube MwkFAOxRlG4 %}



- Master/Slave

{% youtube cYK7M2Y8dfA %}



In addition, I used open source CAD kernel "Open CASCADE" to render virtual robots inside the Human Machine interface of our robot controller.

[![img](https://4.bp.blogspot.com/-7F8OmN2nFSQ/VINGSXvIZoI/AAAAAAAACfg/p2Z6mRquGvM/s1600/daul-arm%2BHMI_4.jpg)](https://4.bp.blogspot.com/-7F8OmN2nFSQ/VINGSXvIZoI/AAAAAAAACfg/p2Z6mRquGvM/s1600/daul-arm%2BHMI_4.jpg)


Furthermore, I extend PMC real-time controller to control three robots in one PC-Based Controller, and I use three robots to perform Load Sharing & Master/Slave together.



{% youtube gvB1T9lgRCw %}

(Exhibited in 2015 TAIROS)

<!-- more -->
