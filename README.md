# VGG-16 Leaf Disease Classification

## Overview

This project implements **leaf disease classification using the VGG-16 deep learning architecture** with TensorFlow and Keras. A pretrained VGG-16 model with ImageNet weights is used as the feature extractor, with a custom classification head for classifying leaf images into 6 disease classes.

## Technologies Used

* Python
* TensorFlow
* Keras
* VGG-16
* NumPy
* Matplotlib
* OpenCV
* Google Colab

## Model Architecture

* Pretrained **VGG-16 with ImageNet weights**
* Convolutional base layers frozen during training
* Flatten layer
* Dense layer with 512 neurons and ReLU activation
* Dropout layer with 0.5 dropout rate
* Softmax output layer for 6-class classification

## Dataset

* Training images: **1,109**
* Validation images: **236**
* Test images: **150**
* Number of classes: **6**
* Input image size: **224 × 224**

## Data Preprocessing

The training pipeline uses image rescaling and augmentation techniques including:

* Rotation
* Zoom
* Horizontal flipping
* Vertical flipping
* Shearing

Validation and test images are rescaled before evaluation.

## Training

The model was trained for **20 epochs** using the Adam optimizer with a learning rate of `1e-4` and categorical cross-entropy loss.

## Results

| Metric                   |   Accuracy |
| ------------------------ | ---------: |
| Training Accuracy        | **87.96%** |
| Best Validation Accuracy | **82.59%** |
| Test Accuracy            | **80.47%** |

The model achieved its highest validation accuracy of **82.59% during Epoch 17**.

## Visualization

The notebook includes training and validation accuracy visualization to analyze model performance across epochs.

## Environment

The project was developed and executed using **Google Colab**.

## Files

* `VGG_16_MODEL.ipynb` — Complete VGG-16 leaf disease classification implementation

## Author

**Pujitha Berugu**
NIT Warangal — Metallurgical & Materials Engineering
