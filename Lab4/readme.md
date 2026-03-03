## Lab4 Overview

This lab focuses on Data Quality Assessment and Data Preprocessing using the Chocolate Sales dataset.
The main objective is to identify data quality issues, clean the dataset, and apply preprocessing techniques that prepare the data for machine learning models.
Data preprocessing is an essential step in the machine learning pipeline because raw datasets often contain missing values, inconsistent data, and outliers that can negatively affect model performance.

---

## Dataset Description

The dataset used in this lab is Chocolate Sales Dataset.
It contains sales transaction information including:
Sales Person – The person responsible for the sale
Country – Country where the sale occurred
Product – Chocolate product sold
Date – Date of the transaction
Amount – Total sales value
Boxes Shipped – Number of chocolate boxes shipped

This dataset is used to demonstrate common data cleaning and preprocessing techniques.

---

## Analysis Steps

1- Data Loading and Initial Inspection
2- Data Quality Assessment
3- Handling Missing Values
4- Median Imputation
5- Outlier Detection using IQR
6- Data Normalization (Min-Max Scaling)
7- Data Standardization (Z-Score)
8- Principal Component Analysis (PCA)
9- PCA Visualization

---

## Preprocessing Techniques Used

Missing Value Handling

Missing values were handled using Median Imputation, which replaces missing values with the median of the column. This method is more robust to outliers compared to mean imputation.

Outlier Detection
Outliers were detected using the Interquartile Range (IQR) method to identify extreme values that may distort analysis.

Data Normalization
Numerical features were scaled using Min-Max Normalization, which rescales values between 0 and 1.

Dimensionality Reduction
Principal Component Analysis (PCA) was applied to reduce dimensionality and visualize the dataset in a lower-dimensional space while preserving most of the information.

---

## Requirements

Python 3.x

Libraries used in this lab:
pandas
numpy
matplotlib
scikit-learn
