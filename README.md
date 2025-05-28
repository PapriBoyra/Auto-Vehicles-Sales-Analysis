# 🚗 Car Price Prediction - Multiple Linear Regression

## 📘 Overview

This project involves building a **Multiple Linear Regression** model to predict car prices based on various car attributes. The problem is inspired by a real-world business case from **Geely Auto**, a Chinese automobile company planning to enter the U.S. market.

The goal is to identify significant variables that affect car pricing and to evaluate how well these variables can predict the price of a car. The model will help stakeholders make data-driven decisions around product design, pricing strategies, and market positioning.

---

## 🏁 Business Problem

**Geely Auto** aims to understand the pricing dynamics in the American car market. They have collected a dataset with various car features and now need:

- Identification of the most significant variables affecting car price
- A statistical model that can accurately predict car prices
- Insights to align their business and design strategies for market entry

---

## 📊 Data Summary

- The dataset includes variables like `car width`, `engine size`, `horsepower`, `fuel type`, and more.
- A special variable, `CarName`, contains both the company and model name. **Only the company name** is considered for modeling.
- The dataset has been cleaned and transformed to be suitable for regression analysis.

---

## 🛠️ Tools & Technologies Used

- **Python**
- **Pandas**, **NumPy** – Data handling
- **Matplotlib**, **Seaborn** – Visualization
- **scikit-learn**, **statsmodels** – Model building & evaluation
- **Jupyter Notebook**

---

## 🧹 Data Cleaning & Preparation

- Extracted **car company name** from `CarName`
- Removed or corrected inconsistencies (e.g., typos in brand names)
- Handled missing values and outliers
- Converted categorical variables using **dummy encoding**
- Derived new metrics where applicable
- Ensured dataset was in clean, model-ready format

---

## 🧠 Model Building & Evaluation

- Performed **EDA** to understand feature relationships
- Used **OLS (Ordinary Least Squares)** and **RFE (Recursive Feature Elimination)** for feature selection
- Built a final **multiple linear regression model**
- Evaluated performance using:
  - **R-squared**
  - **Adjusted R-squared**
  - **Residual plots**
  - **R-squared on test set** using:
    ```python
    from sklearn.metrics import r2_score
    r2_score(y_test, y_pred)
    ```

---

## 📈 Key Findings

- Variables like **engine size**, **curb weight**, and **horsepower** are highly significant
- The final model shows good generalization on the test data
- Brand/company name plays a role in car pricing due to perceived quality

---
