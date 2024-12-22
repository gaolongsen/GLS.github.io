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





**3. Problem and correct related operations for Vicon system**

Sometimes when we decide to make the Initialization for the Vicon system and reset the cartesian coordinate system, we need to use *ViconTracker**(now the newest version is 3.10)* to make the configuration for the Vicon system. Firstly we should open the software, then find the page as below:

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeDlowi0pYJxp3W55C01wu6FcctFwY8Lh74e-zABzXzBLhwXV3ytedlhJTKgPbUrLHWDdD12dnNSITGNNjyDbj4l8vnh8l6UvH_numk4SzW1yS2smyzVgRVPbejFthXjzei7jfOoyia1pdfFO3X18s6a24?key=oIxLDQ1epLIj9gvRDHrQxA)

​	

1. Camera Selection
2. View Changer
3. Important tabs
4. Non-functional Camera symbol

When connecting the Vicon system, you must be sure that the cameras you are interested in working with are all pointing in the direction of the scene you are working in. If the cameras are pointing in the wrong direction, you will see a symbol like (4) in the image above, they might show up with nothing in the frame when looking at camera view similar to the image below.

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfuJC0yKvGKUjST2J1QKBj-EtMKwjSyGhq6D9Q-FqXaSjMjxEmJUs7EwrrnEt8WGKbid8qQlUrKJ5dfJ16jzgAljc-1wJLqkEZ5jp_z_a6DypJU3BfisjfLiuX0bGM6_ciAGOic1MYGPuUMfLyp2JpB-SD7?key=oIxLDQ1epLIj9gvRDHrQxA)

If you run into the scenario mentioned above, the first thing you should do would be to double check your camera positioning to make sure the camera is facing in the right direction and is even capturing the markers you’re interested in.

If you find that the camera is capturing the correct frame, then another option would be to lower the “Threshold” option under that camera's specific properties.

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcDkQE2QqAk5JbNKZ0llOyz0jPIa0yOUBeGBvS1JSRTcCCVqdfZkZpaCmQiWlBzPuA_fdYJ-KtKzyUQz8eerITnW7DFvm2z7-0eiok-6MV09jbce41a0WMUeLxpUTOS53MTOJwwLoNFwKN5Y1qmBw9p2Lm2?key=oIxLDQ1epLIj9gvRDHrQxA)

Once the threshold has been adjusted, your camera should begin showing marker positions, and then you’re ready for the next step.

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfEvQcLDxjMr5EHmyI4fyQ1iVWu6hJy-9ze7PJJxUJ4cwGeMI1rIabCxtsGhRmx2GeBvVfySFeuqO9f2MSNBDzD_725PJhbKuI6kdRibF5Z3PixHnDtXg663lj3UgdZBs6HLBqEBLWOhPa5awZNibozcg?key=oIxLDQ1epLIj9gvRDHrQxA)























①. Click the ‘ **Calibrate**’ button

②. Find the search column for ‘ **Camera Calibration Feedback,’** then choose the cameras which you need to initialize.

③. After finishing the choice, click the ‘ **Start** ’ button in the ‘Calibrate Cameras’ column.

/*********************************************************************************************

**Notice**: Here, we may meet the error after we click the ‘start ’ button as the situation happened below![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeAiqJXkZNrM0ir5T7KY7IeWFBAedr3MdUjCyPvoAevnNZzNxeUxErSJZE8Vxyy3Q32wtRnTlxSwm65EDgxcLy7_IIJvLlZae9dHbRydNtL_6rgCrYeYCsCEf9TquJqxSQP3QNGjJjSZwdQvcER7AehPA?key=oIxLDQ1epLIj9gvRDHrQxA)

As the terminal reported, the Tracker is unable to write to the calibration x2d file. For this error, we need to find the path of data storage for Tracker:

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXePx41PhRzHFpygrt2s2MZAM4Dmco-iOMf2FlTO1DfzNVrDyG-nMSznipgP0ZL9nrW_STSngNPnvtwtgqAnNKfj9Jy8XICLpVB3HdAkk7etAWzka7QPncjYO8ONOP4VWQWkBY3SAS9y2oR5Me3MsNl6O5M?key=oIxLDQ1epLIj9gvRDHrQxA)

Here we can find that there is a compressed file and other previous data files included .x2d file. 

Firstly, we need to move all files except the last one to the compressed file to save the previous data(if required). This operation makes sure that there are no .x2d files and .xcp files in this path to let the tracker write new .x2d and .xcp files here. 

Secondly, we back the tracker, do the same operation as we mentioned above from ①~③, 

Then we can initialize the vicon system successfully, as the shot screen below:

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfzqHyQWRzvx_vtRndsPCyLYaKUGiVfnrMybPAy22-jEcX_j94VkoQay1uzO7aWqDb8HgRyAEGPO043hyhom9gk_QxOOHdvuJL2OpXyS1pvPphDC28Sovo83xpx1AwYmR5E8bJOF_r26nsNJT1P1QO8UwY?key=oIxLDQ1epLIj9gvRDHrQxA)

************************************************************************************************/

④. After we initialize the cameras we selected successfully, we need to set the origin point for the 3-D workspace to build up a new Spatial Cartesian Coordinate System. Here we choose one position, which should be the center point of the workspace’s base on the ground.

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdCDYoFxsxzC9wjAmon2EMJn_W2PDUQCNGniwR2GDcLk6SSHj-34_duqES6KPN2g1r5rUvQSGiKodLP1pebbe9gmZpX8LV5mE-Fc9C31HSjNHwVJwKDs0J27Z5M-UQ6UuOQ_6u0uzA75JRdra-JzuJaAQ?key=oIxLDQ1epLIj9gvRDHrQxA)

Next, we find the ‘ **Set Volume Origin** ’ column on the left and click ‘ **Start**.’ Then we can see the originality part as below:

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfvzVVqQyb-U6Ij1joq0MwtfPf-M6qZ_hlua50pspUTFYes1fIFDIaV0na41JdrdTxgUw1cSRxasHTnL4Mw-IJYFg4loDzwy55cWQp_aSAVkxysvCFjBzdN7JefAAnHu_55emxdC9TO8RtvLAG37WqmlvY?key=oIxLDQ1epLIj9gvRDHrQxA)

⑤. After we click the ‘ **Set Origin** ’ button, all the positions for cameras will be reset, and the new spatial cartesian coordinate system has been built up. 

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcFa6VFink3YrZBA0jfZa-cbpd3aVCIS8AsigwILpJiZQhuSWpHvcIkqtHqrut7bSmzO7L-kyyDKYQ-cAoGBa_NNNGatOj25_wC5FDX_fEyKLopHpQOuMNCQmrSSIaCgHbAVbX7Bz1OD_8ICCOcz_UJPg?key=oIxLDQ1epLIj9gvRDHrQxA)

Once you’ve collected your data using the recording section, you can view the graphs associated with your trial by loading in a trial, 

**Note:** If you find you **cannot set up the origin frame**, please select camera view and then clear all mask for each camera

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXehbjJhRPZ_DBjvPNOWsvuvSDtd6t-ABfXUi83QSrdn4Sj_g9UP43IPc8mic7Yfd2XPPDg594LpyWoiS6u3WBMa8QHIgyPCnqD5QfVaMzU0ZLixRWuMhBzZ-LQfAmDcIy7nM6vq0w?key=oIxLDQ1epLIj9gvRDHrQxA)

 

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd1SXqTYF0_el6fxjZxJD_Ia0U0y2ij3GDg1I_KgYpzAn_Ge9yk5c7OnetwdOPM50LeFSfysIX3ekk7NbHSU_b8qlahgm3Gjbp5R4hVZoJpdvS-2rSjOsyPMVzq7ECFtLc5awvLhR-ymPNEBuzeUmZdeQWj?key=oIxLDQ1epLIj9gvRDHrQxA)

selecting the object in the tracked object in the 3D perspective view, and then switching to graph mode. Once done, you should select the appropriate graph using the drop-down menu, similar to the image below.

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe-ONHcjVMyn_0FJ_cedlyQczQKOF7Qq0Ui1BthcxiDUVAsHWK_JCA2jfjlAo0_QNCTHhL3DDeDX3Qd7c12aH2uEg0OrTbUgKfXj10Gi9C1JeawEH39U0E7sxZx3fo9-Z64tu3gFIBJT4MzWxSJF_TF39w?key=oIxLDQ1epLIj9gvRDHrQxA)

You can then view the position graphs, and from there you can select the velocity and acceleration graphs.

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd0Zw3K_nGsG1FF4c2mzCH5FofcqhGQN4EHAF7oYTbdSJnTbGFPoSzGL-6I_Wtlpc7DRni3FqRmh2GWT9JLssJ45DrvdNaoH1xtZeNDXcJa1Feyx-bm_ImbNinJ91kroraI0GRKnkUGikD6pttQJWxBkTcR?key=oIxLDQ1epLIj9gvRDHrQxA)

