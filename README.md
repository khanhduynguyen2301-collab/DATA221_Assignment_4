# DATA 221 Assignment 4

**Course:** Introduction to Data Science  
**Assignment:** Assignment 4  
**Student:** Duy Khanh Nguyen

## Overview

This repository contains my solutions for **DATA 221 Assignment 4**.  
The assignment explores two major supervised learning approaches:

- **Decision Trees**
- **Neural Networks / Convolutional Neural Networks (CNNs)**

The work is divided into two main parts:

- **Questions 1–5:** Breast Cancer Wisconsin (Diagnostic) dataset
- **Questions 6–7:** Fashion MNIST dataset

## Datasets Used

### 1. Breast Cancer Wisconsin (Diagnostic)
Used for **Questions 1–5**.

This dataset is loaded from `scikit-learn` and contains:

- 569 samples
- 30 numeric features
- Binary target variable:
  - malignant
  - benign

### 2. Fashion MNIST
Used for **Questions 6–7**.

This dataset is loaded from `TensorFlow / Keras` and contains:

- 60,000 training images
- 10,000 test images
- 28 × 28 grayscale images
- 10 clothing categories

## Questions Covered

### Q1 — Dataset Exploration and Understanding
- Constructed the feature matrix `X` and target vector `y`
- Reported the shape of the dataset
- Reported the class distribution
- Discussed whether the dataset is balanced or imbalanced
- Explained why class balance matters in classification

### Q2 — Decision Tree Model Using Entropy
- Split the data using an 80/20 train-test split with stratification
- Trained a Decision Tree classifier using `entropy`
- Reported training accuracy and test accuracy
- Explained entropy in the context of decision trees
- Discussed overfitting vs generalization

### Q3 — Controlling Tree Complexity and Interpretability
- Trained a constrained Decision Tree model
- Reported training accuracy and test accuracy
- Displayed the top 5 most important features
- Discussed the effect of model complexity on overfitting
- Explained how feature importance improves interpretability

### Q4 — Neural Network for Binary Classification
- Standardized the input features
- Built and trained a neural network with at least one hidden layer
- Used a sigmoid output layer for binary classification
- Reported training accuracy and test accuracy
- Explained why feature scaling is important
- Explained what an epoch means during training

### Q5 — Model Evaluation and Comparison
- Computed confusion matrices for:
  - constrained Decision Tree
  - Neural Network
- Compared both models
- Discussed one advantage and one limitation of each

### Q6 — Convolutional Neural Network with Built-in Dataset
- Loaded the Fashion MNIST dataset
- Normalized pixel values to the range `[0, 1]`
- Reshaped images to include a channel dimension
- Built a CNN with:
  - Conv2D layer
  - MaxPooling2D layer
  - Dense output layer
- Trained the model for at least 15 epochs
- Reported test accuracy
- Explained why CNNs are preferred for image data
- Explained what the convolution layer learns

### Q7 — CNN Error Analysis and Misclassification Study
- Generated predictions on the test set
- Computed and displayed the confusion matrix
- Identified at least 3 misclassified images
- Displayed:
  - true label
  - predicted label
- Discussed one misclassification pattern
- Suggested one realistic improvement to CNN performance

