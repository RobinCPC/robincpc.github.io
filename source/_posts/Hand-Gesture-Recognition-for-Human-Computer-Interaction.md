---
title: Hand Gesture Recognition for Human Computer Interaction
tags:
  - Computer Vision
  - hand gesture
  - HCI
  - OpenCV
  - PyAutoGUI
  - Python
cover: https://img.youtube.com/vi/cEqN8qZB-v4/0.jpg
date: 2016-03-23 06:23:00
---

### Hand Gesture Recognition for Human Computer Interaction

This was a final project I participated at Computer Vision class at the University of California, Santa Cruz. The goal of this project is  to use OpenCV in Python to implement hand tracking and gesture recognition to control mouse events. 

In the following video, I use hand gestures to manipulate (such as rotate, zoom, and pan) WebGL 3D objects.

{% youtube cEqN8qZB-v4 %}



The following is draft flow chart of project program:

![Process Pipeline](https://3.bp.blogspot.com/-OmSSAzhKk5w/VvHCwb2Y7EI/AAAAAAAAEIo/dQoPryQaAocGV77U4O9rwu4adKGtu9x7Q/s640/program_flow.png)

The source code of this project: 
https://github.com/RobinCPC/CE264-Computer_Vision 



Some material for each subtasks

- [x] Row Image Input

   * [GUI feature in OpenCV](http://docs.opencv.org/3.0-last-rst/doc/py_tutorials/py_gui/py_table_of_contents_gui/py_table_of_contents_gui.html#py-table-of-content-gui)

- [x] Blur, Skin Detection, Morphology, Background Subtraction

    * [Change BGR to HSV or YCrCb](http://docs.opencv.org/3.0-last-rst/doc/py_tutorials/py_imgproc/py_colorspaces/py_colorspaces.html#converting-colorspaces)
    * [Do medianBlur](http://docs.opencv.org/3.0-last-rst/doc/py_tutorials/py_imgproc/py_filtering/py_filtering.html#filtering)
    * [Do erode and dilate](http://docs.opencv.org/3.0-last-rst/doc/py_tutorials/py_imgproc/py_morphological_ops/py_morphological_ops.html#morphological-ops)

- [x] Hand Contour Extraction

    * [Draw Contour and Find Convex Hull or Convexity Defects](http://docs.opencv.org/3.0-last-rst/doc/py_tutorials/py_imgproc/py_contours/py_table_of_contents_contours/py_table_of_contents_contours.html#table-of-content-contours)

- [x] Gesture Recognition

    * [Find out how many fingers show up](http://docs.opencv.org/3.0-last-rst/doc/py_tutorials/py_imgproc/py_contours/py_contours_more_functions/py_contours_more_functions.html#contours-more-functions)

- [x] Hand Position Tracking

    * [Dynamically change center of ROI] (http://docs.opencv.org/3.0-last-rst/doc/py_tutorials/py_imgproc/py_contours/py_contour_features/py_contour_features.html#contour-features) 

- [x] Input Control

    * [PyAutoGUI](http://pyautogui.readthedocs.org/en/latest/cheatsheet.html)
    * [PyUserInput](https://github.com/SavinaRoja/PyUserInput)
    
    > Note: PyAutoGUI work well in Windows system for me. Ubuntu: got issue (invisible cursor move)

    For install PyAutoGUI on Linux (for python 2.x):
    
    ``` bash
    # install x-lib and scrot (pip not work for me)
    $ sudo apt-get install  python-xlib
    $ sudo apt-get install scrot
    
    # skip install python-tk and python2.x-dev (already had)
    # install Pyautogui
    $ sudo pip install pyautogui
    ```
    
    For install PyAutoGui on Window (for python 2.x):
    Open cmd.exe
    
    ```powershell
    # Install pillow first (PIL module may cause error during install)
    C:\Python27\Scripts\pip.exe install pillow  
    C:\Python27\Scripts\pip.exe install pyautogui
    ```
    Turn off Windows UAC


## Reference

* Hui-Shyong Yeo; Byung-Gook Lee; Hyotaek Lim, "Hand tracking and gesture recognition system for 
  human-computer interaction using low-cost hardware", Multimedia Tools and Applications, Vol. 74, 
  Issue 8, Apr. 2015, On page(s) 2687-2715.

* http://vipulsharma20.blogspot.com/2015/03/gesture-recognition-using-opencv-python.html

<!-- more -->
