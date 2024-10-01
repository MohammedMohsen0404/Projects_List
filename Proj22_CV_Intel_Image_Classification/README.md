# Intel Image Classification

<p align="center">
  <img src="https://github.com/user-attachments/assets/2c2cf3ad-b230-451c-9ae7-3e871c6a0439" height="300"/>
</p>

## Summary
This project focuses on the multi-class image classification of natural scenes using deep learning techniques. The dataset, provided by Intel, contains approximately 25,000 images of size 150x150, categorized into six different scene types: buildings, forests, glaciers, mountains, seas, and streets. By leveraging this dataset, the goal is to develop a model that can accurately classify images into these categories, providing insights into scene recognition and classification in computer vision.

## Dataset
The dataset consists of 11,230 images belonging to six classes:

- **0:** Buildings
- **1:** Forest
- **2:** Glacier
- **3:** Mountain
- **4:** Sea
- **5:** Street

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** TensorFlow/Keras, NumPy, Matplotlib, OpenCV
- **Metrics:** Accuracy, Precision, Recall, F1 Score, Classification Report

## Model Architecture
The model architecture is as follows:

| Layer (type)                    | Output Shape           | Param #       |
|----------------------------------|------------------------|----------------|
| conv2d (Conv2D)                 | (None, 255, 255, 32)   | 896            |
| max_pooling2d (MaxPooling2D)    | (None, 128, 128, 32)   | 0              |
| conv2d_1 (Conv2D)               | (None, 128, 128, 64)   | 18,496         |
| max_pooling2d_1 (MaxPooling2D)  | (None, 64, 64, 64)     | 0              |
| conv2d_2 (Conv2D)               | (None, 64, 64, 128)    | 73,856         |
| max_pooling2d_2 (MaxPooling2D)  | (None, 32, 32, 128)    | 0              |
| conv2d_3 (Conv2D)               | (None, 32, 32, 64)     | 73,792         |
| max_pooling2d_3 (MaxPooling2D)  | (None, 16, 16, 64)     | 0              |
| flatten (Flatten)               | (None, 16384)          | 0              |
| dense (Dense)                   | (None, 128)            | 2,097,280      |
| dense_1 (Dense)                 | (None, 64)             | 8,256          |
| dense_2 (Dense)                 | (None, 32)             | 2,080          |
| dense_3 (Dense)                 | (None, 6)              | 198            |

- **Total params:** 2,274,854
- **Trainable params:** 2,274,854
- **Non-trainable params:** 0

## Model Performance
- **Training Accuracy:** 87.53%
- **Training Loss:** 0.35
- **Test Accuracy:** 86.70%
- **Test Loss:** 0.39

### Classification Report

| Class       | Precision | Recall | F1-Score | Support |
|-------------|-----------|--------|----------|---------|
| Buildings   | 0.81      | 0.90   | 0.85     | 437     |
| Forest      | 0.98      | 0.96   | 0.97     | 474     |
| Glacier     | 0.86      | 0.80   | 0.83     | 553     |
| Mountain    | 0.81      | 0.81   | 0.81     | 525     |
| Sea         | 0.85      | 0.90   | 0.87     | 510     |
| Street      | 0.91      | 0.86   | 0.88     | 501     |
| **Accuracy**|           |        | 0.87     | 3000    |
| **Macro Avg**| 0.87     | 0.87   | 0.87     | 3000    |
| **Weighted Avg**| 0.87   | 0.87   | 0.87     | 3000    |

## Samples
<p align="center">
  <img src="https://github.com/user-attachments/assets/a06b5957-8688-490f-b8c9-a5a0d8e7aaa9"/>
</p>

