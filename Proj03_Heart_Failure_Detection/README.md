# Heart Failure Detection

<p align="center">
  <img src="https://github.com/user-attachments/assets/1abe0d85-cf88-4bae-bfc0-3b505dadef92" height="300"/>
</p>

## Summary
This project aims to develop a machine learning model to predict the likelihood of heart disease. By using a comprehensive dataset consisting of 1,190 observations compiled from five different heart disease datasets, the goal is to identify individuals at high cardiovascular risk. Early detection and management of heart disease can significantly improve patient outcomes, and this predictive model will assist healthcare professionals in making informed decisions.

## Objective
- Build a classification model to predict the likelihood of heart disease.
- Utilize a dataset with various features related to cardiovascular health.
- Improve patient outcomes through early detection and risk assessment.

## Dataset
The dataset used in this project includes the following features:

- **Age:** Age of the patient.
- **Sex:** Gender of the patient (M/F).
- **ChestPainType:** Type of chest pain experienced.
- **RestingBP:** Resting blood pressure.
- **Cholesterol:** Cholesterol levels.
- **FastingBS:** Fasting blood sugar.
- **RestingECG:** Resting electrocardiogram results.
- **MaxHR:** Maximum heart rate achieved.
- **ExerciseAngina:** Presence of exercise-induced angina.
- **Oldpeak:** Depression induced by exercise relative to rest.
- **ST_Slope:** Slope of the peak exercise ST segment.
- **HeartDisease:** Target variable indicating presence (1) or absence (0) of heart disease.

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, XGBoost, Pandas, NumPy, TensorFlow/Keras
- **Data:** Compiled heart disease dataset
- **Metrics:** Accuracy, Precision, Recall, F1 Score

## Best Classical Machine Learning Model

#### Gradient Boosting
- **F1 Score:** 0.90
#### Classification Report

|               | precision | recall | f1-score | support |
|---------------|-----------|--------|----------|---------|
| **0.0**       | 0.89      | 0.89   | 0.89     | 123     |
| **1.0**       | 0.91      | 0.92   | 0.91     | 153     |
| **accuracy**  |           |        | 0.90     | 276     |
| **macro avg** | 0.90      | 0.90   | 0.90     | 276     |

## Best Deep Neural Network (DNN) Model

### DNN Ensemble Model
- **Accuracy:** 0.86
- **Recall:** 0.86
- **Precision:** 0.89
- **F1 Score:** 0.87
