# Student Performance Analysis and Reporting System

## Project Overview

The **Student Performance Analysis and Reporting System** is a Python-based data analysis project developed using **Pandas** and **NumPy** libraries.

This project analyzes student data such as marks, attendance, and department information. It also performs data cleaning, grading, filtering, sorting, and generates a final processed report.

---

# Objectives

The main objectives of this project are:

* Manage student records using DataFrames
* Handle missing values in the dataset
* Perform numerical analysis using NumPy
* Generate grades automatically
* Identify passed and failed students
* Create department-wise summaries
* Export processed data into a CSV file

---

# Technologies Used

* Python
* Pandas
* NumPy

---

# Features

## 1. Data Creation

Student data is stored and converted into a Pandas DataFrame.

## 2. Missing Value Handling

Missing values are handled using:

* Mean replacement for marks
* Median replacement for attendance

## 3. NumPy Array Operations

The project performs:

* Array conversion
* Percentage calculation
* Average marks calculation
* Boolean indexing

## 4. Feature Engineering

New columns are added:

* Passed
* Percentage
* Grade

## 5. Grade Generation

Grades are assigned automatically using conditional logic.

| Marks Range  | Grade |
| ------------ | ----- |
| 85 and above | A     |
| 70 - 84      | B     |
| 50 - 69      | C     |
| Below 50     | Fail  |

---

## 6. Data Filtering

The project filters:

* High scoring students
* Students meeting multiple conditions

---

## 7. Data Sorting

Student records are sorted based on marks in descending order.

---

## 8. loc and iloc Operations

Specific rows and columns are accessed using:

* `loc`
* `iloc`

---

## 9. GroupBy and Aggregation

Department-wise average marks and attendance are calculated.

---

## 10. CSV File Export

The final processed dataset is saved as:

```text
processed_students.csv
```

---

# Concepts Used

* Pandas DataFrame
* Data Cleaning
* Missing Value Handling
* NumPy Arrays
* Boolean Indexing
* Conditional Statements
* Feature Engineering
* Data Filtering
* Data Sorting
* GroupBy Aggregation
* File Handling

---

# How to Run the Project

## Step 1: Install Python

Make sure Python is installed on your system.

---

## Step 2: Install Required Libraries

```bash
pip install pandas numpy
```

---

## Step 3: Run the Program

```bash
python project.py
```

---

# Output

The program successfully:

* Cleans the dataset
* Analyzes student performance
* Generates grades
* Creates summaries
* Saves the final CSV report

---

# Future Improvements

The project can be extended by adding:

* Data visualization (graphs/charts)
* Database integration
* Machine learning prediction models
* Student ranking system
* GUI-based application

---

# Learning Outcomes

Through this project, the following concepts were learned:

* Data analysis using Python
* Data cleaning techniques
* NumPy operations
* Pandas DataFrame handling
* Feature engineering
* Data filtering and sorting
* Report generation

---

# Project Name

## Student Performance Analysis and Reporting System
