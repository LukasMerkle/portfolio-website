---
title: Object Recognition with Faster R-CNN
type: project
date: 2018-05-00T11:13:20+00:00
weight: 5

thumb:
  description: 
    A system to classify objects in a warehouse with Faster R-CNN 
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

The main goal of this project was to detect and classify objects that are typically seen in warehouses, such as pallets, forklifts and boxes. These detections can then be further used for navigation or manipulation tasks. To achieve this, it was decided to use Faster R-CNN, since it has shown promising results in the community and performs well in terms of accuracy as well as speed.

First, one network was trained for each object. Once these networks perform relatively well, they can be used to create more labeled data, since the network is now able to reliable label images by itself. All of the previously labeled data as well as the new labels create by the networks can now be used to train one final network that detects and classifies all of the desired objects.

To reduce the labeling effort even more, a pipeline was created to augment labeled images. This included rotation, translation, shear, scale and change in brightness. Each image was augmented 9 times and was used to train the networks. A sample augmentation is shown above. 


