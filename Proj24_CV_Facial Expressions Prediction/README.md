# Facial Expressions

<p align="center">
  <img src="https://github.com/user-attachments/assets/5559c1c7-b830-47e6-98b8-1f783d41ba0e" height="300"/>
</p>


## Summary
This project aims to develop a model for facial expression recognition using the FER-2013 dataset. The dataset consists of 48x48 pixel grayscale images of faces, with each face automatically registered to ensure consistency in size and positioning within the images.

## Dataset
The dataset contains a total of **22,968 images** for training, **5,741 images** for validation, and **7,178 images** for testing, categorized into 7 classes:

- **0:** Angry
- **1:** Disgust
- **2:** Fear
- **3:** Happy
- **4:** Neutral
- **5:** Sad
- **6:** Surprise

### Data Distribution
- **Training set:** 22,968 images
- **Validation set:** 5,741 images
- **Test set:** 7,178 images

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** TensorFlow/Keras, NumPy, Matplotlib
- **Metrics:** Accuracy, Precision, Recall, F1 Score, Confusion Matrix

## Model Architecture
The model architecture is as follows:

| Layer (type)                | Output Shape         | Param #      |
|-----------------------------|----------------------|--------------|
| input_layer                 | (None, 48, 48, 3)    | 0            |
| standardized_conv2d        | (None, 16, 16, 32)   | 896          |
| batch_normalization         | (None, 16, 16, 32)   | 128          |
| conv2d                     | (None, 16, 16, 32)   | 9,248        |
| conv2d_1                   | (None, 16, 16, 32)   | 9,248        |
| conv2d_3                   | (None, 16, 16, 32)   | 9,248        |
| max_pooling2d              | (None, 8, 8, 32)     | 0            |
| conv2d_4                   | (None, 8, 8, 32)     | 9,248        |
| concatenate                 | (None, 8, 8, 64)     | 0            |
| batch_normalization_1       | (None, 8, 8, 64)     | 256          |
| conv2d_5                   | (None, 8, 8, 64)     | 36,928       |
| conv2d_6                   | (None, 8, 8, 64)     | 36,928       |
| BeforeFinal_Layer          | (None, 8, 8, 64)     | 36,928       |
| max_pooling2d_1            | (None, 4, 4, 64)     | 0            |
| conv2d_9                   | (None, 4, 4, 64)     | 36,928       |
| conv2d_2                   | (None, 4, 4, 32)     | 1,056        |
| concatenate_1               | (None, 4, 4, 160)    | 0            |
| batch_normalization_2       | (None, 4, 4, 160)    | 640          |
| conv2d_10                  | (None, 4, 4, 128)    | 184,448      |
| conv2d_11                  | (None, 4, 4, 128)    | 147,584      |
| conv2d_14                  | (None, 4, 4, 128)    | 147,584      |
| conv2d_12                  | (None, 4, 4, 128)    | 147,584      |
| conv2d_15                  | (None, 2, 2, 128)     | 147,584      |
| max_pooling2d_2            | (None, 2, 2, 128)     | 0            |
| batch_normalization_3       | (None, 2, 2, 128)     | 512          |
| conv2d_7                   | (None, 2, 2, 32)      | 2,080        |
| concatenate_2               | (None, 2, 2, 288)     | 0            |
| conv2d_16                  | (None, 2, 2, 256)     | 663,808      |
| conv2d_17                  | (None, 2, 2, 256)     | 590,080      |
| conv2d_19                  | (None, 2, 2, 64)      | 147,520      |
| conv2d_18                  | (None, 2, 2, 256)     | 590,080      |
| conv2d_20                  | (None, 1, 1, 256)     | 147,712      |
| max_pooling2d_3            | (None, 1, 1, 256)     | 0            |
| batch_normalization_4       | (None, 1, 1, 256)     | 1,024        |
| conv2d_13                  | (None, 1, 1, 32)      | 4,128        |
| concatenate_3               | (None, 1, 1, 544)     | 0            |
| Final_Layer                 | (None, 1, 1, 512)     | 2,507,264    |
| batch_normalization_5       | (None, 1, 1, 512)     | 2,048        |
| flatten                     | (None, 512)            | 0            |
| dropout                     | (None, 512)            | 0            |
| dense                       | (None, 1024)           | 525,312      |
| dropout_1                   | (None, 1024)           | 0            |
| dense_1                     | (None, 7)              | 7,175        |

- **Total params:** 6,188,135 (23.61 MB)
- **Trainable params:** 6,185,831 (23.60 MB)
- **Non-trainable params:** 2,304 (9.00 KB)

## Model Performance
- **Training Accuracy:** 45.33%
- **Training Loss:** 0.3032
- **Test Accuracy:** 45.85%
- **Test Loss:** 0.3019

### Classification Report

| Class       | Precision | Recall | F1-Score | Support |
|-------------|-----------|--------|----------|---------|
| Angry       | 0.37      | 0.12   | 0.18     | 958     |
| Disgust     | 0.14      | 0.71   | 0.23     | 111     |
| Fear        | 0.18      | 0.01   | 0.01     | 1,024   |
| Happy       | 0.75      | 0.79   | 0.77     | 1,774   |
| Neutral     | 0.33      | 0.57   | 0.41     | 1,233   |
| Sad         | 0.34      | 0.25   | 0.29     | 1,247   |
| Surprise    | 0.52      | 0.80   | 0.63     | 831     |
| **Accuracy**        |      |        | 0.46     | 7,178   |
| **Macro Avg**      | 0.37 | 0.47   | 0.36     | 7,178   |
| **Weighted Avg**   | 0.44 | 0.46   | 0.41     | 7,178   |

## Samples
<p align="center">
  <img src="https://github.com/user-attachments/assets/f3944fe3-5656-4ba3-93f0-5ebe0567f218"/>
  <img src="https://github.com/user-attachments/assets/889f8f95-6fc9-439a-9d85-5b05308fd6d5"/>
</p>




