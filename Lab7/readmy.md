# Logistic Regression Assignment
### ARTI308 - Machine Learning

---

##  Assignment Overview

This assignment applies **Logistic Regression** to predict whether an internet user will click on an advertisement based on their behavior and demographic data.

The goal is to build, train, and evaluate a classification model using real-world-style data.

---

##  Dataset — advertising.csv

The dataset contains **1000 records** of internet users with the following features:

| Column | Description |
|--------|-------------|
| `Daily Time Spent on Site` | Time the consumer spent on the site (in minutes) |
| `Age` | Age of the customer (in years) |
| `Area Income` | Average income of the consumer's geographical area |
| `Daily Internet Usage` | Average minutes per day the consumer spends on the internet |
| `Ad Topic Line` | Headline of the advertisement |
| `City` | City of the consumer |
| `Male` | Whether the consumer is male (1) or not (0) |
| `Country` | Country of the consumer |
| `Timestamp` | Time at which the consumer clicked on the ad or closed the window |
| `Clicked on Ad` | Target variable — 0 (did not click) or 1 (clicked) |

---

##  What the Notebook Does

1. **Imports** necessary libraries (pandas, numpy, matplotlib, seaborn, sklearn)
2. **Loads** the `advertising.csv` dataset
3. **Explores** the data using `.head()`, `.info()`, and `.describe()`
4. **Visualizes** the data using:
   - Histogram of Age distribution
   - Jointplot of Area Income vs Age
   - Jointplot (KDE) of Daily Time Spent on Site vs Age
   - Jointplot of Daily Time Spent on Site vs Daily Internet Usage
   - Pairplot with hue based on `Clicked on Ad`
5. **Prepares** features: selects numeric columns relevant for prediction
6. **Splits** the data into training and testing sets (67% / 33%)
7. **Trains** a Logistic Regression model (`max_iter=1000`)
8. **Evaluates** the model using a Classification Report

---

##  Model Results

```
              precision    recall  f1-score   support

           0       0.86      0.96      0.91       162
           1       0.96      0.85      0.90       168

    accuracy                           0.91       330
```

The model achieved **91% accuracy** on the test set.

---

## How to Run

1. Make sure you have the following libraries installed:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
2. Place `advertising.csv` in the same directory as the notebook
3. Open `02-Logistic_Regression_Assignment_Completed.ipynb` in Jupyter
4. Run all cells in order
