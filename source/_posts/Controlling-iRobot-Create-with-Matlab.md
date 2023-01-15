---
title: Controlling iRobot Create with Matlab
tags:
  - Create
  - GUI
  - iRobot
  - matlab
  - roomba
cover: https://img.youtube.com/vi/NS7bluhL_fk/0.jpg
date: 2011-08-22 16:44:00
---

### Controlling iRobot Create with Matlab

It is a self-study case. This case refers to first homework project of COMS W4733 COMPUTATIONAL ASPECTS OF ROBOTICS taught by Prof. Peter Allen at Columbia University.  

I use [iRobot Open Interface](http://www.irobot.com/filelibrary/pdfs/hrd/create/Create%20Open%20Interface_v2.pdf) to create a GUI interface in Matlab to control iRobot Create.  The interface takes serial commands from a remote computer and executes them on the robot, returning sensor data as required. In addition, Professor Joel Esposito and Owen Barton at the United States Naval Academy had made a Matlab toolbox for iRobot Create.  Therefore, I can use or modified their code to fit with my GUI program. 

![GUI](http://2.bp.blogspot.com/-HbF3srGERxg/TlPl-dHgY1I/AAAAAAAAAQU/9I6belO25dI/s400/CreateGui1.jpg)



### This Matlab program does those functions: 

- Open - open the COM port for serial communication (unable when connecting)
- Close - close the COM port for serial communication (unable when disconnecting)
- Safe - set iRobot Create to Safe Mode
- Go and Back - move forward and Back
- Stop
- Turn left and right
- Turn Angle - let robot  turn the angle (in degree) inputted by user 
- Go Distance - let robot move the distance  (in meter) inputted by user
- Go Velocity -  let robot move in certain speed seted by user
- Make Square - let robot drive in square whose side is decided by suer
- Read Sensor - Read and Display the state of the wheel, bumper, virtual wall,  and cliff sensors (binary) and read and display the value of the wall signal sensor (0-4095).


### The films of Create GUI:

| {% youtube NS7bluhL_fk %} | {% youtube  v8r25wIZpfU %} |
| ------------------------- | -------------------------- |

Please start screen view in 2nd second and robot view in 0 second.

<!-- more -->
