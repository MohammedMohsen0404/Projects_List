# Insurance Claim Prediction

<p align="center">
  <img src="https://github.com/user-attachments/assets/32251377-1f4d-495c-a1b3-1b6f112dffd3" height="300"/>
</p>

## Summary
The Insurance Claim Prediction project falls under the Classification Machine Learning Problem category. The project aims to develop a machine learning model capable of accurately predicting whether an insurance claim will be made based on various personal and demographic attributes of the policyholder. By leveraging a dataset with information on age, sex, BMI, steps, children, smoker status, region, and charges, the goal is to assist insurance companies in predicting claims and managing risks more effectively.

## Objective
- Develop a classification model to predict the likelihood of an insurance claim.
- Use a dataset with personal and demographic attributes of policyholders.
- Enhance risk management and decision-making processes for insurance companies.

## Dataset
The dataset used in this project includes the following features:

- **Age:** Age of the policyholder.
- **Sex:** Gender of the policyholder (0: Female, 1: Male).
- **BMI:** Body Mass Index of the policyholder.
- **Steps:** Number of steps walked.
- **Children:** Number of children/dependents.
- **Smoker:** Whether the policyholder is a smoker (0: No, 1: Yes).
- **Region:** The region of residence.
- **Charges:** Medical charges.
- **InsuranceClaim:** Target variable indicating if an insurance claim was made (1: Yes, 0: No).

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, XGBoost, Pandas, NumPy
- **Data:** Insurance claim dataset
- **Metrics:** Accuracy, Precision, Recall, F1 Score

## Best Classical Machine Learning Models

#### Gradient Boosting
- **F1 Score:** 0.98
- Classification Report

|               | precision | recall | f1-score | support |
|---------------|-----------|--------|----------|---------|
| **0**         | 0.96      | 0.98   | 0.97     | 167     |
| **1**         | 0.99      | 0.97   | 0.98     | 235     |
| **accuracy**  |           |        | 0.98     | 402     |
| **macro avg** | 0.97      | 0.98   | 0.97     | 402     |
| **weighted avg** | 0.98   | 0.98   | 0.98     | 402     |

#### XGBoost
- **F1 Score:** 0.98
- Classification Report

|               | precision | recall | f1-score | support |
|---------------|-----------|--------|----------|---------|
| **0**         | 0.98      | 0.98   | 0.98     | 167     |
| **1**         | 0.98      | 0.98   | 0.98     | 235     |
| **accuracy**  |           |        | 0.98     | 402     |
| **macro avg** | 0.98      | 0.98   | 0.98     | 402     |
| **weighted avg** | 0.98   | 0.98   | 0.98     | 402     |
