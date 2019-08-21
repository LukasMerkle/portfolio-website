---
title: Object Recognition with Faster R-CNN
type: project
date: 2018-05-00T11:13:20+00:00
weight: 5

thumb:
  description: 
    A system to classify objets in a warehouse with Faster R-CNN 
  img:  pallet_thumb.png

highlights:
- Modified Faster R-CNN and trained on collected data to classify pallets, forklifts and robots
- Implemented augmentation algorithm (rotation, scale, etc.) to speed up labeling process
- Developed pipeline to retrain on labels created by neural network (Semi-supervised learning)

info:
  robot_type: Object Detection Algorithm
  application: Warehouse Automation

org:
  name: Still GmbH
  link: https://www.still.de/en-DE.html

personal:
  role: Perception Intern
  timeframe: May 2019 – August 2019

media:
- type: image
  src: forklifts.png
  caption: 
      Detection and classification of forklifts in a warehouse
- type: image
  src: pallet.png
  caption: 
      Detection and classification of (solely) pallets in a warehouse
- type: image
  src: augment2.png
  caption:
      Augmentation sample for labeled image with a forklift
- type: image
  src: pipeline_rcnn.png
  caption:
      Proposed pipeline for manual semi-supervised learning


---


