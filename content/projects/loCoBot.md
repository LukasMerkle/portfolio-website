---
title: LoCoBot
type: project
date: 2018-05-00T11:13:20+00:00

thumb:
  description: 
    Scene analysis and manipulation of small blocks using a 5 DoF low cost arm
  img: drone.jpg

highlights:
- Leading a team of 5 Graduate Students to develope a UAV that will compete in the MBZIRC Challenge 2020 in Abu-Dhabi 
- Designed manipulator using permanent electro magnets and its underlying control algorithm
- 

info:
  robot_type: Hexacopter using Pixhawk and Jetson
  application: Manipulation of blocks/ construction

org:
  name: Carnegie Mellon University, MRSD program
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

- type: video 
  src: https://www.youtube.com/embed/JgrY1aPXASY
  width: 800
  height: 600
  caption:
    A visualization of the person tracker in rviz. Blue points near the
    tracked_person coordinate frame are particles from the particle filter;
    other points are 3D points from the depth sensor.

- type: image
  src: person_tracker_block.png
  caption: 
    Block diagram of the perception for the person follower.
    I implemented the Person Tracker section.

- type: image 
  src: person_tracker_telemetry.png
  caption: 
    Visualization of the robot telemetry in rviz. Blue points near the
    tracked_person coordinate frame are particles from the particle filter;
    other points are 3D points from the depth sensor.

---

The main goal of this project is to assemble a specified structure, such as a wall, by using a UAV equipped with a manipulator. This system will compete in the third challenge of the MBZIRC competition in Abu Dhabi in February 2020. It makes use of a Hexcopter running Pixhawk as a flight controller, a Nuc as the main computer and a costomed designed manipulator arm attached at the bottom of the drone.  