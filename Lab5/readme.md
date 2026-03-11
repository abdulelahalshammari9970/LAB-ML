# ARTI 308 – Lab 5: Feature Engineering (Classification)

## Overview
This lab focuses on feature engineering for a classification task using a Talabat-style food delivery dataset. The goal is to predict the order status (`Delivered`, `Cancelled`, or `In Transit`) and examine how engineered features affect model performance and feature importance.

## Objective
The main objective of this lab is to build a baseline classification model and improve understanding of how feature engineering influences prediction results. The work includes creating new features, encoding categorical variables, training a Random Forest classifier, and evaluating model performance.

## Dataset
The dataset used in this lab contains food delivery order records. It includes information such as:
- Order price
- Delivery distance
- Order and delivery time
- Driver and customer locations
- Payment and city-related information
- Item names
- Order status

The dataset was already clean:
- No missing values
- No duplicate rows
- Consistent data types

## Tasks Completed

### 1. Dataset inspection
The dataset was loaded and checked for:
- shape
- missing values
- duplicate rows
- target class distribution

### 2. Baseline classification model
A baseline **Random Forest Classifier** was trained to predict `Order_Status`.

### 3. Feature engineering
Several engineered features were created to improve the model, including time-based and category-reduction features.

An additional engineered feature was also created:

- **`price_per_km`** = `Total_Price / Delivery_Distance_km`

This feature was designed to combine order value and delivery effort into one useful measure.

### 4. Peak-hour rule experiment
A different rule for `is_peak_hour` was tested to see whether model performance changed.

### 5. Category reduction experiment
Different values of `top_k` were tested for `Item_Name_reduced`:
- 10
- 30
- 50

The results were compared in terms of:
- accuracy
- top feature importances

### 6. Feature selection
The optional feature selection section using **SelectFromModel** was run to test whether reducing the number of features would help simplify the model without hurting performance.

## Results Summary

### Baseline / Task 2 Accuracy
- Accuracy: **0.85195**

### Task 3 Results (`top_k` comparison)
- `top_k = 10` → Accuracy: **0.85195**
- `top_k = 30` → Accuracy: **0.85195**
- `top_k = 50` → Accuracy: **0.85195**

The top feature importances remained the same across all values:
- `Total_Price`
- `Delivery_Distance_km`
- `Driver_Lon`
- `Driver_Lat`
- `Customer_Lat`

### Feature Selection Result
- Accuracy with feature selection: **0.8519**

## Discussion
The experiments showed that changing the `is_peak_hour` rule had only a small effect on model performance. Similarly, changing `top_k` in `Item_Name_reduced` did not change the model accuracy or the most important features. This suggests that order status prediction in this dataset depends more on numerical and location-based features than on reduced item-name categories.

The feature selection step was helpful because it simplified the model while keeping nearly the same accuracy. However, the classification report showed that the model mainly predicted the majority class (`Delivered`) and performed poorly on the minority classes (`Cancelled` and `In Transit`). This indicates that class imbalance is still an important challenge in this task.

## Conclusion
This lab demonstrated the importance of feature engineering in classification problems. Although some engineered features and experiments had limited impact on accuracy, they helped illustrate how feature design affects model behavior. The most influential predictors were price, delivery distance, and geographic location features. Feature selection also showed that the model could be simplified without a major loss in performance.

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
