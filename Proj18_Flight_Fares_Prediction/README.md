# Flight Fares Prediction

<p align="center">
  <img src="https://github.com/user-attachments/assets/8921f969-f2f0-4fb0-ab6c-9e8ad617bc88" height="300"/>
</p>

## Summary
This project aims to predict flight fares using machine learning techniques. By analyzing flight data collected from EaseMyTrip, the project seeks to develop models that help users make informed decisions about when and where to purchase flight tickets.

## Objective
- Develop predictive models for flight fares based on various flight details.
- Assist users in identifying the best times to book tickets and save money.
- Provide insights into patterns and trends in flight pricing.

## Dataset
The dataset includes the following features:

- **Date_of_journey:** Date when the flight is booked.
- **Journey_day:** Day of the week for the journey.
- **Airline:** Name of the airline operating the flight.
- **Flight_code:** Code assigned to the flight.
- **Class:** Class of travel (e.g., Economy).
- **Source:** Departure airport.
- **Departure:** Time of departure.
- **Total_stops:** Number of stops (e.g., non-stop).
- **Arrival:** Time of arrival.
- **Destination:** Arrival airport.
- **Duration_in_hours:** Duration of the flight in hours.
- **Days_left:** Days remaining until the journey.
- **Fare:** Price of the flight ticket.

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, XGBoost, TensorFlow/Keras, Pandas, NumPy
- **Metrics:** Cross-Validation Score, R² Score, Mean Squared Error (MSE), Mean Absolute Error (MAE)

## Best Classical Machine Learning Model

### Random Forest Regressor
- **Cross Val Score:** 0.9639
- **R² Score:** 0.9649
- **MSE:** 0.0248
- **MAE:** 0.0956

### XGBRegressor
- **Cross Val Score:** 0.9391
- **R² Score:** 0.9382
- **MSE:** 0.0436
- **MAE:** 0.1539

## Best Deep Neural Network (DNN) Model
- **Loss:** 0.0472
- **R² Score:** 0.9328
