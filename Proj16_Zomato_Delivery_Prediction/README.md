# Zomato Restaurant Analysis

<p align="center">
  <img src="https://github.com/user-attachments/assets/73ce77ee-e746-457e-a159-170aadcd1419" height="300"/>
</p>

## Summary
This project provides extensive insights into restaurants listed on Zomato, focusing on various attributes that influence customer choices, such as online delivery, table booking, location, and restaurant type. The goal is to perform exploratory data analysis, visualization, and regression modeling to uncover patterns and trends in the restaurant industry, particularly in Bengaluru.

## Objective
- Analyze restaurant data to understand customer preferences.
- Build regression models to predict ratings based on various features.
- Provide actionable insights to enhance business strategies in the restaurant industry.

## Dataset
The dataset includes the following features:

- **url:** Link to the restaurant page on Zomato.
- **address:** Address of the restaurant.
- **name:** Name of the restaurant.
- **online_order:** Availability of online ordering (Yes/No).
- **book_table:** Availability of table booking (Yes/No).
- **rate:** Customer rating of the restaurant.
- **votes:** Number of votes received.
- **phone:** Contact number of the restaurant.
- **location:** Area where the restaurant is located.
- **rest_type:** Type of restaurant (e.g., Casual Dining).
- **dish_liked:** Popular dishes among customers.
- **cuisines:** Types of cuisine offered.
- **approx_cost(for two people):** Estimated cost for two people.
- **reviews_list:** List of customer reviews.
- **menu_item:** Menu items available.
- **listed_in(type):** Type of listing.
- **listed_in(city):** City of the restaurant.

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, XGBoost, TensorFlow/Keras, Pandas, NumPy
- **Data:** Zomato restaurant dataset
- **Metrics:** Cross-Validation Score, R² Score, MSE, MAE

## Best Classical Machine Learning Models

### Random Forest Regressor
- **Cross Val Score:** 0.90
- **R² Score:** 0.92
- **MSE:** 0.0349
- **MAE:** 0.1062

### XGBRegressor
- **Cross Val Score:** 0.80
- **R² Score:** 0.79
- **MSE:** 0.0860
- **MAE:** 0.2190

## Best Deep Neural Network (DNN) Model

### DNN Model
- **Loss:** 0.1429
- **R² Score:** 0.6522

