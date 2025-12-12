# 🛍️ Customer Segmentation with K-Means

[![Python](https://img.shields.io/badge/python-3.x-blue)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

---

## 📌 Description

This project implements a **K-Means clustering model** to automatically segment a customer database into homogeneous groups.  
The goal: identify distinct profiles to **better understand customers**, personalize offers, and optimize marketing campaigns.

---

## 🎯 Objectives

* Create an **actionable and coherent** segmentation.
* Identify groups based on: age, income, spending score, and purchasing behavior.
* Provide a foundation for: targeted marketing campaigns, customer retention, and personalized offers.

---

## 🗂️ Data Used

| Variable                 | Description                             |
| ------------------------ | --------------------------------------- |
| `Gender`                 | Customer gender                          |
| `Age`                    | Customer age                             |
| `Annual Income (k$)`     | Annual income in k$                       |
| `Spending Score (1-100)` | Spending score / purchasing behavior    |

> **Note**: Complete dataset, no missing values or duplicates.

---

## 🔍 Exploratory Data Analysis (EDA)

* Variable distributions and identification of outliers
* Correlations between age, income, and spending score
* Scatter matrix and pairplot to visualize natural groupings
* Observation: Age, Income, and Spending Score show bimodal trends → perfect for K-Means

---

## ⚙️ Data Preparation

* Encoding `Gender` into numerical variables (One-Hot)
* Standardization using `StandardScaler`
* Creation of the final dataset for clustering

---

## 🧩 K-Means Clustering

* **Methods to determine the number of clusters**:

  * Elbow Method
  * Silhouette Score
  * Yellowbrick visualizations
* **Optimal number of clusters**: `k = 3`

### Cluster Profiles

| Cluster | Age        | Income   | Spending Score | Profile                                             |
| ------- | ---------- | -------- | --------------- | -------------------------------------------------- |
| 0       | 20-40 yrs  | 30-70 k$ | High
