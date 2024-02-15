# Ensembles

This project is designed to explore various machine learning techniques and ensemble methods using the MNIST dataset, a collection of 70,000 images of handwritten digits. There are multiple classifiers that are tested for training, including a Random Forest Classifier, a Neural Network, and an SVM Classifier.The goal is to compare the performance of individual classifiers and to combine them into a voting ensemble that aims to outperform each classifier on its own. Additionally, this notebook explores the concept of stacking ensembles by training a "blender" classifier that uses the predictions of the initial classifiers to make a final prediction.


## Dataset
The MNIST dataset, available in SciKit Learn, is split into three parts for this assignment: 50,000 instances for training, 10,000 for validation, and 10,000 for testing. This division helps in training the models, tuning their hyperparameters to avoid overfitting, and finally evaluating their performance.

## Training Classifiers

Used SciKit Learn to train various classifiers separately on the training set and evaluate their performance on the validation set. This process helps identify the most effective models and adjust their parameters to enhance performance.

## Voting Ensemble

Combined the trained classifiers into a voting ensemble, experimenting with both soft and hard voting, to achieve better performance on the training set. Evaluated this ensemble on the test set using a consistent metric.

## Stacking Ensemble

Ran the individual classifiers to make predictions on the validation set, then created a new training set from these predictions for training a "blender" classifier. This approach forms a stacking ensemble, which is then evaluated on the test set.

## Comparison and Analysis

Compared the performance of the voting ensemble with the stacking ensemble, including an analysis of the SciKit Learn StackingClassifier.
