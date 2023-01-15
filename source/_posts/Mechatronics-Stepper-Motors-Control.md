---
title: Mechatronics - Stepper Motors Control
tags:
  - control
  - Mechatronics
  - Microcontroller
  - motor
cover: false
date: 2011-08-31 13:48:00
---

### Mechatronics - Stepper Motors Control

One of case studies at Mechatronics class at Columbia University taught by Dr. Fred R. Stolfi. The goal of this case study is get an understand of the issues and techniques for stepper motor control using an embedded microcomputer. Stepper motors are the preferred technology for position control system such as those in machine tools.
The main apparatus includes: 

- A microcontroller, PIC16F74 
- A Microchip microcomputer board 
- Two permanent magnet stepper motors (unipolar and bipolar) 
- Four optical interrupters (four sets of LED and Photo Transistor ) 



The film of stepper motors control:

{% youtube f2wJ3UzY3mU %}


The following describes the different modes of motor operation:


**1. Mode 1 - Basic Incremental Motion**
In mode 1, the microcomputer will rotate the stepper motors between the (optical) interrupters sequentially (i.e. only one motor will move at any time). For this mode, when the red button (on microcomputer board) is pressed, the microcomputer will cycle a stepper motor between the two interrupters by shortest path. Full step operation will be used for both motors (unipolar and bipolar)


**2. Mode 2 - Basic Opposed Continuous Motion**
In mode 2, the microcomputer basically controls the motors in full stepping operation continuously (two motors move at the same time) with the motors moving in opposite directions. Both motors start at the horizontal interrupter position. After red button is pressed, both motors are cyclically driven between the two interrupters continuously by the shortest path. If the red button is held down as the motors reach the horizontal interrupters, then motion is stopped. Otherwise the motion continuous. At any time when the motors have stopped moving, a green button press will switch to another mode. A red button press will start this mode again.

**3. Mode 3 - Basic Synchronous Continuous Motion**
In mode 3, the microcomputer basically control the motors in full stepping continuously ( again,two motors move at the same time) with the motors moving in the same direction. The bipolar motors start at the horizontal interrupter position and the unipolar motor start at the vertical interrupter position. After the red button is pressed, both motors are cyclically driven between the two interrupters continuously by the longest path. If the speeds of motors are different, the faster motor must wait at the interrupter position until the slower one reach interrupter position. If the red button is held down as the motors reach the starting position, the motion is stopped. Otherwise the motion continuous. 


**4. Mode 4 - Basic Opposed Continuous Motion - Wave Drive**
In mode 4, the microcomputer basically controls the motors in wave drive motion the same way it was done in Mode 2 (full drive motion). After red button is pressed, both motors are cyclically driven between the two interrupters continuously by shortest path.If the speeds of motors are different, the faster motor must wait at the interrupter position until the slower one reach interrupter position. If the red button is held down as the motors reach the starting position, the motion is stopped. Otherwise the motion continuous.

<!-- more -->
