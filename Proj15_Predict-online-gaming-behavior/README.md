# Predict Online Gaming Behavior

<p align="center">
  <img src="https://github.com/user-attachments/assets/7a9b4d77-d768-4741-b5c9-759fc342462f" height="300"/>
</p>

## Summary
This project aims to analyze player behavior in online gaming environments by developing machine learning models to predict player retention and engagement. Utilizing a comprehensive dataset, the goal is to uncover patterns that can enhance player experience and optimize game design.

## Objective
- Build classification models to predict player engagement levels.
- Utilize a dataset encompassing various metrics related to player demographics and gaming behavior.
- Improve player retention through insights gained from data analysis.

## Dataset
The dataset includes the following features:

- **PlayerID:** Unique identifier for each player.
- **Age:** Age of the player.
- **Gender:** Gender of the player.
- **Location:** Geographic location of the player.
- **GameGenre:** Genre of the game played.
- **PlayTimeHours:** Average hours spent playing per session.
- **InGamePurchases:** Indicates in-game purchases (0 = No, 1 = Yes).
- **GameDifficulty:** Difficulty level of the game.
- **SessionsPerWeek:** Number of gaming sessions per week.
- **AvgSessionDurationMinutes:** Average session duration in minutes.
- **PlayerLevel:** Current level of the player in the game.
- **AchievementsUnlocked:** Number of achievements unlocked by the player.
- **EngagementLevel:** Target variable reflecting player retention ('High', 'Medium', 'Low').

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, XGBoost, TensorFlow/Keras, Pandas, NumPy
- **Data:** Original dataset by Rabie El Kharoua
- **Metrics:** Accuracy, Precision, Recall, F1 Score

## Best Classical Machine Learning Model

### XGBoost
- **Cross Val Score:** 0.91
- **F1 Score:** 0.92

#### Classification Report
| Engagement Level | Precision | Recall | F1-Score | Support |
|------------------|-----------|--------|----------|---------|
| 0                | 0.91      | 0.89   | 0.90     | 645     |
| 1                | 0.92      | 0.95   | 0.93     | 1211    |
| 2                | 0.92      | 0.90   | 0.91     | 646     |
| **Accuracy**     |           |        | 0.92     | 2502    |
| **Macro Avg**    | 0.92      | 0.91   | 0.91     | 2502    |
| **Weighted Avg** | 0.92      | 0.92   | 0.92     | 2502    |

## Best Deep Neural Network (DNN) Model
- **F1 Score:** 0.48
- **Loss:** 0.3160
