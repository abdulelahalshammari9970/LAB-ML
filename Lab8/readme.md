# K-Nearest Neighbors (KNN) - Lab 8

## Overview
This lab focuses on implementing the K-Nearest Neighbors (KNN) algorithm for classification using Python and Scikit-learn. The goal is to build a model that can classify data points based on their nearest neighbors.

## Dataset
The dataset used in this lab is:
- `KNN_Project_Data.csv`

It contains multiple features and a target column called:
- `TARGET CLASS`

## Steps Performed

1. **Data Loading**
   - Loaded the dataset using pandas.

2. **Exploratory Data Analysis (EDA)**
   - Used visualization tools like seaborn to understand the data.

3. **Data Preprocessing**
   - Applied feature scaling using `StandardScaler`.

4. **Train-Test Split**
   - Split the data into training and testing sets.

5. **Model Training**
   - Used `KNeighborsClassifier` to train the model.

6. **Model Evaluation**
   - Evaluated performance using:
     - Confusion Matrix
     - Classification Report

7. **Choosing Optimal K**
   - Tested multiple K values.
   - Used the error rate to find the best K.

## Results
- The model performance improved after selecting the optimal value of K.
- Better accuracy was achieved compared to the initial model.

## Conclusion
This lab demonstrates how KNN works and highlights the importance of:
- Feature scaling
- Choosing the right K value
- Evaluating model performance properly
