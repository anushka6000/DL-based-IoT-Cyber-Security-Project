# DL-based-IoT-Cyber-Security-Project
The repository contains google colab notebook of the cyber security project.

# Motivation 
As the Internet of Things is becoming a part of our lives by connecting a large number of devices we use daily, it is also essential to develop systems that prevent data breach by detecting suspicious activities and alerting users. There have been many attempts at developing Intrusion Detection Systems to solve the above purpose but none achieve 100% accuracy. Motivated by this, we try to improve intrusion detection systems by trying various machine learning and deep learning methods. Here I have performed an attack vs non-attack classification on the BoT-IoT dataset. I have achieved an overall best accuracy score of 1 for attack vs non-attack classification with the help of a Semi-Supervised Learning model.

# Dataset Used
I have used the BoT-IoT dataset to perform the task. Link to the dataset:
https://drive.google.com/file/d/13kZD73VEOQwlGCIarPxtr-oFkrsN-aUV/view?usp=sharing 

# Model Used 
Disagreement based semi-supervised learning 
Semi-supervised learning is concerned with strategies for automatically utilising unlabeled data in addition to labelled data in order to increase learning performance without requiring human interaction. The goal of disagreement-based semi-supervised learning is to create several learners, allow them to collaborate to exploit unlabeled data, and keep the basic learners in disagreement. The model used here is a disagreement based semi-supervised learning with single view multiple-classifier. Three classifiers are used here namely: Decision Tree, BP network and Gaussian Naive Bayes classifier.

## Decision Tree
For classification, Decision Trees (DTs) are a non-parametric supervised learning approach. The objective is to learn basic decision rules from data attributes to develop a model that predicts the value of a target variable. A tree is an approximation to a piecewise constant. It is a flowchart like tree structure, where each internal node denotes a test on an attribute, each branch represents an outcome of the test, and each leaf node (terminal node) holds a class label.

## BP Network
One of the most extensively used neural network algorithms is the back propagation (BP) neural network method, which is a multi-layer feedforward network trained using the error back propagation technique. The BP network can learn and store a large number of input-output model mapping relations. Its learning rule is to employ the steepest descent approach, in which back propagation is used to control the network's weight and threshold values in order to attain the lowest error sum of squares.

## Gaussian Naive Bayes
Naive Bayes classifiers are a collection of classification algorithms based on Bayes’ Theorem.  It is a group of algorithms that share a similar premise, namely that each pair of characteristics being categorized is independent of the others. It predicts membership probabilities for each class such as the probability that a given record or data point belongs to a particular class.  The class with the highest probability is considered as the most likely class. When attribute values are continuous, an assumption is made that the values associated with each class are distributed according to Gaussian i.e., Normal Distribution. In such cases the Gaussian Naive Bayes classifier is used. 20\% of the data is considered as labelled data and is trained on the model with 20 data splits on the entire dataset. The error, accuracy, precision are found as an average of the 20 results obtained from each split. 

