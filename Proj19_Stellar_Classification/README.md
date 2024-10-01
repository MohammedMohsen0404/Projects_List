# Stellar Classification

<p align="center">
  <img src="https://github.com/user-attachments/assets/543c54fb-5243-4f25-bfe2-322af1df06fa" height="300"/>
</p>

## Summary
The aim of this project is to classify stars into different categories using their spectral data, focusing on identifying giants and dwarfs. The classification is based on absolute magnitude and B-V color index, which are key attributes in the Morgan–Keenan (MK) classification system. This project helps in understanding the characteristics and classification of stars in the stellar spectrum.

## Objective
- Develop a classification model to identify giant and dwarf stars based on spectral data.
- Utilize key attributes such as absolute magnitude and B-V color index for classification.
- Enhance understanding of stellar characteristics through data analysis.

## Dataset
The dataset includes the following features:

- **Vmag:** Apparent magnitude of the star.
- **Plx:** Parallax measurement.
- **e_Plx:** Error in parallax measurement.
- **B-V:** B-V color index, indicating the color of the star.
- **SpType:** Spectral type of the star.
- **Amag:** Absolute magnitude of the star.
- **TargetClass:** Target variable indicating class (0 for giants, 1 for dwarfs).

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, XGBoost, TensorFlow/Keras, Pandas, NumPy
- **Metrics:** F1 Score, Accuracy

## Best Classical Machine Learning Models

### XGBoost
- **F1 Score:** 0.91

#### Classification Report
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.92      | 0.89   | 0.90     | 5933    |
| 1     | 0.89      | 0.92   | 0.91     | 5933    |
| **Accuracy** |     |        | **0.91** | 11866   |
| **Macro Avg** | 0.91 | 0.91   | 0.91     | 11866   |
| **Weighted Avg** | 0.91 | 0.91   | 0.91     | 11866   |

### Random Forest
- **F1 Score:** 0.91

#### Classification Report
| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.92      | 0.89   | 0.90     | 5933    |
| 1     | 0.89      | 0.92   | 0.91     | 5933    |
| **Accuracy** |     |        | **0.91** | 11866   |
| **Macro Avg** | 0.91 | 0.91   | 0.91     | 11866   |
| **Weighted Avg** | 0.91 | 0.91   | 0.91     | 11866   |

## Best Deep Neural Network (DNN) Model
- **F1 Score:** 0.6680
- **Loss:** 0.1964
