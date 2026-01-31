# 🏡 Boston Housing Price Prediction

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview
This project focuses on predicting housing prices in Boston using advanced **Machine Learning** techniques. The goal was to build a model that outperforms the standard Linear Regression baseline by effectively handling skewed data and non-linear relationships.

## 🎯 Key Results
| Model | R² Score | RMSE |
| :--- | :--- | :--- |
| **Polynomial Ridge Regression** | **83.3%** | **4.32** |
| Standard Linear Regression | ~69% | 4.77 |

> **Achievement:** Improved model accuracy by **~14%** using Log Transformation and Polynomial Features.

## 🛠️ Technologies Used
* **Python**: Data Analysis & Modeling.
* **Pandas & NumPy**: Data Manipulation.
* **Plotly**: Exploratory Data Analysis (EDA).
* **Scikit-Learn**: Machine Learning (Linear Regression, Ridge, Polynomial Features).

## 📊 Key Steps & Methodology

### 1. Exploratory Data Analysis (EDA)
* Analyzed the distribution of all 14 features.
* identified that `LSTAT` (Lower Status Population) has a non-linear relationship with price.
* Detected heavy skewness in features like `CRIM` and `DIS`.

### 2. Data Preprocessing
* **Imputation:** Used `Median` for skewed features and `Mean` for normal features to handle missing values.
* **Log Transformation:** Applied `np.log1p` to highly skewed features (`CRIM`, `LSTAT`, `DIS`) to improve linearity.

### 3. Model Building
* Started with a **Linear Regression** baseline.
* Upgraded to **Polynomial Regression (Degree 2)** to capture curves in data.
* Finalized with **Ridge Regularization** to prevent overfitting and handle multicollinearity.

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/Boston-Housing-Price-Prediction.git](https://github.com/YOUR_USERNAME/Boston-Housing-Price-Prediction.git)
