---
title: "Anomaly detection in videos"
date: 2021-05-21
menu:
  sidebar:
    name:  Anomaly detection in videos 
    identifier: anomaly-detection-in-videos
    weight: 1
---
For my end of studies internship, I'm working on an anomaly detection model. The goal is to be able to detect unexpected human actions in videos. The model I developed is an autoencoder, that uses a pose estimation as input, and tries to reconstruct it as well as possible. The idea is to train it on normal human actions in order to be able to recognise them. In this case the reconstruction error is low. The model will then have a high reconstruction error for all the other actions it wasn't trained on.   

The model could be used on different usecases but I'm testing it on a pedestrian dataset. In this dataset the normal behaviour is someone walking in the street and the anomaly is for example someone running, riding a bike or jumipng.  