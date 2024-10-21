# Chest X-Ray Images (Pneumonia)

<p align="center">
  <img src="https://github.com/user-attachments/assets/ff16427f-5dec-4c14-8a58-c6258c70a6cb" height="300"/>
</p>

## Summary
This project centers around the classification of chest X-ray images to distinguish between cases of pneumonia and normal, healthy lungs. Utilizing deep learning and computer vision techniques, the aim is to develop a model capable of accurately identifying pneumonia from X-ray images, providing an essential tool for medical diagnostics.

## Dataset
The dataset is organized into 3 folders (train, test, val) and contains subfolders for each image category (Pneumonia/Normal). It includes a total of 5,863 X-ray images (JPEG) divided into two categories:

- **Pneumonia:** 3,875 images
- **Normal:** 1,341 images

### Data Distribution
- **Training set:** 
  - NORMAL: 1,341
  - PNEUMONIA: 3,875
- **Validation set:**
  - NORMAL: 8
  - PNEUMONIA: 8
- **Test set:**
  - NORMAL: 234
  - PNEUMONIA: 390

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** TensorFlow/Keras, NumPy, Matplotlib, OpenCV
- **Metrics:** Accuracy, Precision, Recall, F1 Score, Confusion Matrix

## Model Architecture
The model architecture is as follows:

| Layer (type)                    | Output Shape           | Param #       |
|----------------------------------|------------------------|----------------|
| xception (Functional)           | ?                      | 20,861,480     |
| batch_normalization (BatchNormalization) | ?               | 0 (unbuilt)    |
| dropout (Dropout)               | ?                      | 0 (unbuilt)    |
| dense (Dense)                   | ?                      | 0 (unbuilt)    |
| dropout_1 (Dropout)             | ?                      | 0 (unbuilt)    |
| dense_1 (Dense)                 | ?                      | 0 (unbuilt)    |
| dense_2 (Dense)                 | ?                      | 0 (unbuilt)    |

- **Total params:** 20,861,480 (79.58 MB)
- **Trainable params:** 0 (0.00 B)
- **Non-trainable params:** 20,861,480 (79.58 MB)

## Model Performance
- **Training Accuracy:** 94.88%
- **Training Loss:** 0.1266
- **Test Accuracy:** 89.10%
- **Test Loss:** 0.2915

### Confusion Matrix

|               | NORMAL | PNEUMONIA |
|---------------|--------|-----------|
| **NORMAL**    | 203    | 31        |
| **PNEUMONIA** | 37     | 353       |

### Classification Report

| Class       | Precision | Recall | F1-Score | Support |
|-------------|-----------|--------|----------|---------|
| NORMAL      | 0.85      | 0.87   | 0.86     | 234     |
| PNEUMONIA   | 0.92      | 0.91   | 0.91     | 390     |
| **Accuracy**|           |        | 0.89     | 624     |
| **Macro Avg**| 0.88     | 0.89   | 0.88     | 624     |
| **Weighted Avg**| 0.89  | 0.89   | 0.89     | 624     |

## Samples
<p align="center">
  <img src="https://github.com/user-attachments/assets/c6e7b4d7-b26c-49d2-9016-2ed1cd2baa2c"/>
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/88fd98d3-5271-4e66-aebc-4924e6b84125"/>
</p>
