---
title: "Geometric deep learning"
date: 2020-06-05
menu:
  sidebar:
    name: Geometric deep learning 
    identifier: geometric-deep-learning
    weight: 6
---
## 1. Introduction
{{<img src="https://user-images.githubusercontent.com/47567574/118884993-7720c000-b8f7-11eb-960d-fe864b3dac94.png" alt="Prediction example" float="right" caption="Prediction example">}}
Traditional facial rehabilitation for facial palsy patients uses commonly visual feedback and subjective palpation techniques to evaluate the patient's progress. A computer vision system with real time feedback could be an innovative solution. The goal is to accomplish a segmentation on the different parts of the face (eyes, nose and mouth). The dataset contains face point clouds extracted using a kinect.

## 2. Data pre-processing
We decided to use the [PointNet++](https://github.com/Pangoraw/pointnet2) model. The dataset is composed of 333 samples with an average of around 145 200 points per file. The model uses samples with 2 048 points each. Because the initial number of points is too large for efficient learning and the number is not constant, we performed a random downsampling. 

## 3. Results
The model was trained using an Nvidia Tesla K80 on GCP. After a hyperparameters optimization obtained we obtained an accuracy of 99% and an IOU of 89%. 



{{<img src="https://user-images.githubusercontent.com/47567574/118883606-b64e1180-b8f5-11eb-8de6-ae514c6728ca.png"  alt="Confusion matrix " caption="Confusion matrix"  align="center">}}
