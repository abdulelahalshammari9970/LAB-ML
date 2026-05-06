# Support Vector Machines - Iris Dataset

## Overview
This project applies Support Vector Machine (SVM) classification on the famous Iris flower dataset.
The goal is to classify iris flowers into three species based on their sepal and petal measurements.

## Dataset
- **Source:** Seaborn built-in dataset (`sns.load_dataset('iris')`)
- **Samples:** 150 flowers (50 per species)
- **Features:** sepal length, sepal width, petal length, petal width (all in cm)
- **Target:** species (setosa, versicolor, virginica)

## Project Steps
1. **Exploratory Data Analysis** — Pairplot and KDE plot to visualize the data
2. **Train/Test Split** — 70% training, 30% testing
3. **Model Training** — SVC classifier from scikit-learn
4. **Model Evaluation** — Confusion matrix and classification report
5. **Hyperparameter Tuning** — GridSearchCV to find best C and gamma values

## Requirements
- Python 3.x
- pandas, numpy, matplotlib, seaborn, scikit-learn

## Results
The SVM model achieved ~98% accuracy on the test set.
GridSearchCV confirmed the default parameters were already near-optimal for this dataset.
