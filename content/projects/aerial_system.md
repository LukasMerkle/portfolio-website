---
title: Aerial Manipulation System
type: project
date: 2018-05-00T11:13:20+00:00
weight: 1

thumb:
  description: 
    A fully autonomous UAV that grasps blocks and stacks them on top of each other
  img: drone2.jpeg

highlights:
- Developed strategies to assemble a wall made out of 1.5 kg blocks using a hexcopter and manipulator
- Designed gripping mechanism and control algorithm to grasp blocks with an electromagnet
- Used neural network to perform detection and classification of target objects
- Lead team of 5 graduate students to participate in the third challenge of the MBZIRC competition


info:
  robot_type: Hexacopter using Pixhawk and Jetson
  application: Automated Construction

org:
  name: MRSD Capstone project, Carnegie Mellon University
  link: https://mrsdprojects.ri.cmu.edu/2018teamc/

personal:
  role: Team Lead
  timeframe: September 2018 – present

media:
- type: video
  src: https://www.youtube.com/embed/gDecDPKogvs
  width: 800
  height: 450
  caption: 
    A summary of the work that was achieved during Spring 2019. It includes
    a simulation, block detection and block placement.

- type: image
  src: Func_arch.jpg
  caption: 
      Functional Architecture of the system

- type: image 
  src: drone_setup.png
  caption: 
    Descriptive UAV setup that was developed

- type: video
  src: https://www.youtube.com/embed/gDecDPKogvs
  width: 800
  height: 450
  caption: 
    Position hold based on aruco marker detections 

---

The main goal of this project is to assemble a specified structure, such as a wall, by using a UAV equipped with a manipulator. This system will compete in the third challenge of the MBZIRC competition in Abu Dhabi in February 2020. It makes use of a hexcopter running Pixhawk as a flight controller, an Intel NUC as the main computer and a custom designed manipulator arm attached at the bottom of the drone. 

The overall strategy to build such a structure is as follows: The UAV will identify the location of the blocks with YOLO and will use GPS to navigate to the general region of interest. It then visual servos towards the desired block and grasps it with the electromagnet attached to the manipulator at the bottom of the drone. Similarly, the system uses GPS again to get to the location to build the structure. Finally, it uses a modified visual servoing algorithm to assemble the wall block by block. 