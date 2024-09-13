# Credit Card Clustering

<p align="center">
  <img src="https://github.com/user-attachments/assets/1084e3ac-7736-4dc8-a0f6-cec2fed6e8ea" height="300"/> <!-- Replace with a relevant image -->
</p>

## Summary
This project focuses on customer segmentation for credit card holders to enhance marketing strategies. By analyzing the usage behavior of approximately 9,000 active credit card holders over the past 6 months, the objective is to identify distinct customer segments. This segmentation enables more targeted marketing campaigns and improved customer relationship management.

## Objective
- Develop clustering models to segment credit card users.
- Analyze various usage behaviors to define customer segments.
- Tailor marketing strategies and improve customer relationship management based on identified segments.

## Dataset
The dataset used in this project includes the following features:

- **CUST_ID:** Customer ID.
- **BALANCE:** Credit card balance.
- **BALANCE_FREQUENCY:** Frequency of balance updates.
- **PURCHASES:** Total purchases amount.
- **ONEOFF_PURCHASES:** Total one-off purchases amount.
- **INSTALLMENTS_PURCHASES:** Total installment purchases amount.
- **CASH_ADVANCE:** Total cash advances amount.
- **PURCHASES_FREQUENCY:** Frequency of purchases.
- **ONEOFF_PURCHASES_FREQUENCY:** Frequency of one-off purchases.
- **PURCHASES_INSTALLMENTS_FREQUENCY:** Frequency of installment purchases.
- **CASH_ADVANCE_FREQUENCY:** Frequency of cash advances.
- **CASH_ADVANCE_TRX:** Number of cash advance transactions.
- **PURCHASES_TRX:** Number of purchase transactions.
- **CREDIT_LIMIT:** Credit limit.
- **PAYMENTS:** Total payments amount.
- **MINIMUM_PAYMENTS:** Minimum payments amount.
- **PRC_FULL_PAYMENT:** Percentage of full payment.
- **TENURE:** Tenure in months.

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy, Matplotlib
- **Data:** Credit card usage dataset
- **Metrics:** Silhouette Score, Davies-Bouldin Index, Calinski-Harabasz Index

## Best Clustering Algorithms

#### KMeans
- **Silhouette Score:** 0.4086
- **Davies-Bouldin Index:** 0.7757
- **Calinski-Harabasz Index:** 8378.2768

#### Agglomerative Clustering
- **Silhouette Score:** 0.3546
- **Davies-Bouldin Index:** 0.8675
- **Calinski-Harabasz Index:** 6994.7350
