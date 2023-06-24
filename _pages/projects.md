---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
redirect_from:
  - /resume
---
NIO-AD·Autonomous Driving Development
------
* **AutoLabeling**
Responsible for building an automated production pipeline for the data loop back, and opening up the entire link from mass production backflow data to dataset production. Design and integrate multiple algorithm modules 3D lidar odemetry & visual odemetry & nerf.

* **AutoTriage**
Responsible for the Autotriage project and design the architecture. Develop cloud offline perception system and locate the root cause of the DLB data. The project is used in AEB, ELK, NOP+ business, its automated processing rate reaches 70\%.

* **BEV perception**
  * Build the cloud-sensing BEV processing capability, complete the delivery of multiple 3D detection models. 
  * Design the GOD process pipeline based LiDAR points cloud.
  * Design LiDAR-CAM fusion big models to solve the missed detection of special-shaped vehicles and VRU issues. 
  * Propose TiG-BEV multiview learning scheme to improve the detection performance of the cam-based detector, which is submiteed to **ICCV 2023**.
  * Design Self-supervised depth estimation model using the Lidar Points as the depth label and optimize the reprojection error using the CAN signal.


Alibaba DAMO Academy-Autonomous Driving
------
* **Safety perception cerebellum**
Design and Lead full cycle of the Project. By checking the calculation unit & hardware & algorithm and the information of short-distance obstacles around the vehicle, implement transparent transmission or change operations on the commands issued by the control module. This project has been applied to the L4 product.

* **Lidar Perception**
Participate in the system construction of the autonomous driving perception module and responsible for the update and release of the software. Carry out the 3D point cloud detection work on business data, including model design & traing & deployment & optimization.

* **Neural Architecture Search**
Based on the FBNetV3, proposed a new nas pipeline for compressing the business model to adapt the certain compute hardware unit. Redundancy is carried out from the three dimensions of model depth, width and feature size, and the time-consuming of specific hardware is introduced as a constraint to search. The latency of the multi-task Perception model has been reduced from 40ms to 22ms on Xavier with less than 2% map decrease.

* **Pruning**
Develop and design lightweight tool auto-prune lib, which is currently used in various online model deployments and can achieve about 20% compression of parameters while ensuring accuracy.

* **Quantification**
Import the int8 quantization strategy on the lightweight compute hardware. This part of the work is based on the quantization capability of pytorch to achieve one-step compression of the model.

* **Knowledge Distillation**
In order to further improve the performance of the optimized model, the KD method has been applied the model development. On the visual business model, the mAP and mIOU can be improved by roughly 2%. While conducting the  business, a method for knowledge distillation that explores the inter-channel correlation to mimic the feature diversity of the teacher network has been proposed, which was accepted by **ICCV 2021**.

* **Model Automation Generation & Deployment & Evaluation**
Conduct the train-aware quantification and model deployment. Design model automation iterative pipeline based on DAG flow and link many business production modules such as data production, model training, and model online evaluation based on MotionNet to speed up the development of the model.
