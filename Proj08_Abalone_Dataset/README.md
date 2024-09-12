# Regression with an Abalone Dataset

<p align="center">
  <img src="https://github.com/user-attachments/assets/aa62d9fe-7094-4d77-b0e7-7cd19290d847" height="300"/>
</p>

## Summary
This project focuses on regression tasks using a dataset derived from the original Abalone dataset. The dataset features are similar to, but not identical to, those in the original dataset. The goal is to predict the number of rings on an abalone based on various physical attributes. By exploring and incorporating both the derived dataset and the original Abalone dataset, the project aims to enhance model performance and understanding.

## Objective
- Develop a regression model to predict the number of rings on abalones.
- Utilize features such as length, diameter, height, and weights of abalones.
- Compare the performance of models trained on both the derived dataset and the original Abalone dataset.

## Dataset
The dataset includes the following features:

- **id:** Unique identifier for each abalone.
- **Sex:** Gender of the abalone (F = Female, M = Male, I = Infant).
- **Length:** Length of the abalone (in mm).
- **Diameter:** Diameter of the abalone (in mm).
- **Height:** Height of the abalone (in mm).
- **Whole weight:** Weight of the abalone including the shell (in grams).
- **Whole weight.1:** Alternative measurement of the whole weight.
- **Whole weight.2:** Another alternative measurement of the whole weight.
- **Shell weight:** Weight of the shell (in grams).
- **Rings:** Number of rings, the target variable.


## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn
- **Data:** Derived Abalone dataset and original Abalone dataset
- **Metrics:** R2 Score, Mean Squared Error (MSE), Mean Absolute Error (MAE)

## Best Model

### Gradient Boosting Regressor
- **R2 Score:** 0.7655
- **Mean Squared Error (MSE):** 0.0191
- **Mean Absolute Error (MAE):** 0.1019
