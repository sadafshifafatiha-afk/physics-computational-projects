# CIFAR-10 Neural Network Image Classifier

**Field:** Machine Learning / Computer Vision  
**Tools:** Python, TensorFlow / Keras, NumPy, Matplotlib  

## Overview
This project implements a Convolutional Neural Network (CNN) to classify images from the CIFAR-10 dataset into 10 distinct categories (airplanes, automobiles, birds, cats, deer, dogs, frogs, horses, ships, and trucks).

## Objective
To build, train, and evaluate a deep learning model for multi-class image classification while analyzing performance metrics such as accuracy and loss to understand model performance.

## Methodology
* **Data Preprocessing:** Loaded the CIFAR-10 dataset and normalized pixel values from `[0, 255]` to `[0, 1]` for improved model convergence.
* **Model Architecture:** Constructed a Sequential CNN featuring:
  * 2D Convolutional layers (`Conv2D`) with ReLU activation to extract spatial features.
  * Max Pooling layers (`MaxPooling2D`) for spatial downsampling.
  * Flattening layer to convert 2D feature maps to 1D feature vectors.
  * Fully Connected (`Dense`) layers with a final Softmax activation for 10-class probability output.
* **Training & Optimization:** Compiled using the Adam optimizer and Sparse Categorical Cross-Entropy loss function, trained for 10 epochs with a validation split.

## Results & Performance
* **Test Accuracy:** ~70% *(insert your exact printed test accuracy here, e.g., 72.45%)*
* **Metrics:** Evaluated model performance across training and validation sets to monitor convergence and check for overfitting.

## Visualization
The notebook produces visual evaluation plots showing:
1. **Training vs. Validation Accuracy/Loss curves** over 10 epochs.
2. **Sample Test Predictions:** A grid of test images displaying predicted labels alongside true labels (coded green for correct predictions, red for errors).

## How to Run
1. Open the notebook in Google Colab or Jupyter Notebook.
2. Ensure required dependencies are installed:
   ```bash
   pip install tensorflow numpy matplotlib
