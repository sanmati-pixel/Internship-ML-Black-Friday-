# Internship-ML-Black-Friday-
# 🖤🛒 Black Friday Dataset – EDA & Feature Engineering

This project focuses on **exploratory data analysis (EDA)** and **feature engineering** performed on the Black Friday dataset to prepare it for machine learning model training.

---

## 📌 Problem Statement
A retail company **ABC Private Limited** wants to understand **customer purchase behavior**, specifically the **purchase amount**, across different product categories.

The dataset contains:
- Customer demographics (age, gender, marital status, city type, stay in current city)
- Product details (product ID, product categories)
- Total purchase amount from the previous month

🎯 **Objective:**  
Prepare clean, numerical, and machine-learning-ready data that can be used to predict customer purchase amounts and enable **personalized offers**.

---

## 📂 Dataset Overview
- `train.csv`
- High-volume purchase data from the last month
- Mix of **categorical** and **numerical** features

---

## 🔍 Exploratory Data Analysis (EDA)
- Loaded and inspected dataset using `pandas`
- Checked feature distributions and unique values
- Identified categorical variables requiring transformation
- Analyzed age groups, gender distribution, and city categories

---

## 🧹 Data Cleaning & Preprocessing

### 1️⃣ Handling Categorical Features

#### Gender Encoding
- Converted gender from categorical to numerical:
  - `F → 0`
  - `M → 1`

```python
df['Gender'] = df['Gender'].map({'F': 0, 'M': 1})
