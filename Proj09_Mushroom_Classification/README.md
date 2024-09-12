# Mushroom Classification

<p align="center">
  <img src="https://github.com/user-attachments/assets/7ad44b9e-7742-4b71-9b8a-719e049914a9" height="300"/>
</p>

## Summary
This project utilizes a dataset of mushroom descriptions to classify mushrooms as either edible or poisonous. The dataset includes various features describing the physical characteristics of mushrooms, such as cap shape, color, and odor. The goal is to develop predictive models that can accurately determine the edibility of a mushroom based on these features. This can aid mushroom foragers in identifying safe mushrooms to eat and avoiding poisonous ones.

## Objective
- Build classification models to predict whether a mushroom is edible or poisonous.
- Use a range of features to improve the accuracy of the classification.
- Provide a reliable tool for identifying edible versus poisonous mushrooms.

## Dataset
The dataset includes the following features:

- **cap-shape:** Shape of the mushroom cap (bell=b, conical=c, convex=x, flat=f, knobbed=k, sunken=s)
- **cap-surface:** Surface texture of the mushroom cap (fibrous=f, grooves=g, scaly=y, smooth=s)
- **cap-color:** Color of the mushroom cap (brown=n, buff=b, cinnamon=c, gray=g, green=r, pink=p, purple=u, red=e, white=w, yellow=y)
- **bruises:** Presence of bruises (bruises=t, no=f)
- **odor:** Odor of the mushroom (almond=a, anise=l, creosote=c, fishy=y, foul=f, musty=m, none=n, pungent=p, spicy=s)
- **gill-attachment:** Gill attachment (attached=a, descending=d, free=f, notched=n)
- **gill-spacing:** Spacing of the gills (close=c, crowded=w, distant=d)
- **gill-size:** Size of the gills (broad=b, narrow=n)
- **gill-color:** Color of the gills (black=k, brown=n, buff=b, chocolate=h, gray=g, green=r, orange=o, pink=p, purple=u, red=e, white=w, yellow=y)
- **stalk-shape:** Shape of the stalk (enlarging=e, tapering=t)
- **stalk-root:** Type of stalk root (bulbous=b, club=c, cup=u, equal=e, rhizomorphs=z, rooted=r, missing=?)
- **stalk-surface-above-ring:** Surface texture above the ring (fibrous=f, scaly=y, silky=k, smooth=s)
- **stalk-surface-below-ring:** Surface texture below the ring (fibrous=f, scaly=y, silky=k, smooth=s)
- **stalk-color-above-ring:** Color above the ring (brown=n, buff=b, cinnamon=c, gray=g, orange=o, pink=p, red=e, white=w, yellow=y)
- **stalk-color-below-ring:** Color below the ring (brown=n, buff=b, cinnamon=c, gray=g, orange=o, pink=p, red=e, white=w, yellow=y)
- **veil-type:** Type of veil (partial=p, universal=u)
- **veil-color:** Color of the veil (brown=n, orange=o, white=w, yellow=y)
- **ring-number:** Number of rings (none=n, one=o, two=t)
- **ring-type:** Type of ring (cobwebby=c, evanescent=e, flaring=f, large=l, none=n, pendant=p, sheathing=s, zone=z)
- **spore-print-color:** Color of the spore print (black=k, brown=n, buff=b, chocolate=h, green=r, orange=o, purple=u, white=w, yellow=y)
- **population:** Population density (abundant=a, clustered=c, numerous=n, scattered=s, several=v, solitary=y)
- **habitat:** Habitat of the mushroom (grasses=g, leaves=l, meadows=m, paths=p, urban=u, waste=w, woods=d)

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn
- **Data:** Mushroom dataset
- **Metrics:** F1 Score, Classification Report

## Best Model

#### XGBoost
- **F1 Score:** 1.00
- Classification Report:

|               | precision | recall | f1-score | support |
|---------------|-----------|--------|----------|---------|
| **0 (edible)**| 1.00      | 1.00   | 1.00     | 1175    |
| **1 (poisonous)** | 1.00   | 1.00   | 1.00     | 1263    |
| **accuracy**  |           |        | 1.00     | 2438    |
| **macro avg** | 1.00      | 1.00   | 1.00     | 2438    |
| **weighted avg** | 1.00    | 1.00   | 1.00     | 2438    |

#### Logistic Regression
- **F1 Score:** 1.00
- Classification Report:

|               | precision | recall | f1-score | support |
|---------------|-----------|--------|----------|---------|
| **0 (edible)**| 1.00      | 1.00   | 1.00     | 1175    |
| **1 (poisonous)** | 1.00   | 1.00   | 1.00     | 1263    |
| **accuracy**  |           |        | 1.00     | 2438    |
| **macro avg** | 1.00      | 1.00   | 1.00     | 2438    |
| **weighted avg** | 1.00    | 1.00   | 1.00     | 2438    |
