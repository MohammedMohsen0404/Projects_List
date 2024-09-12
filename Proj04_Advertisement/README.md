# Advertisement Click Prediction

<p align="center">
  <img src="https://github.com/user-attachments/assets/65c662c9-41dd-4ba7-9c02-007451115bcf" height="200"/>
</p>

## Summary
This project aims to develop a predictive model to determine whether a consumer will click on an advertisement based on various features. By analyzing a dataset containing consumer demographics, behavioral metrics, and geographic details, the goal is to optimize ad targeting and improve campaign effectiveness.

## Objective
- Build a predictive model to forecast whether a consumer will click on an advertisement.
- Analyze consumer demographics, behavioral metrics, and geographic details to improve ad targeting.
- Evaluate the model's performance using accuracy as the primary metric.

## Dataset
The dataset includes the following features:

- **Daily Time Spent on Site:** Time spent by the consumer on the website (in minutes).
- **Age:** Age of the consumer.
- **Area Income:** Income of the consumer's area (in USD).
- **Daily Internet Usage:** Daily internet usage of the consumer (in minutes).
- **Ad Topic Line:** The text of the advertisement.
- **City:** The city of the consumer.
- **Male:** Gender of the consumer (0 = Female, 1 = Male).
- **Country:** The country of the consumer.
- **Timestamp:** The date and time when the data was recorded.
- **Clicked on Ad:** Target variable indicating whether the ad was clicked (1) or not (0).

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy
- **Metrics:** Accuracy

## Best Model

### Logistic Regression
- **Accuracy:** 0.96

### Naive Bayes
- **Accuracy:** 0.96

### Support Vector Machine
- **Accuracy:** 0.95
