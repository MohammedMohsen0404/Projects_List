# Big Mart Sales Prediction
<p align="center">
  <img src="https://github.com/user-attachments/assets/59ab1b47-09a5-4988-93e2-63ee449a7bda" alt="dataset-card" height="500"/>
</p>

## Summary
This project aims to develop an accurate predictive model for forecasting sales at Big Mart using machine learning techniques. The goal is to predict sales of various products across different stores based on historical data and relevant features. The model will help optimize inventory management and stock replenishment strategies.

## Objective
- Build a regression model to predict sales for Big Mart products.
- Utilize historical sales data and relevant features.
- Enhance inventory and stock management through reliable sales forecasts.

## Dataset
The dataset used in this project includes the following features:

- **Item_Identifier:** Unique identifier for the item.
- **Item_Weight:** Weight of the item.
- **Item_Fat_Content:** Indicator of whether the item is low fat or regular.
- **Item_Visibility:** The proportion of the item’s visibility in the store.
- **Item_Type:** Type of item (e.g., Snack, Dairy).
- **Item_MRP:** Maximum Retail Price of the item.
- **Outlet_Identifier:** Unique identifier for the outlet.
- **Outlet_Establishment_Year:** Year the outlet was established.
- **Outlet_Size:** Size of the outlet (e.g., Small, Medium, Large).
- **Outlet_Location_Type:** Location type of the outlet (e.g., Tier 1, Tier 2).
- **Outlet_Type:** Type of outlet (e.g., Supermarket, Grocery Store).
- **Item_Outlet_Sales:** Sales of the item at the outlet (target variable).

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, XGBoost, Pandas, NumPy
- **Data:** Big Mart sales dataset
- **Metrics:** R2 Score, Mean Squared Error (MSE), Mean Absolute Error (MAE)

## Best Model
The best performing model for this project is the **Gradient Boosting Regressor** with the following performance metrics:
- **R2 Score:** 0.6979
- **Mean Squared Error (MSE):** 41.0022
- **Mean Absolute Error (MAE):** 4.9445
