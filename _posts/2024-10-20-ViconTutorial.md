---
layout: post
title: Tutorial for Vicon System Setup and Usage
date: 2024-12-21 16:00:00-0400
description: This would be like an instruction to help the newer to learn how to setup and use Vicon in just one day.
tags: Vicon System
categories: sample-posts
related_posts: false
giscus_comments: true
---

# **How to set up and use Vicon System within just one day?**

 <img src="https://github.com/JackTony123/picx-images-hosting/raw/master/vicon.70aeh6yr4g.webp" style="zoom: 25%;" /><img src="https://github.com/JackTony123/picx-images-hosting/raw/master/vicon_real.4g4k4k0l0h.webp" style="zoom: 14%;" />

This tutorial is based on the [Vicon System](https://www.vicon.com/), which is a state-of-the-art tool widely used in robotics research for precise motion tracking and analysis. With its high-speed cameras and advanced algorithms, Vicon provides accurate 3D position and orientation data of objects and markers in real time. This turtorial is based on our Lab's environment, software and hardware to give a detailed instruction to help the beginner to learn how to set up all preparation work and use Vicon for your research in quick.

**Preparation work:** You should have installed the [Vicon Tracker](https://www.vicon.com/software/tracker/) software with an active license. (We use the Version 3.8 as example based on our lab's version). Also, make sure all the cables connect with your Vicon camera correctly to make sure all Vicon cameras can build up connection through ethernet to your client PC.

First, when you first time to use Vicon, open the Vicon Tracker app, and then you will see this screen:

![](https://github.com/JackTony123/picx-images-hosting/raw/master/1.26ljljru7r.webp)

The `Vicon Camera` tabular list all camera connected to your PC actively as shown below:

![](https://github.com/JackTony123/picx-images-hosting/raw/master/image.1028cy4mm6.webp)

Note that if you have redundant cameras which may not need to use or if you have more than two aeras for different research testbed, you can click one camera and then unchoose the `Enabled` as shown below:

![](https://github.com/JackTony123/picx-images-hosting/raw/master/image.ic6od95pg.webp)

Then you will see these is a pause icon before the camera as shown below:

![](https://github.com/JackTony123/picx-images-hosting/raw/master/image.86tpqab5bt.webp)

Also, you will also see the pause icon appear on the screen of the specific camera:

![](https://github.com/JackTony123/picx-images-hosting/raw/master/image.9rjgprap3j.webp)

Next, before configurate the setup of your software, you need to use a laster pointer to make sure each camera's lens project to the same point in your experiment area (strongly suggest that set up the center point to be the center point of your experimental ground).

![](https://github.com/JackTony123/picx-images-hosting/raw/master/b851111ec9b9b2016c9b032100105af.7pcv83vca.webp)

The corrected adjusted position for each Vicon camera should be sure that the laser point out the same position as the example shown below:

![](https://github.com/JackTony123/picx-images-hosting/raw/master/image.3nronbgz0h.webp)

After that, once you set up all cameras' posture, then strongly suggest that there should be two people that one people check the app to choose the scenario to the  `CAMERA` 

![](https://github.com/JackTony123/picx-images-hosting/raw/master/image.6m3yqtv12y.webp)

Then, you will see the senero as shown below:

![](https://github.com/JackTony123/picx-images-hosting/raw/master/image.b8ysy80av.webp)

If the camera is ready to use as shown above, you will see so many green cross dots appear on the white rectangle aera, this means the focal distance of the camera is suitable to make sure the camera can see the scenario clearly. If the focal distance is not suitable, you will see that the triangle icon in the center of the icon for the specific camera in`Vicon Camera` tabular will be the dark green, not the light green as the camera 1, 2, 3, 4 shown above. In that case, you need to ajust the focal distance by using the two lens on the camera as shown below:

![](https://github.com/JackTony123/picx-images-hosting/raw/master/image.83a3slb11r.webp)

As the picture shown above, you can adjust the lens ① and ② to change the focal distance of the camera to make sure the the green cross dots can be appeared on the software to make sure the camera can see your experimental ground clearly.
