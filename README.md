# Automatic Facial Expression Recognition Using Features Extraction On Spatial Data Using CNN-RNN

This repository contains code for Automatic Facial Expression Recognition using feature extraction on spatial data with Convolutional Neural Networks (CNN) and Recurrent Neural Networks (RNN). The project uses OpenCV for image processing and various publicly available datasets from the internet for training and testing the models. The code is written in Python 3.8.

## Introduction

Facial expression recognition is a key component in human-computer interaction, enabling systems to interpret and respond to human emotions. This project focuses on extracting spatial features from facial images and utilizing CNNs and RNNs to classify different facial expressions.

## Features

- **Feature Extraction**: Uses OpenCV to preprocess and extract features from images.
- **Modeling**: Combines the power of CNNs for spatial feature extraction and RNNs for temporal dynamics.
- **Datasets**: Utilizes various publicly available datasets for comprehensive training and evaluation.
- **Python 3.8**: The code is compatible with Python 3.8.

## Installation

1. Clone the repository

2. Create and activate a virtual environment:
   ```bash
   python3.8 -m venv venv
   source venv/bin/activate
   ```

3. Install the required packages

## Usage

1. **Data Preparation**: Download the datasets (see the Datasets section) and place them in the `data/` directory.

2. **Preprocessing**: Run the preprocessing script to prepare the data:
   ```bash
   python preprocess.py
   ```

3. **Training**: Train the model using the training script:
   ```bash
   python train.py
   ```

4. **Evaluation**: Evaluate the model on the test set:
   ```bash
   python evaluate.py
   ```

## Datasets

The project uses several publicly available datasets, including:

- [FER-2013](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data)
- [CK+](https://www.jeffcohn.net/resources)
- [JAFFE](https://zenodo.org/record/3451524)

Download the datasets and place them in the `data/` directory. Update the paths in the configuration file if necessary.

## Model Architecture

The model architecture consists of:

1. **Convolutional Neural Network (CNN)**: For extracting spatial features from the images.
2. **Recurrent Neural Network (RNN)**: For capturing temporal dynamics and dependencies in the features.
