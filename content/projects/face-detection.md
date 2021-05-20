---
title: "Face detection"
date: 2020-06-04
menu:
  sidebar:
    name: Face detection 
    identifier: face-detection
    weight: 7
---

The goal of this project is to perform a face detection on images, using classical algorithms. The complete code is available [here](https://gitlab.utc.fr/bdebbabi/face-detection/-/tree/master).

## Training
{{<img src="https://gitlab.utc.fr/bdebbabi/face-detection/-/raw/master/images/test_example.png" align="center" caption="Face detection example" float="right">}}
A sliding window algorithm is applied, combined with a SVC (_Support Vector Classifier_) and HOG (_Histogram of Oriented Gradients_) features.
The best hyper-parameters, classification algorithm and feature descriptors were obtained using a cross-validation.

## Testing

The following results were obtained on the test images:

- Precision:  99.07 %
- Recall   :  94.02 %
- F1-score :  96.48 %
- AUC      :  93.46 %
  
{{<img src="https://user-images.githubusercontent.com/47567574/119037173-ed81f880-b9b1-11eb-804c-e65929b7c20d.gif" width="50%" align="center"  caption="Sliding window">}}

