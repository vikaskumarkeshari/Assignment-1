#CIFAR-10 Image Classification Using Convolutional Neural Networks (CNN)
Overview

This project implements an image classification system using a Convolutional Neural Network (CNN) on the CIFAR-10 dataset.
The task was completed as part of Assignment-1, where any dataset from Google Dataset Search could be used with a machine-learning algorithm covered in class.

The trained CNN model achieves:

Training Accuracy: 95%

Testing Accuracy: 96%

Dataset

Source: CIFAR-10 (via Google Dataset Search / Keras Datasets)

Summary:

60,000 color images (32×32 pixels)

10 object categories

50,000 training images + 10,000 test images

Classes:
Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck

Important Note:
✔ No normalization to 0–1 was applied
✔ No data augmentation was used
✔ Model was trained directly on raw pixel values (0–255 range)

Abstract

The CIFAR-10 dataset is widely used for evaluating deep learning classification models.
In this project, a CNN model is implemented using Python, without applying common preprocessing steps like pixel normalization or augmentation.
Despite this, the model is able to learn robust features and achieves 95% training accuracy and 96% testing accuracy, demonstrating strong feature extraction and generalization.

Methodology
Preprocessing

Used raw pixel values in the 0–255 intensity range

No normalization

No augmentation

Converted labels to one-hot encoded format

CNN Model Architecture

The model includes:

Multiple Conv2D + ReLU layers

MaxPooling2D for downsampling

Flatten + Dense layers for classification

Softmax activation in the output layer

Training Setup

Optimizer: Adam

Loss: Categorical Cross-Entropy

Batch Size: 32

Epochs: 20 (or as configured)

Metrics: Accuracy

Results Snapshot
Model	Training Accuracy	Testing Accuracy	Notes
CNN (This Project)	95%	96%	No normalization, no augmentation

The model generalizes very well despite minimal preprocessing.
