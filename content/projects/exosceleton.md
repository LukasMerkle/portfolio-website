---
title: Hip Exoskeleton
type: project
date: 2018-05-00T11:13:20+00:00
weight: 8
thumb:
  description: 
    Simulation of hip exoskeleton for elderly to prevent falling 
  img: bio_thumb2.png

highlights:
- Implemented a Neuromuscular Locomotion Model using MATLAB Simulink to simulate human walking
- Induced external disturbances to simulate falling in the elderly
- Improved stabiliy by adding PD controller at the hip to prevent falling

info:
  robot_type: Simulation of Medical Robot
  application: Medical Industry

org:
  name: Biomechanics and Controls Course, Carnegie Mellon University

personal:
  role: Team Lead, Modelling and Controls engineer 
  timeframe: February 2019 – May 2019

media:
- type: video
  src: https://www.youtube.com/embed/T2jrt6l4vP4
  width: 800
  height: 600
  caption:
    Simulated effects of neural delay and muscle deterioration that causes elderly falling. Regained gait stability is achieved by a PD controller at the hip, which simulates a hip exoskeleton
- type: image
  src: bio_diagram.png
  caption: 
      Diagram of the Neuromuscular Locomotion Model's overall implementation
- type: image
  src: noPD_f.jpg
  caption: 
      Effects of neural delay and muscle deterioration WITHOUT PD controller

- type: image
  src: pd_noW_f.jpg
  caption: 
      Effects of neural delay and muscle deterioration WTIH PD controller

---

The purpose of this project was to investigate how a hip exoskeleton can prevent falling in elderly. First, a Neuromuscular Locomotion Model was implemented in MATLAB Simulink consisting of three layers: The body-mechanical layer simulates the body parts, such as thigh, foot and a torso. These are connected with revolute joins. The second layer is the muscle actuation layer, which consists of seven hill-type muscles that produce their own force in the model. Finally, there is the neural control layer, that receives feedback from the first layer and uses this information to calculate the muscle stimulation for the second layer. 

The two main reasons why people fall are muscle deterioration and a slower transmission of neural signals in the body. The muscle deterioration was simulated by decreasing the maximal force that can be applied by each muscle. The neural delay was simulated by a time delay of the simulated neural signal from the neural control layer to the muscle actuation layer. This lead to gait instability.

Finally, a PD controller at the hip was implemented that simulates a hip exoskeleton. The controller uses the feedback from the joints and adds the additional torque that is needed to produce stable walking. 