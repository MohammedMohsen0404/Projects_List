# Customer Clustering

<p align="center">
  <img src="https://github.com/user-attachments/assets/a1295e58-5d5a-4608-9199-2f6d5f82fea4" height="300"/>
</p>

## Summary
Customer segmentation is a critical process in market analysis that involves dividing a market into distinct groups of customers who share similar characteristics. This project aims to cluster customers based on various attributes to identify different customer segments. By understanding these segments, companies can tailor their products and services to better meet the needs of their diverse customer base, thereby gaining a competitive edge.

## Objective
- Perform customer segmentation to identify distinct customer groups.
- Use clustering algorithms to group customers based on attributes such as age, income, and occupation.
- Utilize these insights to develop targeted marketing strategies and improve customer satisfaction.

## Dataset
The dataset includes the following attributes:

- **ID:** Unique identifier for the customer.
- **Sex:** Gender of the customer (0=Male, 1=Female).
- **Marital status:** Marital status of the customer (0=Single, 1=Married).
- **Age:** Age of the customer.
- **Education:** Level of education (1=Low, 2=Medium, 3=High).
- **Income:** Annual income of the customer.
- **Occupation:** Occupation of the customer (0=Unemployed, 1=Employed).
- **Settlement size:** Size of the settlement where the customer resides (0=Small, 1=Medium, 2=Large).

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn
- **Data:** Customer dataset
- **Metrics:** Silhouette Score, Davies-Bouldin Index, Calinski-Harabasz Index

## Clustering Algorithms and Evaluation

#### KMeans
- **Number of Clusters:** 4
- **Silhouette Score:** 0.5428
- **Davies-Bouldin Index:** 0.5399
- **Calinski-Harabasz Index:** 4456.6133

#### Agglomerative
- **Silhouette Score:** 0.5318
- **Davies-Bouldin Index:** 0.5514
- **Calinski-Harabasz Index:** 4366.3156

## Conclusion
Both KMeans and Agglomerative clustering algorithms were used to segment customers into distinct groups. The evaluation metrics indicate the effectiveness of each algorithm in forming meaningful clusters. KMeans showed a slightly higher Silhouette Score and Calinski-Harabasz Index, suggesting better-defined clusters compared to Agglomerative clustering.

