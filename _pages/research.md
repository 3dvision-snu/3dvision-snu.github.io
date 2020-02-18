---
title: "3D Vision Lab - Research"
layout: textlay
excerpt: "3D Vision Lab -- Research"
sitemap: false
permalink: /research/
---

# Research

We strive to the emerging field of 3D vision where we understand the 3D world around us. We not only sense, acquire and perceive the 3D models, but also visualize and extract semantic information to develop various applications, namely VR/AR, robotics, human augmentation, and ambient intelligence to name a few. The ultimate goal is the bridge between human and intelligent agent to benefit human.

### Research projects include: <br>
**1) 3D acquisition and modeling:**{: style="font-size: 110%" } With the help of various acquisition devices, we can capture and build a 3D model of objects, scenes, and human bodies. The research assist robots or human users to acquire the 3D models of interest. We also ease the everyday use of acquired models in everyday life by updating the 3D models with light-weight acquisition devices, or send the stream of 3D video over mobile network.

![]({{ site.url }}{{ site.baseurl }}/images/respic/image001.png){: style="width: 300px; border: 10px"}<br>
![]({{ site.url }}{{ site.baseurl }}/images/respic/image002.png){: style="width: 300px; border: 10px"}<br>

**Light-Weight Update of Large- Scale 3D Scenes**<br>
<U>Research objective</U>: Given off-line 3D scan and online 360 photo, quickly update the 3D model of the scene.<br>
<U>Approach</U>: Hybrid feature matching of different data modality for localization, the change detection of 360 images with respect to the large- scale 3D model.<br>

![]({{ site.url }}{{ site.baseurl }}/images/respic/image003.png){: style="width: 300px; border: 10px"}<br>

**Real-Time 3D Video Streaming System**<br>
<U>Research objective</U>: Streaming volumetric video at video frame rate via mobile devices<br>
<U>Research scope</U>: Efficient storing and processing with dynamic octree structure, adaptive rendering resolution and view-point prediction<br><br>

**2) Using 3D models for visualization:**{: style="font-size: 110%" } 3D models are crucial for seamless AR/VR applications and realistic rendering. The key technical components include localization, pose estimation, texture acquisition, and lighting estimation.<br>
![]({{ site.url }}{{ site.baseurl }}/images/respic/image004.jpg){: style="width: 300px; border: 10px"}<br>
![]({{ site.url }}{{ site.baseurl }}/images/respic/image005.png){: style="width: 300px; border: 10px"}<br>

**Novel View Synthesis**<br>
<U>Research objective</U>: Synthesize a target view from a given source view and its camera pose without a 3D model, Extend the latent space representation into multi-object 3D scenes<br>
<U>Approach</U>: Neural rending with end-to-end trainable framework<br><br>

**3) Using 3D data for perception:**{: style="font-size: 110%" } 3D information is widely used for perception, and recent trends on 3D perception utilize the state-of-the-art techniques from computer vision and machine learning. We utilize neural networks of generative models, metric learning, and/or reinforcement learning to boost the performance.<br>

![]({{ site.url }}{{ site.baseurl }}/images/respic/image006.jpg){: style="width: 300px; border: 10px"}<br>
![]({{ site.url }}{{ site.baseurl }}/images/respic/image007.png){: style="width: 300px; border: 10px"}<br>

**Shape Completion Preserving Details**<br>
<U>Motivation</U>: Existing 3D data suffer from occlusion and noise of sensors. Current shape completion pipeline acts as object recognition<br>
<U>Approach</U>: Train GAN in local and global shape and use graph-based convolutional network to preserve details<br>

![]({{ site.url }}{{ site.baseurl }}/images/respic/image008.png){: style="width: 300px; border: 10px"}<br>

**Point Cloud Instance Segmentation**<br>
<U>Research objective</U>: Direct segmentation of individual objects on the raw 3D measurements<br>
<U>Approach</U>: Deep metric learning on point cloud feature extracted via sparse convolutional neural network<br><br>

**4) Using 3D information for interaction**:  The real-world 3D models are utilized for manipulation, navigation, or other robotic applications. Our focus is to build algorithms to control robot in un-constrained set-up and robust to small changes.

![]({{ site.url }}{{ site.baseurl }}/images/respic/image009.png){: style="width: 300px; border: 10px"}<br>

**Visuomotor Policy via Scene Understanding**<br>
<U>Research objective</U>: Given complex visual scene, make robot disentangle raw observation into latent full state, and learn generalized policy.<br>
<U>Research scope</U>: Robot manipulation in non-stationary environment based on 2D/3D raw observation<br>

![]({{ site.url }}{{ site.baseurl }}/images/respic/image010.png){: style="width: 300px; border: 10px"}<br>

**Occlusion-Aware Navigation**<br>
<U>Research objective</U>: Given an approximate map of changing environment, infer the navigation path allowing online modification<br>
<U>Research scope</U>: Scene understanding from partial observation, joint inference of human-object interaction and scene reconstruction<br><br>