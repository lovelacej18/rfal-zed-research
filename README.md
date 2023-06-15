# rfal-zed-research
Current resources for using ZED2 in underwater stereo vision. 

#### In this Directory

###### README.md

[The file you are looking at now!] Documenting the compiled resources and how to navigate the directory.

###### Working with the ZED2.md

Documentation of using ZED2 camera with ROS integration, how to run the ZED node, settings that can be adjusted for imaging onboard the ZED, information about the open capture API (for raw data capture) and underwater calibration. 


###### Portofino (folder)

Dataset from Rizzini et al 2015. Underwater stereo images from Portofino, Italy from MARIS project. Goal of the project was for object detection underwater - code does not implement depth estimation. 

For more information on the MARIS project see the [RIMLab project page][https://rimlab.ce.unipr.it/Maris.php#MarisGarda] or the paper, Rizzini2015.pdf in this directory. 


###### Rizzini2015.pdf

Summary paper on MARIS project goals and software. Sections of most relevance are ***Image Pre-Processing Before Object Detection*** and ***Dataset Acquisition***. 

---

#### Underwater Stereo Imaging Projects

###### MARIS (Marine Autonomous Robotics for InterventionS) Project, RIMLab
[Project Homepage][https://rimlab.ce.unipr.it/Maris.php#MarisGarda]
Rizzini et al 2015. Investigation of Vision-based Underwater Object Detection with Multiple Datasets. 
Object detection as opposed to depth recovery - but initial processing might contain more what we're looking for.  
[project description pls write j]

*Software/Code*
Maris Vision - collection of ROS packages used for MARIS project. The stereo vision system is designed for detection, pose estimation, and grasp planning for object manipulation. 
[GitHub Repo][https://github.com/dlr1516/maris_vision]

*Datasets*
Portofino 2014 - a half an hour of image frame pairs. Provided "AS IS". Contains a README and 3 .tar.xz files. See Portofino folder in this repo.

Garda 2013 - raw dataset in rosbag format. 
[Source][https://www.ce.unipr.it/~rizzini/maris_acquisition_20130714/]

---

#### Calibration

##### Underwater Camera Calibration (CamOdoCal+PinAx)
Docker container with the CamOdoCal camera calibration software and PinAx model for underwater cameras. Automatically performs camera intrinsic and extrinsic calibration from images collected in-air, and provides underwater rectification maps.  

Requirements: Docker >= 1.12, nvidia-docker2
[GitHub Repo][https://github.com/jacobs-robotics/uw-calibration-pinax]

#### CADDY Software Tools
Underwater Camera Calibration - Docker container including CamOdoCal camera calibration package for in-air cameras, and the PinAx underwater camera model to rectify the images for underwater applications. 
[Home Page][http://www.caddian.eu//CADDY-Software-Tools.html], [GitHub Source][https://github.com/jacobs-robotics/uw-calibration-pinax]

---
