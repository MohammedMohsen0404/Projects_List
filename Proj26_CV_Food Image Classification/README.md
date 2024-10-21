# Food Image Classification

<p align="center">
  <img src="https://github.com/user-attachments/assets/705f862b-a960-4043-9f42-76971f6fefde" height="300"/>
</p>

## Summary
This project aims to leverage the dataset of 16,643 food images, organized into 11 major food categories, to develop and refine food classification models. By utilizing the evaluation, training, and validation splits provided, the goal is to build a robust model capable of accurately identifying and categorizing different food types. This work is intended to enhance food recognition systems and contribute to applications in areas such as dietary tracking and food-related artificial intelligence.

## Dataset

This dataset contains 16,643 food images grouped in 11 major food categories.

There are 3 splits in this dataset:
- Training set   9,866
- Validation set 3,430
- Test set 3,347

### Classes Present in Dataset
- **0:** Bread
- **1:** Dairy product
- **2:** Dessert
- **3:** Egg
- **4:** Fried food
- **5:** Meat
- **6:** Noodles-Pasta
- **7:** Rice
- **8:** Seafood
- **9:** Soup
- **10:** Vegetable-Fruit

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** TensorFlow/Keras, NumPy, Matplotlib
- **Metrics:** Accuracy, Precision, Recall, F1 Score, Confusion Matrix

## Model: 

**EfficientNetB7 with Extra Layers**

| Layer (type)                   | Output Shape         | Param #   | Connected to             |
|--------------------------------|----------------------|-----------|--------------------------|
| efficientnetb7 (EfficientNetB7)| (None, 7, 7, 2560)   | 66,244,336 | -                        |
| global_average_pooling2d       | (None, 2560)         | 0         | efficientnetb7[0][0]    |
| dense                           | (None, 512)          | 1,310,720 | global_average_pooling2d[0][0] |
| dense_1                         | (None, 64)           | 32,832    | dense[0][0]             |
| dense_2                         | (None, 11)           | 715       | dense_1[0][0]           |

- **Total params:** 67,588,603  
- **Trainable params:** 1,344,267  
- **Non-trainable params:** 66,244,336  

## Model Performance
- **Training Accuracy:** 91.56%
- **Training Loss:** 0.25
- **Test Accuracy:** 87.87%
- **Test Loss:** 0.37

### Classification Report

| Class            | Precision | Recall | F1-Score | Support |
|------------------|-----------|--------|----------|---------|
| Bread            | 0.84      | 0.83   | 0.83     | 368     |
| Dairy product    | 0.88      | 0.71   | 0.78     | 148     |
| Dessert          | 0.86      | 0.78   | 0.82     | 500     |
| Egg              | 0.87      | 0.84   | 0.85     | 335     |
| Fried food       | 0.83      | 0.88   | 0.85     | 287     |
| Meat             | 0.84      | 0.93   | 0.88     | 432     |
| Noodles-Pasta    | 0.94      | 0.99   | 0.96     | 147     |
| Rice             | 0.90      | 0.97   | 0.93     | 96      |
| Seafood          | 0.89      | 0.89   | 0.89     | 303     |
| Soup             | 0.96      | 0.96   | 0.96     | 500     |
| Vegetable-Fruit  | 0.92      | 0.94   | 0.93     | 231     |
| **Accuracy**     |           |        | 0.88     | 3347    |
| **Macro Avg**    | 0.88      | 0.88   | 0.88     | 3347    |
| **Weighted Avg** | 0.88      | 0.88   | 0.88     | 3347    |


## Samples 
<p align="center">
  <img src="https://github.com/user-attachments/assets/d342d030-7bb6-4acd-9122-ee65fcfcf8a0"/>
</p>
