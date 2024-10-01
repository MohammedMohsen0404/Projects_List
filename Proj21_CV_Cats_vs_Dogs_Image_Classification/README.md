# Cats vs Dogs: Image Classification

<p align="center">
  <img src="https://github.com/user-attachments/assets/63d27992-45fc-463a-9b29-e4b7a8fcea16" height="300"/>
</p>

## Summary
This project aims to tackle the classic binary classification problem of distinguishing between images of cats and dogs using Convolutional Neural Networks (CNNs). By leveraging this image dataset, which consists of two classes—cats and dogs—the goal is to build a robust model capable of accurately classifying images into one of these two categories. This task is a fundamental challenge in computer vision, providing a practical application of CNNs in image recognition and classification. The insights gained from this project can be extended to more complex image classification tasks and further exploration in the field of deep learning.

## Objective
- Develop a CNN model to classify images of cats and dogs.
- Achieve high accuracy and F1 scores to validate the effectiveness of the model.
- Provide insights into the model architecture and its performance metrics.

## Dataset
The dataset consists of images categorized into two classes:
- **Class 0:** Cats
- **Class 1:** Dogs

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** TensorFlow/Keras, NumPy, Matplotlib, OpenCV
- **Metrics:** Accuracy, F1 Score, Classification Report

## Model Architecture
The CNN architecture consists of the following layers:

| Layer (type)                    | Output Shape           | Param #       |
|----------------------------------|------------------------|----------------|
| conv2d (Conv2D)                 | (None, 255, 255, 32)   | 896            |
| max_pooling2d (MaxPooling2D)    | (None, 128, 128, 32)   | 0              |
| conv2d_1 (Conv2D)               | (None, 128, 128, 64)   | 18,496         |
| max_pooling2d_1 (MaxPooling2D)  | (None, 64, 64, 64)     | 0              |
| conv2d_2 (Conv2D)               | (None, 64, 64, 128)    | 73,856         |
| max_pooling2d_2 (MaxPooling2D)  | (None, 32, 32, 128)    | 0              |
| flatten (Flatten)               | (None, 131072)         | 0              |
| dense (Dense)                   | (None, 128)            | 16,777,344     |
| dense_1 (Dense)                 | (None, 64)             | 8,256          |
| dense_2 (Dense)                 | (None, 32)             | 2,080          |
| dense_3 (Dense)                 | (None, 1)              | 33             |

- **Total params:** 16,880,961
- **Trainable params:** 16,880,961
- **Non-trainable params:** 0

## Model Performance
- **Training Accuracy:** 100%
- **Validation Accuracy:** 100%
- **F1 Score:** 1.00
- Classification Report

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 1.00      | 1.00   | 1.00     | 2023    |
| 1     | 1.00      | 1.00   | 1.00     | 2023    |
| **Accuracy** |           |        | 1.00     | 4046    |
| **Macro Avg** | 1.00      | 1.00   | 1.00     | 4046    |
| **Weighted Avg** | 1.00      | 1.00   | 1.00     | 4046    |


## Results
<p align="center">
  <img src="https://github.com/user-attachments/assets/cde43c21-a89e-4399-b1d8-3d563799bf78" height="300"/>
</p>


