# Human Stress Detection

<p align="center">
  <img src="https://github.com/user-attachments/assets/2e15c8f1-f78a-4b77-a864-73e537faf5c7" height="300"/>
</p>

## Summary
Human stress detection is crucial in wearable technology and healthcare. This project focuses on detecting and analyzing human stress levels based on physiological data collected from wearable devices. The dataset is designed to classify stress levels into three categories: low stress, normal stress, and high stress.

## Objective
- Develop a classification model to detect and analyze human stress levels.
- Utilize physiological data, including humidity, temperature, and step count.
- Achieve high accuracy in classifying stress levels into three categories.

## Dataset
The dataset used in this project contains the following features:

- **Humidity:** Body humidity.
- **Temperature:** Body temperature.
- **Step Count:** Number of steps taken by the user.
- **Stress Levels:** Classified into three categories - low stress, normal stress, and high stress.

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy
- **Data:** Stress detection dataset
- **Metrics:** Cross-validation Score, F1 Score, Precision, Recall, Accuracy

## Best Models

#### Random Forest
- **Cross-Val Score:** 1.00
- **F1 Score:** 1.00
- **Classification Report:**
  
|               | precision | recall | f1-score | support |
|---------------|-----------|--------|----------|---------|
| **0**         | 1.00      | 1.00   | 1.00     | 151     |
| **1**         | 1.00      | 1.00   | 1.00     | 237     |
| **2**         | 1.00      | 1.00   | 1.00     | 213     |
| **accuracy**  |           |        | 1.00     | 601     |
| **macro avg** | 1.00      | 1.00   | 1.00     | 601     |
| **weighted avg** | 1.00   | 1.00   | 1.00     | 601     |

#### Gradient Boosting
- **Cross-Val Score:** 1.00
- **F1 Score:** 1.00
- **Classification Report:**

|               | precision | recall | f1-score | support |
|---------------|-----------|--------|----------|---------|
| **0**         | 1.00      | 1.00   | 1.00     | 151     |
| **1**         | 1.00      | 1.00   | 1.00     | 237     |
| **2**         | 1.00      | 1.00   | 1.00     | 213     |
| **accuracy**  |           |        | 1.00     | 601     |
| **macro avg** | 1.00      | 1.00   | 1.00     | 601     |
| **weighted avg** | 1.00   | 1.00   | 1.00     | 601     |
