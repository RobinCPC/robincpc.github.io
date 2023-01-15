---
title: Demo of PMC Robot Teach Pendant
tags:
  - GUI
  - Industrial
  - robot arm
  - robotics
  - Scintilla
  - serial manipulator
  - Teach Panel
  - Teach Pendant
cover: https://img.youtube.com/vi/JmXIHzVw23U/0.jpg
date: 2015-09-16 08:38:00
---

### Demo of PMC Robot Teach Pendant

This is a beta version of teach pendant of PMC Robot Controller.

{% youtube JmXIHzVw23U %}



The hardware (6.5" touch screen with physical buttons) is bought from IEI, and we use it to implement the user interface of teach pendant.

![teach pandent outline1](https://4.bp.blogspot.com/-DWZScRk2PYM/VlULLsDusmI/AAAAAAAAEGc/TLlBYkBQqok/s400/teach_pendant_outline1.jpg)


I, as a project leader, mentor junior engineer to develop user interface of teach pendant and use Git to control software version & record our progress. Meanwhile, I focus on improving the real-time system of controller (manual mode and message alarm).

Basically, this teach pendant has three modes:

1. Teach mode: user can move (jog) robot arm step by step with certain distance and speed in joint-space or Cartesian-space. User can record positions they want for composing motion script later.
   (Please watch above video from 25 sec to 55 sec)



![teach mode](https://3.bp.blogspot.com/-2_xQ5gOsuKs/VlUMnHVfZeI/AAAAAAAAEGw/f8xRAHjyxTc/s640/teach_mode.jpg)



2. Manual mode: user can use PMC robot language to edit motion script of robot arm and run scripts manually (one by one command line. Please watch above video from 1:37 to 2:10 for more detail)



![manual mode](https://1.bp.blogspot.com/-SU2JCLluzZI/VlUMeg-T_iI/AAAAAAAAEGs/tiTRYLz2zeo/s640/manual_mode.jpg)



3. Auto mode: Similar as manual mode, but user can run script continually. (Please watch above video from 2:15 to 2:40 for more detail.)  It also has pages to monitor I/O condition, display message from real-time system and setting tool & base. (Please watch above video from 1:02 sec to 1:08 sec for more detail)



![IO page](https://4.bp.blogspot.com/-9I72esb5B4c/VlUMzzWz7BI/AAAAAAAAEG4/78BRKayqedI/s640/IO_page.jpg)



4. Also, I use Scintilla API to enhance the interface of PMC Robot Language Editor.

   I also wrote the proposal and acquired funding from Taiwan Government for this project.



![Edit page](https://2.bp.blogspot.com/-gp83Nikxsu0/VlUNIGT-5wI/AAAAAAAAEHA/mfs-noUKAbs/s640/edit_page.jpg)


Please watch above video from 1:12 sec to 1:36 sec for more detail about the process of editing robot command.

<!-- more -->
