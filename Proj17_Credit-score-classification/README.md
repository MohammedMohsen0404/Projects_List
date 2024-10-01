# Credit Score Classification

<p align="center">
  <img src="https://github.com/user-attachments/assets/8c99e111-1101-4924-8e22-4594e7c429a8" height="300"/>
</p>

## Summary
This project focuses on developing a machine learning model to classify credit scores based on a person's credit-related information. The aim is to assist a global finance company in automating the segregation of individuals into credit score brackets, thereby reducing manual efforts and improving efficiency.

## Objective
- Develop a classification model to predict credit scores based on various features.
- Automate the process of credit score classification to enhance operational efficiency.
- Provide insights into factors influencing credit scores.

## Dataset
The dataset includes the following features:

- **ID:** Unique identifier for each record.
- **Customer_ID:** Unique identifier for each customer.
- **Month:** Month of the record.
- **Name:** Name of the customer.
- **Age:** Age of the customer.
- **SSN:** Social Security Number of the customer.
- **Occupation:** Job title of the customer.
- **Annual_Income:** Annual income of the customer.
- **Monthly_Inhand_Salary:** Monthly salary received.
- **Num_Bank_Accounts:** Number of bank accounts held by the customer.
- **Num_Credit_Card:** Number of credit cards owned.
- **Interest_Rate:** Interest rate applicable to loans.
- **Num_of_Loan:** Number of loans taken.
- **Type_of_Loan:** Types of loans taken by the customer.
- **Delay_from_due_date:** Days delayed in payment.
- **Num_of_Delayed_Payment:** Number of delayed payments.
- **Changed_Credit_Limit:** Changed credit limit status.
- **Num_Credit_Inquiries:** Number of credit inquiries made.
- **Credit_Mix:** Type of credit (e.g., good, bad).
- **Outstanding_Debt:** Total outstanding debt.
- **Credit_Utilization_Ratio:** Ratio of credit used to total credit available.
- **Credit_History_Age:** Duration of credit history.
- **Payment_of_Min_Amount:** Status of minimum payment.
- **Total_EMI_per_month:** Total Equated Monthly Installment.
- **Amount_invested_monthly:** Monthly investment amount.
- **Payment_Behaviour:** Behaviour regarding payments.
- **Monthly_Balance:** Monthly account balance.
- **Credit_Score:** Target variable representing the credit score category.

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, TensorFlow/Keras, Pandas, NumPy
- **Metrics:** Cross-Validation Score, F1 Score, Accuracy

## Best Classical Machine Learning Model

### Random Forest
- **Cross Val Score:** 0.79
- **F1 Score:** 0.81

#### Classification Report
| Credit Score Class | Precision | Recall | F1-Score | Support |
|---------------------|-----------|--------|----------|---------|
| 0                   | 0.81      | 0.83   | 0.82     | 1450    |
| 1                   | 0.83      | 0.82   | 0.83     | 2658    |
| 2                   | 0.73      | 0.74   | 0.74     | 892     |
| **Accuracy**        |           |        | 0.81     | 5000    |
| **Macro Avg**       | 0.79      | 0.80   | 0.79     | 5000    |
| **Weighted Avg**    | 0.81      | 0.81   | 0.81     | 5000    |

## Best Deep Neural Network (DNN) Model
- **F1 Score:** 0.4644
- **Loss:** 0.6481
