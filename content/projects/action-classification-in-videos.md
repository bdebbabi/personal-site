---
title: "Action classification in videos"
date: 2021-01-10
menu:
  sidebar:
    name: Action classification in videos
    identifier: action-classification
    weight: 2
---
The goal of this project is to classify human actions in videos. The [Slowfast](https://github.com/bdebbabi/SlowFast) model, developed by the Facebook AI Research team is used. I improved it by adding a person tracking algorithm using the [deepsort](https://github.com/nwojke/deep_sort) algorithm. It was then possible to have a summary of all the actions performed by a specific person in a video. The idea is to use this model to improve remote meetings and brainstorming sessions. 

{{<img src="https://user-images.githubusercontent.com/47567574/118726618-dddba600-b831-11eb-9d61-bf1afc933aa7.gif" align="center" caption="An example of tracking the activities of subjects">}}
