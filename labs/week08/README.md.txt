# AI Lab 7 – Applicant Data Preprocessing Project

## Project Overview

This project is developed in Python using **Pandas**, **NumPy**, and **Scikit-learn**. The main objective of this project is to perform complete data preprocessing on applicant datasets stored in CSV and JSON formats.

The notebook demonstrates how to:

* Create datasets
* Load CSV and JSON files
* Inspect data
* Merge datasets
* Handle missing values
* Clean inconsistent data
* Create new features
* Normalize numerical columns
* Build a reusable preprocessing function

This project is useful for beginners who want to understand real-world data preprocessing techniques used in Data Science and Machine Learning.

---

# Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Jupyter Notebook

---

# Libraries Used

```python
import pandas as pd
import numpy as np
import json
from sklearn.preprocessing import MinMaxScaler
```

---

# Dataset Information

The project uses two datasets:

## 1. applicants.csv

Contains applicant information:

| Column          | Description         |
| --------------- | ------------------- |
| id              | Applicant ID        |
| name            | Applicant Name      |
| age             | Applicant Age       |
| experience      | Years of Experience |
| expected_salary | Expected Salary     |
| education       | Education Level     |
| city            | Applicant City      |

## 2. applicants_extra.json

Contains additional applicant details:

| Column | Description        |
| ------ | ------------------ |
| id     | Applicant ID       |
| skills | Technical Skills   |
| status | Application Status |

---

# Project Tasks

# Task 1 – Create and Load Dataset

In this task:

* CSV file is created using Python
* JSON file is created using Python
* Both datasets are loaded using Pandas

### Concepts Used

* File Handling
* CSV Handling
* JSON Handling
* Pandas DataFrames

### Code Example

```python
pd.read_csv("applicants.csv")
pd.read_json("applicants_extra.json")
```

---

# Task 2 – Inspect Dataset

The dataset is inspected to understand:

* Head of dataset
* Data types
* Missing values
* Shape of dataset

### Functions Used

```python
head()
dtypes
isnull().sum()
shape
```

### Purpose

This helps identify data quality issues before preprocessing.

---

# Task 3 – Merge Datasets

The CSV and JSON datasets are merged using the `id` column.

### Code Used

```python
df = pd.merge(df_csv, df_json, on="id", how="left")
```

### Purpose

Combining data from multiple sources into a single DataFrame.

---

# Task 4 – Handle Missing Values

Several missing value handling techniques are applied.

## Age Column

Missing ages are replaced with median value.

```python
df["age"] = df["age"].fillna(df["age"].median())
```

## Experience Column

Missing experience values are replaced with 0.

```python
df["experience"] = df["experience"].fillna(0)
```

## Expected Salary Column

* `?` values are replaced with NaN
* Converted to numeric format
* Missing salaries filled using median

```python
df["expected_salary"] = df["expected_salary"].replace("?", np.nan)
```

## Education Column

Missing education values are replaced with `Unknown`.

```python
df["education"] = df["education"].fillna("Unknown")
```

## Name Column

Missing names are replaced with `Anonymous`.

```python
df["name"] = df["name"].fillna("Anonymous")
```

---

# Task 5 – Data Cleaning

City names are cleaned and standardized.

### Operations Performed

* Replace `isl` with `Islamabad`
* Convert all city names to lowercase

### Code

```python
df["city"] = df["city"].replace("isl", "Islamabad")
df["city"] = df["city"].str.lower()
```

### Purpose

Ensures consistency in categorical data.

---

# Task 6 – Feature Engineering

A new column named `experience_level` is created.

### Levels

| Experience | Level  |
| ---------- | ------ |
| 0–1        | Junior |
| 2–5        | Mid    |
| 6+         | Senior |

### Function

```python
def experience_level(exp):
    if exp <= 1:
        return "junior"
    elif exp <= 5:
        return "mid"
    else:
        return "senior"
```

### Purpose

Transforms numerical experience into meaningful categories.

---

# Task 7 – Data Normalization

Numerical columns are normalized using MinMaxScaler.

### Columns Normalized

* age
* experience
* expected_salary

### Code

```python
scaler = MinMaxScaler()
df[cols] = scaler.fit_transform(df[cols])
```

### Purpose

Normalization scales values between 0 and 1.
This improves machine learning model performance.

---

# Task 8 – Reusable Preprocessing Function

A reusable preprocessing function is created.

### Function Name

```python
preprocess_applicants(df)
```

### Purpose

This function automates:

* Missing value handling
* Data cleaning
* Feature engineering
* Normalization

This makes the preprocessing pipeline reusable for future datasets.

---

# Key Concepts Learned

* Data Cleaning
* Data Inspection
* Missing Value Handling
* Feature Engineering
* Data Normalization
* Data Merging
* Pandas Operations
* NumPy Operations
* Machine Learning Preprocessing

---

# Output of Project

After preprocessing:

* Data becomes clean and consistent
* Missing values are handled
* Numerical values are normalized
* New useful features are created
* Dataset becomes ready for Machine Learning models

---

# Advantages of This Project

* Beginner-friendly
* Real-world preprocessing techniques
* Practical implementation of Pandas
* Improves understanding of data pipelines
* Useful for AI and Data Science students

---

# Future Improvements

Possible future enhancements:

* Add data visualization
* Use larger datasets
* Train machine learning models
* Save processed dataset automatically
* Add graphical dashboard

---

# Conclusion

This project demonstrates a complete applicant data preprocessing workflow using Python. It covers essential concepts required in Artificial Intelligence, Data Science, and Machine Learning projects.

By completing this project, students can understand how raw data is transformed into clean, structured, and machine-learning-ready data.

---

# How to Run the Project

## Step 1

Install required libraries:

```bash
pip install pandas numpy scikit-learn
```

## Step 2

Open Jupyter Notebook.

## Step 3

Run all cells one by one.

## Step 4

View the cleaned and processed dataset.

---

# Author

AI Lab 7 Project
Applicant Data Preprocessing System
