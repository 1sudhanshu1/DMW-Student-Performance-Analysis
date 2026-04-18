# 📊 Student Performance Analysis (DMW Project)

## 📌 Project Overview

This project focuses on analyzing student performance using Data Mining and Data Warehousing techniques. The objective is to identify key factors affecting student scores and build predictive models.

The system is designed to be **robust**, meaning it can handle changes in data such as missing values, added records, or modifications without breaking.

---

## 🎯 Objectives

* Analyze student performance data
* Identify patterns and relationships between variables
* Apply machine learning models for prediction
* Design Star Schema and Snowflake Schema
* Build a system that adapts to changing datasets

---

## 📂 Dataset

* Dataset: *Students Performance in Exams*
* Source: Kaggle
* Features include:

  * Gender
  * Parental level of education
  * Lunch type
  * Test preparation course
  * Math, Reading, Writing scores

---

## ⚙️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab

---

## 🧠 Methodology (Step-by-Step Algorithm)

### Step 1: Data Collection

* Load dataset from CSV file into the system

### Step 2: Data Understanding

* Analyze dataset structure using:

  * shape
  * columns
  * info()
  * describe()

### Step 3: Data Preprocessing

* Handle missing values:

  * Numerical → median
  * Categorical → mode
* Remove duplicate records
* Ensure data consistency

### Step 4: Feature Engineering

* Create `average_score` from subject scores
* Create `performance` category dynamically based on mean score

### Step 5: Data Analysis

* Use groupby() for category-based analysis
* Use correlation to find relationships
* Identify patterns in performance

### Step 6: Data Visualization

* Histogram → distribution
* Bar chart → comparison
* Heatmap → correlation
* Scatter plot → relationships
* Boxplot → outlier detection

### Step 7: Outlier Handling

* Apply IQR method to remove extreme values

### Step 8: Model Building

* Split data into training and testing sets
* Apply:

  * Linear Regression
  * Decision Tree Regressor

### Step 9: Model Evaluation

* Evaluate using Mean Squared Error (MSE)
* Compare model performance

### Step 10: Clustering (Optional Enhancement)

* Apply K-Means to group students into clusters

### Step 11: Data Warehouse Design

* Star Schema:

  * Fact Table → Scores
  * Dimension Tables → Student, Preparation, Time
* Snowflake Schema:

  * Normalize dimension tables

### Step 12: Robustness Implementation

* Dynamic file loading
* No hardcoded values
* Automatic handling of missing data
* Adaptive thresholds based on dataset

---

## 📊 Key Insights

* Strong positive correlation between subject scores
* Students with test preparation perform better
* Most students fall in the average performance range
* Parental education influences student outcomes
* Data preprocessing improves model accuracy

---

## 🏗️ Data Warehouse Design

### ⭐ Star Schema

* Central Fact Table: Student Scores
* Connected Dimension Tables:

  * Student Information
  * Test Preparation
  * Time

### ❄️ Snowflake Schema

* Dimension tables are further normalized into smaller related tables
* Reduces redundancy and improves structure

---

## 📈 Results

* Linear Regression provides baseline predictions
* Decision Tree captures complex relationships better
* Models achieve reasonable accuracy

---

## 🔒 Robustness Features

* Handles missing values dynamically
* Works with modified datasets
* Handles outliers using statistical methods
* No dependency on fixed data format

---

## 👨‍💻 Author

Sudhanshu Nikam
PRN: 20240802174

---

## 📎 How to Run

1. Open the notebook in Google Colab
2. Upload the dataset
3. Run all cells step by step
4. View analysis, graphs, and results
