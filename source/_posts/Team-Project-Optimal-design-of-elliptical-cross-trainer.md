---
title: 'Team Project: Optimal design of elliptical (cross) trainer'
tags:
  - eight-bar
  - elliptical trainer
  - four-bar
  - GUI
  - linkage
  - matlab
  - simulation
cover: https://img.youtube.com/vi/6qxCdixfiII/0.jpg
date: 2011-08-23 03:16:00
---

### Optimal design of elliptical (cross) trainer

This was a team project I participated at Mechanism Design class at National Taiwan University. The goal of this project is optimize the design of elliptical trainer, which is one of fitness equipment we can can see in gym.

The following are what I did:  

* Analyzing and optimal designing of four-bar linkage (Home-use, cheap, and ineffective elliptical trainer)

* Analyze of eight-bar linkage (effective and expensive elliptical trainer, which we can see in gym)





The simulation of four-bar elliptical trainer in Matlab:

{% youtube 97GhadOHFXM %}

The red point is the position of pedal, and the dash ellipse is the trajectory of your foot when using elliptical trainer.
And, this is the real one (four-bar elliptical trainer):

![four-bar type elliptical trainer](https://2.bp.blogspot.com/-C9qTIAVJMA0/TlPdbCjNz3I/AAAAAAAAAQQ/wdM8SXcOQOc/s400/fourBar1.jpg)

We bought this trainer for our project about NTD 2000 (USD65 ).

This is the model for my simulation, and I extracted some useful data from the above simulation:

- The major axis (step length) of dash ellipse is 32.02 cm
- The ratio of major/minor axis of dash ellipse is 1.415 




Next, we went to NTU's gym to find better elliptical trainer, and did a little analysis:
It is a eight-bar type elliptical trainer, and one of its bar is slider. Then, we measured each bar and used it a little while to felt what the difference between the four-bar one. 

Here is  the simulation of eight-bar elliptical trainer in Matlab:

{% youtube 6qxCdixfiII %}



The red point is the position of pedal, and the dash ellipse is the trajectory of your foot when using elliptical trainer.

This is the film of real elliptical trainer:

{% youtube cuV2y6PyxpM %}



I extracted some useful data from the above simulation:

The major axis (step length) of dash ellipse is 47.12 cm

The ratio of major/minor axis of dash ellipse is 2.12

Comparing these two trainer, with our user experience and reference, we find out:

- The longer step length will let people use more type muscle (in different position).
- The bigger ratio of ellipse means the minor axis of ellipse is shorter , so you will not bend your knee to much when using trainer. With shorter minor axis, your motion looks much like skiing not riding bicycle.  



Therefore, longer step length and larger ratio will make more training efficiency. 

Also,from animate of 4-bar type, we can see the tilt angle of pedal is changing largely in every cycle. While, from animate of 8-bar type, we can see the tilt angle of pedal is stable.

As our experience, the stable pedal will let user's ankle feel better.



Also, I used Matlab toolbox - GUIDE to make a GUI version of four-bar simulation:

{% youtube cMqUwASI1J0 %}



<!-- more -->
