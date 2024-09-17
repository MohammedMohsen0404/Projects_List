# Appliances Energy Prediction
<p align="center"> <img src="https://github.com/user-attachments/assets/1685f8c3-6268-4dc9-a6de-215733ae0462" height="300"/> </p>

## Summary
This project involves developing regression models to predict the energy consumption of appliances in a low-energy house. The dataset, collected over approximately 4.5 months, provides experimental data that will be used to optimize energy usage in residential buildings. By leveraging machine learning and deep learning techniques, this project aims to enhance energy efficiency and support sustainable living practices.

## Objective
- Develop regression models to predict energy consumption of appliances.
- Utilize a comprehensive dataset with various environmental and operational features.
- Optimize energy usage and contribute to sustainable energy practices.

## Dataset
The dataset used in this project includes the following features:
- **date:** Timestamp of the data entry.
- **Appliances:** Energy consumption of the appliances in watt-hours.
- **lights:** Energy consumption by the lights in watt-hours.
- **T1:** Temperature in the first room.
- **RH_1:** Relative humidity in the first room.
- **T2:** Temperature in the second room.
- **RH_2:** Relative humidity in the second room.
- **T3:** Temperature in the third room.
- **RH_3:** Relative humidity in the third room.
- **T4:** Temperature in the fourth room.
- **RH_4:** Relative humidity in the fourth room.
- **T_out:** Outside temperature.
- **Press_mm_hg:** Atmospheric pressure.
- **RH_out:** Outside relative humidity.
- **Windspeed:** Wind speed.
- **Visibility:** Visibility distance.
- **Tdewpoint:** Dew point temperature.
- **rv1, rv2:** Random variables.

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy, TensorFlow/Keras
- **Data:** Experimental data from a low-energy building
- **Metrics:** Cross-validation Score, R2 Score, Mean Squared Error (MSE), Mean Absolute Error (MAE)

## Best Classical Machine Learning Model
#### Random Forest Regressor
- **Cross Val Score:** 0.61
- **R2 Score:** 0.60
- **MSE:** 0.17
- **MAE:** 0.23

## Best Deep Neural Network (DNN) Model
- **Loss:** 0.1081
- **R2 Score:** 0.43
