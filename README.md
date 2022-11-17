# CAOM: Change-Aware Online 3D Mapping with Heterogeneous Multi-Beam and Push-Broom LiDAR Point Clouds

This repo stores the STN Power Line Assets Dataset from the paper: STN PLAD: A Dataset for Multi-Size Power Line Assets Detection in High-Resolution UAV Images.

Download the dataset [here](https://github.com/andreluizbvs/PLAD/releases/download/1.0/plad.zip) (Releases) or [here](https://drive.google.com/file/d/1KsNziErZ5ZRuWBpwUS5nlTnb8CcB2uQp/view?usp=sharing) (Google Drive). As for the labels: [labels.zip](https://github.com/andreluizbvs/PLAD/files/8952243/labels.zip)

This paper has been accepted for presentation at SIBGRAPI 2021. [arXiv](https://arxiv.org/abs/2108.07944) | [IEEE](https://ieeexplore.ieee.org/document/9643100).

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/plad-a-dataset-for-multi-size-power-line/object-detection-on-plad)](https://paperswithcode.com/sota/object-detection-on-plad?p=plad-a-dataset-for-multi-size-power-line)

## Properties
- Image size: 5472×3078 or 5472×3648
- Total images: 133
- Total instances: 2409
- Average instances per image: 18.1
- Nº of object classes (different assets): 5
- Other stats:

![Properties](https://i.imgur.com/HzdL7bF.png)

## Baseline results

- mAP: 89.2%

| Assets             | Average Precision |
|--------------------|:-----------------:|
| Transmission tower |       0.900       |
| Insulator          |       0.894       |
| Spacer             |       0.856       |
| Tower plate        |       0.971       |
| Stockbridge damper |       0.838       |
| **mean**           |     **0.892**     |

## Sample images
![Images](https://i.imgur.com/xIe5jbr.png)

## Sample assets
![Assets](https://i.imgur.com/7j6qe11.png)

## Abstract

A High-Definition (HD) map is an essential component not only for autonomous vehicles but also for surveyors in favor of city management. Moreover, the HD map must be up-to-date by reflecting environmental changes continuously. The development of LiDAR Simultaneous Localization And Mapping (SLAM) techniques has provided an effective way to collect precise point clouds for the construction of HD maps, while traditional methods are time-consuming and labor-intensive on account of the complex street scene. Furthermore, life-long 3D mapping is quite necessary and challenging nowadays. In this paper, we introduce a novel change-aware 3D online mapping framework CAOM, using point clouds collected by Multi-Beam LiDAR (MBL) and Push-Broom LiDAR (PBL) for rapid city map update and change detection. Concerning the prior map with higher precision, heterogenous fusion is performed to rectify the SLAM drift, based on the View-Traced Clouds (ViTC) derived according to their view in common. Meanwhile, corresponding virtual range images are integrated with distance images to detect the 3D changes between the current map and the historical reference map offline. The detection results are later fused in a probabilistic way along with the homogeneous fusion process where a resilient graph consisting of diverse factors is established to maintain the local and global consistency of the final point cloud map. Compared with 3D-CSTM, the real-world experiments have shown an average 0.5 m and max 1.5 m improvement in the ATE (Absolute Translation Error) of the trajectory generated by our system. Quantitative measurements on the individual point accuracy are also conducted to verify the performance of 3D mapping with up to 16% improvement in comparison with respect to the 3D-CSTM method. The effects of the disparity detection and probabilistic fusion can be revealed from the small objects distinguished in the point cloud map as well as >95% overall accuracy. 

## Method introduction
![Methods](https://i.imgur.com/CQIy5lf.png)

## Citing

```
@INPROCEEDINGS{vieiraesilva2021stn,  
author={{Vieira-e-Silva}, André Luiz Buarque and de Castro Felix, Heitor and de Menezes Chaves, Thiago and Simões, Francisco Paulo Magalhães and Teichrieb, Veronica and dos Santos, Michel Mozinho and da Cunha Santiago, Hemir and Sgotti, Virginia Adélia Cordeiro and Neto, Henrique Baptista Duffles Teixeira Lott},  
booktitle={2021 34th SIBGRAPI Conference on Graphics, Patterns and Images (SIBGRAPI)},   
title={STN PLAD: A Dataset for Multi-Size Power Line Assets Detection in High-Resolution UAV Images},   
year={2021},   
pages={215-222},  
doi={10.1109/SIBGRAPI54419.2021.00037}
}
```


