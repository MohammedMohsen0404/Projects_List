# Bank Note Authentication UCI

<p align="center">
  <img src="https://github.com/user-attachments/assets/952b7d1b-7a45-4c7d-bca9-ba318a5cf846" height="300"/>
</p>

## Summary
This dataset originates from images of genuine and forged banknotes, captured using an industrial camera typically used for print inspection. The images have a resolution of approximately 660 dpi and are grayscale with dimensions of 400x400 pixels. Features extracted using Wavelet Transform from these images enable binary classification tasks. The objective is to develop machine learning models that accurately distinguish between genuine and forged banknotes based on these extracted features.

## Objective
- Develop a classification model to distinguish between genuine and forged banknotes.
- Utilize features extracted from grayscale images of banknotes using Wavelet Transform.
- Achieve high accuracy in binary classification tasks for detecting counterfeit notes.

## Dataset
The dataset includes the following features:

- **Variance:** Variance of Wavelet Transformed image (continuous).
- **Skewness:** Skewness of Wavelet Transformed image (continuous).
- **Curtosis:** Curtosis of Wavelet Transformed image (continuous).
- **Entropy:** Entropy of image (continuous).
- **Class:** Class label indicating genuine (0) or forged (1) banknote.

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, XGBoost, Pandas, NumPy, TensorFlow/Keras
- **Data:** Banknote images dataset
- **Metrics:** Accuracy, Precision, Recall, F1 Score

## Best Classical Machine Learning Models

#### Random Forest
- **F1 Score:** 1.00
- Classification Report

|               | precision | recall | f1-score | support |
|---------------|-----------|--------|----------|---------|
| **0**         | 1.00      | 1.00   | 1.00     | 191     |
| **1**         | 1.00      | 1.00   | 1.00     | 152     |
| **accuracy**  |           |        | 1.00     | 343     |
| **macro avg** | 1.00      | 1.00   | 1.00     | 343     |
| **weighted avg** | 1.00   | 1.00   | 1.00     | 343     |

#### K-Nearest Neighbors
- **F1 Score:** 1.00
- Classification Report

|               | precision | recall | f1-score | support |
|---------------|-----------|--------|----------|---------|
| **0**         | 1.00      | 1.00   | 1.00     | 191     |
| **1**         | 1.00      | 1.00   | 1.00     | 152     |
| **accuracy**  |           |        | 1.00     | 343     |
| **macro avg** | 1.00      | 1.00   | 1.00     | 343     |
| **weighted avg** | 1.00   | 1.00   | 1.00     | 343     |

#### Gradient Boosting
- **F1 Score:** 1.00
- Classification Report

|               | precision | recall | f1-score | support |
|---------------|-----------|--------|----------|---------|
| **0**         | 1.00      | 1.00   | 1.00     | 191     |
| **1**         | 1.00      | 1.00   | 1.00     | 152     |
| **accuracy**  |           |        | 1.00     | 343     |
| **macro avg** | 1.00      | 1.00   | 1.00     | 343     |
| **weighted avg** | 1.00   | 1.00   | 1.00     | 343     |

## Best Deep Neural Network (DNN) Model
- **F1 Score:** 1.00
- Classification Report

|               | precision | recall | f1-score | support |
|---------------|-----------|--------|----------|---------|
| **0**         | 1.00      | 1.00   | 1.00     | 191     |
| **1**         | 1.00      | 1.00   | 1.00     | 152     |
| **accuracy**  |           |        | 1.00     | 343     |
| **macro avg** | 1.00      | 1.00   | 1.00     | 343     |
| **weighted avg** | 1.00   | 1.00   | 1.00     | 343     |
