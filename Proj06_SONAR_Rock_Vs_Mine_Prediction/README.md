# SONAR Rock Vs Mine Prediction

<p align="center">
  <img src="https://github.com/user-attachments/assets/2166d146-5329-48a7-801e-53440736fceb" height="300"/> 
</p>

## Summary
The SONAR Rock Vs Mine Prediction project is a classification machine learning problem. The goal is to develop a model that can accurately distinguish between metal cylinders (mines) and rocks based on SONAR return data. This project is part of the 100 Days 100 ML Projects Challenge and aims to leverage machine learning techniques to classify sonar returns.

## Objective
- Develop a classification model to differentiate between mines and rocks using SONAR data.
- Analyze and preprocess SONAR return data to train and test the model.
- Achieve high accuracy in distinguishing between the two classes.

## Dataset
The dataset used in this project consists of SONAR return data with the following format:

- **Features:** 60 columns of SONAR return values.
- **Target:** Label indicating whether the observation is a mine (1) or a rock (0).

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, XGBoost, Pandas, NumPy
- **Data:** SONAR return data
- **Metrics:** F1 Score, Precision, Recall, Accuracy

## Best Model

#### XGBoost
- **F1 Score:** 0.86
- Classification Report:
  
|               | precision | recall | f1-score | support |
|---------------|-----------|--------|----------|---------|
| **0**         | 0.88      | 0.85   | 0.86     | 33      |
| **1**         | 0.84      | 0.87   | 0.85     | 30      |
| **accuracy**  |           |        | 0.86     | 63      |
| **macro avg** | 0.86      | 0.86   | 0.86     | 63      |
| **weighted avg** | 0.86   | 0.86   | 0.86     | 63      |
