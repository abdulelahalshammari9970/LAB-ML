# Lab 2 – Identifying ML Problems, Selecting Open Datasets, and Drawing a Methodology Diagram



---

## Problem Statement

This project aims to build a **binary classification model** that predicts whether an email is **spam** or **not spam (ham)**.  
The dataset contains word frequncy vectors for 5,172 emails. The target variable is the column `Prediction`, where:

- `0` = not spam  
- `1` = spam  

The task is **supervised learning** because labelled examples are provided.

---

## Dataset Description

- **Source:** From kaggle (([https://www.kaggle.com/datasets/balaka18/email-spam-classification-dataset-csv?resource=download](https://www.kaggle.com/datasets/balaka18/email-spam-classification-dataset-csv?resource=download))) 
- **Format:** CSV 
- **Number of instances:** 5,172
- **Number of features:** 3,001 (word frequency counts)
- **Target column:** `Prediction` (binary)


Each row represents one email, and each feature column (from `the` to `dry`) represents the number of times that word appears in the email.

---

## Machine Learning Task

- **Type:** Supervised Learning – Binary Classification  
- **Target variable:** `Prediction`  


---

## Initial Data Inspection (Jupyter Notebook)

The notebook `lab2_spam_inspection.ipynb` perform the following :

1. **Load the dataset** using `pandas.read_csv()`.
2. **Display the shape** – confirms 5,172 rows × 3,002 columns.
3. **Preview the first few rows** – shows word frequencies and the `Prediction` column.
4. **Check column names and data types** – all feature columns are integers (`int64`), the `Email No.` column is object , and `Prediction` is integer.



---

## Methodology Diagram

The overall machine learning workflow is illustrated in `Diagram.png` .  
It includes the following stages:

1. **Dataset collection**  
2. **Data preprocessing**  
3. **Model selection** 
4. **Model training & validation**   
5. **Model evaluation**  
6. **Final model**

![Methodology Diagram](methodology_diagram.png)

---
