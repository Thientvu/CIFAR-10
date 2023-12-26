# CIFAR Classification Project README

## Project Overview

This project explores the CIFAR-10 dataset using four different classifiers: kNN, Logistic Classifier, Neural Network, and Convolutional Neural Network (CNN). The goal is to compare their performances and provide insights into model selection and hyperparameter tuning.

### Team Members
- Gregory Saldanha, Ying-Che Shih, and Thien Vu 

## Data Description

The CIFAR-10 dataset comprises 60,000 color images (32x32) distributed across 10 classes. The data was flattened into a numpy array with 3072 features, representing red, green, and blue channel values.

## Experimental Setup

- Dataset splits: 40k training, 10k validation, 10k testing samples.
- Pixel values normalized to [0, 1].

## Evaluation and Model Selection

### 1. kNN Classifier
- Selected k = 5 for better generalization.

### 2. Logistic Classifier
- Optimal model (Model E): Learning rate = 0.01, Batch size = 128.

### 3. Neural Network
- Model B selected as the best performer (50.3% accuracy on validation data).

### 4. Convolutional Neural Network
- Tuned Model C with regularization and batch size.
- Achieved 73.6% accuracy on the test data.

## Insights

- Surprising kNN performance with over 30% accuracy despite high dimensionality.
- Logistic classifier underperformed expectations, potential overfitting.
- Successful hyperparameter tuning, especially for CNN.
- Importance of visualizing models and systematic experiment documentation.

## Error Analysis

- CNN confusion matrix revealed frequent misclassification between classes 5 (dog) and 3 (cat).