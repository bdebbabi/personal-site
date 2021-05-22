---
title: "Comments classification"
date: 2021-01-15
menu:
  sidebar:
    name:  Comments classification 
    identifier: comments-classification
    weight: 3
---
My school website has a section where students can rate the courses and add a comment. I had to classify the comments into positive and negative. As a ground truth, I used the rating. If it's above a certain value the comment is positive. This method can be biased since students can post a negative comment with a good rating. But it's the only available way.

I used the [Camembert](https://camembert-model.fr/) model, the french version of [BERT](https://huggingface.co/transformers/model_doc/bert.html). I fine-tuned it on a part of my dataset. In the end I obtained an AUC of around 0.80.

As we can see in the confusion matrix, the model performs better when predicting negative comments..  

{{<img src="https://user-images.githubusercontent.com/47567574/119195857-93eafe00-ba85-11eb-8069-d454b57dbbfa.png"  caption="Confusion matrix" align="center">}}
