# Comparative Analysis of Pretrained Models for Alzheimer's Disease Classification

## Overview
This project focuses on the classification of Alzheimer's Disease (AD) using MRI images. The goal is to develop and compare pre-trained deep learning models to classify MRI images into different stages of Alzheimer's Disease accurately.

## Datasets
Two distinct datasets from Kaggle were used in this study, providing a diverse set of brain MRI images for analysis.

### 1. Augmented Alzheimer MRI Dataset
- **Total Images**: 33,984
- **Classes**:
  - Non-Demented
  - Mildly Demented
  - Very Mildly Demented
  - Moderate Demented

This dataset was primarily used for training and validation. The image augmentation helped ensure the model generalizes well across various Alzheimer's cases.

### 2. Alzheimer's Dataset: 4 Classes of Images
- **Total Images**: 6,400 (1,279 in the test set)
- **Classes**:
  - Non-Demented
  - Mildly Demented
  - Very Mildly Demented
  - Moderate Demented

This dataset was crucial for testing and evaluating the model's classification performance across the different stages of Alzheimer's Disease.

## Model Architectures
Two pre-trained models were used in this project:

### 1. DenseNet169
- **Description**: DenseNet169 is a convolutional neural network that employs dense connections between layers, allowing for better feature propagation and reducing the risk of vanishing gradients.
- **Performance**: While the model showed good performance, it was outperformed by the Inception V3 model.

### 2. Inception V3
- **Description**: Inception V3 is a well-known deep learning model designed for efficient computation and high accuracy. Its factorized convolutions and regularization techniques help achieve superior performance.
- **Performance**: Inception V3 achieved the best results, with a testing accuracy of 93.59%.

## Results
The following table summarizes the performance of both models:

| Model         | Training Accuracy | Testing Accuracy | Correct Predictions (out of 1279) |
|---------------|-------------------|------------------|-----------------------------------|
| Inception V3  | 92.27%            | 93.59%           | 1190                              |
| DenseNet169   | 91.79%            | 77.24%           | 987                               |
