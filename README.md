# Tweet Sentiment Extraction

## Table of Content  
  * [Overview](#overview)
  * [Motivation](#motivation)
  * [Dataset](#dataset)
  * [Technical](#technical)
  



## Overview
This project aims to identifiy the words in a sentence which contribute to it's sentiment classification as Positive,Negative or Neutral.


## Motivation
Explainable AI [XAI]  is an emerging research topic.XAI refers to tools and technologies that help in interpreting the model.If an image is classified as a cat, we need to know
why it is detected as a cat.
In this project the sentiments of the tweets Positive,Negative and Neutral are already given and the part of the tweet which contributes to the classification is also given
We aim to build a machine learning model which learns which part of the tweet has influenced the classification of it.


## Dataset
Dataset from Tweet Sentiment Extraction Kaggle competition is used.


## Technical 
Problem statement is formulated as a Question Answering problem
Input text : Tweet
Question : Sentiment
Answer : part of the Tweet.

Tensorflow deep learning frame work is used.

Model trained on Kaggle GPU

BERT Base pretrained model and Roberta base pretrained model from Hugging face is explored.
A simple 2 Soft max layer head is used on top of the pretrained model from Hugging face.

Stratified K fold sampling technique used.

ByteLevelBPE Tokenizer is used.

Cyclic Learning rate and Learning rate decay experimented as learning rate schedulers.

Pre-Processing of the dataset is based on Abhishek Thakur's tutorials.

Adam optimizer is used









