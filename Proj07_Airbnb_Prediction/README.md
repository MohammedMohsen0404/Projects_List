# Airbnb Cleaned Europe Prediction

<p align="center">
  <img src="https://github.com/user-attachments/assets/0c997259-91e8-4347-8acf-2474703a462a" height="300"/>
</p>

## Summary
This project uses a cleaned dataset from Airbnb listings across nine major European cities: Amsterdam, Athens, Barcelona, Berlin, Budapest, Lisbon, Paris, Rome, and Vienna. The original dataset was messy and lacked descriptive information. The goal of this project is to analyze the data and develop predictive models to understand and forecast Airbnb prices based on various factors.

## Objective
- Perform exploratory data analysis (EDA) on the Airbnb dataset.
- Develop a regression model to predict Airbnb prices.
- Analyze the impact of various features on pricing and provide insights.

## Dataset
The dataset includes the following features:

- **City:** City where the listing is located.
- **Price:** Price per night of the listing.
- **Day:** Day of the week (Weekday/Weekend).
- **Room Type:** Type of room (e.g., Private room, Shared room).
- **Shared Room:** Indicator if the room is shared (True/False).
- **Private Room:** Indicator if the room is private (True/False).
- **Person Capacity:** Number of people the room can accommodate.
- **Superhost:** Indicator if the host is a superhost (True/False).
- **Multiple Rooms:** Indicator if the listing includes multiple rooms (True/False).
- **Business:** Indicator if the listing is business-friendly (True/False).
- **Cleanliness Rating:** Rating of cleanliness (1-10 scale).
- **Guest Satisfaction:** Overall guest satisfaction rating (1-100 scale).
- **Bedrooms:** Number of bedrooms in the listing.
- **City Center (km):** Distance from the city center in kilometers.
- **Metro Distance (km):** Distance from the nearest metro station in kilometers.
- **Attraction Index:** Index of nearby attractions.
- **Normalised Attraction Index:** Normalized index of nearby attractions.
- **Restaurant Index:** Index of nearby restaurants.
- **Normalised Restaurant Index:** Normalized index of nearby restaurants.

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn
- **Data:** Airbnb listings dataset
- **Metrics:** R2 Score, Mean Squared Error (MSE), Mean Absolute Error (MAE)

## Best Model
#### Random Forest Regressor
- **R2 Score:** 0.8036
- **Mean Squared Error (MSE):** 0.0026
- **Mean Absolute Error (MAE):** 0.0371
