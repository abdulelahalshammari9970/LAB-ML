# Decision Trees & Random Forest - Lab 9

## Overview
This lab explores tree-based machine learning models, specifically **Decision Trees** and **Random Forest**, for classification tasks. The objective is to build, train, and evaluate models to predict outcomes based on input features.

## Dataset
The dataset used:
- `loan_data.csv`

It includes information about loan applicants and a target variable indicating whether the loan is approved or not.

## Libraries Used
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Steps Performed

1. **Data Loading**
   - Loaded the dataset using pandas.

2. **Exploratory Data Analysis (EDA)**
   - Analyzed relationships between variables.
   - Visualized data distributions.

3. **Data Preprocessing**
   - Handled categorical variables.
   - Converted features into a suitable format for modeling.

4. **Train-Test Split**
   - Split the dataset into training and testing sets.

5. **Decision Tree Model**
   - Trained a Decision Tree classifier.
   - Evaluated performance.

6. **Random Forest Model**
   - Trained a Random Forest classifier.
   - Compared results with Decision Tree.

## Results
- Random Forest generally performed better than Decision Tree.
- Improved accuracy and reduced overfitting.

## Conclusion
This lab highlights:
- The effectiveness of ensemble methods like Random Forest
- The importance of model comparison
- How tree-based models handle classification problems
