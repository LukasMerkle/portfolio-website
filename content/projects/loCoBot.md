---
title: LoCoBot
type: project
date: 2018-05-00T11:13:20+00:00
weight: 2
thumb:
  description: 
    Scene analysis and manipulation of small blocks using a 5 DoF low cost arm
  img: LoCoBot2.jpg

highlights:
- Developed control algorithms of a 5 DoF robotic arm to perform manipulation tasks
- Implemented vision system to identify small blocks‘ center, orientation and color 
- Improved robot“s precision by adding visual servoing towards the center of blocks
- Combined implementations to perform scene analysis of a given structure to rebuild it on the other side of the robot 

info:
  robot_type: 5 DoF Manipulator Arm
  link: https://www.pyrobot.org/
  application: Manipulation of small objects

org:
  name: Robot Autonomy course, Carnegie Mellon University

personal:
  role: Computer Vision and Control Engineer 
  timeframe: February 2019 – May 2019

media:
- type: video
  src: https://www.youtube.com/embed/T2Kym57aCQA
  width: 800
  height: 450
  caption: 
    Demonstration of block stacking, scene analysis and reconstruction of block configuration

- type: image
  src: mask.png
  caption: 
    Mask from block segmentation based on color and contour
    
- type: video
  src: https://www.youtube.com/embed/w3A3Ud1HF5o
  width: 560
  height: 315
  caption: 
    Implementation of a RRT Planner in Simulation

---

This project was all about exploring what can be done with a low cost robot that does not have the accuracy and precision of a industrial manipulator. First, forward and inverse kinematics were implemented such that the arm can move to any given x-y-z position in its reach. Next, a vision pipeline using a Realsense was implemented. It was able to segment out green, blue and red blocks based on their color and shape and determined its location in the robot frame. With this method, it was possible to grasp these blocks and place them at desired locations.

However, due to the inaccuracy of the arm, this was not satisfying since the arm did not always grasp the blocks in the middle, which lead to errors while placing them. To improve this, visual servoing was implemented using a second camera attached at the wrist of the arm. The manipulator was now able to go to a roughly correct location from the vision algorithm, to servo towards the center of the block until it converged and to grasp it in the middle.

Finally, a similar method was used the analyze a given block structure on one side of the robot and replicate it on the other side of the arm using all methods described above. The robot detects the location of each block using the real sense. It then identifies their exact locations with visual servoing and adds an offset to them to shift them to the other side of the robot. At last, it picks them up using visual servoing and places them at the new desired locations.
