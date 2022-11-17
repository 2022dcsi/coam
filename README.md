# CAOM: Change-Aware Online 3D Mapping with Heterogeneous Multi-Beam and Push-Broom LiDAR Point Clouds

This repo stores the code of the paper CAOM: Change-Aware Online 3D Mapping with Heterogeneous Multi-Beam and Push-Broom LiDAR Point Clouds.

## Abstract

A High-Definition (HD) map is an essential component not only for autonomous vehicles but also for surveyors in favor of city management. Moreover, the HD map must be up-to-date by reflecting environmental changes continuously. The development of LiDAR Simultaneous Localization And Mapping (SLAM) techniques has provided an effective way to collect precise point clouds for the construction of HD maps, while traditional methods are time-consuming and labor-intensive on account of the complex street scene. Furthermore, life-long 3D mapping is quite necessary and challenging nowadays. In this paper, we introduce a novel change-aware 3D online mapping framework CAOM, using point clouds collected by Multi-Beam LiDAR (MBL) and Push-Broom LiDAR (PBL) for rapid city map update and change detection. Concerning the prior map with higher precision, heterogenous fusion is performed to rectify the SLAM drift, based on the View-Traced Clouds (ViTC) derived according to their view in common. Meanwhile, corresponding virtual range images are integrated with distance images to detect the 3D changes between the current map and the historical reference map offline. The detection results are later fused in a probabilistic way along with the homogeneous fusion process where a resilient graph consisting of diverse factors is established to maintain the local and global consistency of the final point cloud map. Compared with 3D-CSTM, the real-world experiments have shown an average 0.5 m and max 1.5 m improvement in the ATE (Absolute Translation Error) of the trajectory generated by our system. Quantitative measurements on the individual point accuracy are also conducted to verify the performance of 3D mapping with up to 16% improvement in comparison with respect to the 3D-CSTM method. The effects of the disparity detection and probabilistic fusion can be revealed from the small objects distinguished in the point cloud map as well as >95% overall accuracy. 

## Method
![Methods](https://i.imgur.com/CQIy5lf.png)

## Code
### The code will come soon…
