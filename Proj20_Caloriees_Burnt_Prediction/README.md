# Calories Burnt Prediction

<p align="center">
  <img src="https://github.com/user-attachments/assets/3bd929bf-4532-424e-bc83-c452d27fd6de" height="300"/>
</p>

## Summary
This project aims to develop a predictive model for calorie burn estimation, leveraging data science techniques to address a key health and wellness challenge. By analyzing various input features—such as the type of physical activity, its duration, intensity, and individual characteristics like age, weight, and gender—the goal is to accurately predict the number of calories burned during a given activity. This model will serve as a valuable tool for individuals, fitness enthusiasts, and healthcare professionals to optimize calorie management and physical activity planning.

## Objective
- Develop a regression model to estimate calories burned based on various physical activity parameters.
- Utilize individual characteristics and activity details for more accurate predictions.
- Provide insights that can help users manage their fitness and health goals effectively.

## Dataset
The dataset includes the following features:

- **User_ID:** Unique identifier for each user.
- **Gender:** Gender of the individual (male/female).
- **Age:** Age of the individual.
- **Height:** Height of the individual in cm.
- **Weight:** Weight of the individual in kg.
- **Duration:** Duration of the activity in minutes.
- **Heart_Rate:** Average heart rate during the activity.
- **Body_Temp:** Body temperature during the activity.
- **Calories:** Target variable representing the calories burned.

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, XGBoost, TensorFlow/Keras, Pandas, NumPy
- **Metrics:** Cross-Validation Score, R² Score, Mean Squared Error (MSE), Mean Absolute Error (MAE)

## Best Classical Machine Learning Models

### XGBRegressor
- **Cross Val Score:** 0.9986
- **R² Score:** 0.9988
- **MSE:** 0.0011
- **MAE:** 0.0226

### Random Forest Regressor
- **Cross Val Score:** 0.9977
- **R² Score:** 0.9981
- **MSE:** 0.0017
- **MAE:** 0.0254

## Best Deep Neural Network (DNN) Model
- **Loss:** 6.0851e-04
- **R² Score:** 0.9993
