---
title: Hip Exosceleton
type: project
date: 2018-05-00T11:13:20+00:00

thumb:
  description: 
    Simulation of hip exosceleton for elderly to prevent falling 
  img: bio_thumb.png

highlights:
- Implemented a … model unsing MATLAB Simulink to simulate human walking
- Induced external disturbances to simulate falling in elderly
- Improved stabiliy by adding controllers at the hip to prevent falling

info:
  robot_type: Simulation
  application: 

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
  src: bio_dia.png
  caption: 
    Block diagram of the perception for the person follower.
    I implemented the Person Tracker section.

---

The purpose of this project was to investigate how a hip exosceleton can prevent falling in elderly. First, a ... model was implemented in MATLAB consisting of a neural layer, muscle layer and ... layer. This model is solely based on reflexes and simulates human walking. Next, the two main reasons why people fall are muscle deterioation and a slower transmission of neural signals in the body. The muscle deterioration was simulated by decreasing the maxmial force that can be applied by each muscle and the neural delay by a time delay of the simulated neural signal from the neural layer. This lead to gait instability  