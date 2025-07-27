# 🚦 ETA Prediction Using Machine Learning

This project focuses on **predicting the Estimated Time of Arrival (ETA)** for vehicles passing through various roads in Iran using machine learning models. The dataset contains records of actual arrival times (ATA), geographic coordinates, user IDs, city names, timestamps, and road types.

The goal is to accurately predict the ETA using this real-world traffic data, reducing the gap between predicted and actual arrival times. The problem is formulated as a **regression task**, and three different ML models are applied:

- **Linear Regression**
- **Random Forest**
- **Gradient Boosting**

---

## 📊 Dataset Overview

The dataset includes:
- Road types (`way_type`)
- Entry and exit times (`ETA`, `ATA`)
- User behavior and group
- Geographic data (`longitude`, `latitude`, `city`)
- Time-based features (`hour`, `timestamp`)

---

## 🛠️ Preprocessing Steps

- Loaded CSV files and combined train/test sets
- Removed outliers using **Z-score**
- Converted timestamps to extract `hour`
- Mapped geographic coordinates using Google Maps
- Cleaned and transformed features for modeling

---

## 🤖 Machine Learning Models

Three models were trained and evaluated:

1. **Linear Regression**
2. **Random Forest Regressor**
3. **Gradient Boosting Regressor**

---

## 📈 Evaluation Metrics

The models were evaluated using:

- `MAE` - Mean Absolute Error
- `MSE` - Mean Squared Error
- `MAPE` - Mean Absolute Percentage Error

---

## ✅ Results

- The **Linear Regression model** performed the best overall.
- It provided the **lowest error** and was closest to actual ATA values.
- Gradient Boosting and Random Forest also performed well but had slightly higher error margins.

---

## 📌 Key Insights

- The features `city` and `hour` had the strongest impact on model performance.
- Models struggled more with road types that had fewer data points.
- There's a **linear correlation** between `Length` and `ATA` for many road types.

