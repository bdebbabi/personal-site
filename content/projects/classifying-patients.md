---
title: "Classifying patients"
date: 2020-06-10
menu:
  sidebar:
    name: Classifying patients 
    identifier: classifying-patients
    weight: 5
---
The task consists in classifying patients as belonging to one out of three disease categories: Normal, Disk Hernia or Spondylolisthesis. Each patient is represented in the data set by six biomechanical attributes derived from the shape and orientation of the pelvis and lumbar spine. The complete code is available in this [notebook](https://www.kaggle.com/bilel09/classifying-patients-with-biomechanical-features). Different models were tested. The best one was a logistic regression which had an accuracy of 84%. 

The following figure shows the classification results displayed with a PCA _(Principal Component Analysis)_

{{<img src="https://user-images.githubusercontent.com/47567574/119036103-a9dabf00-b9b0-11eb-879d-e7d9630c64f8.png" align="center" caption="Patients classification results">}}
