# ⚡️ Global Active Power Consumption Prediction

> A Machine Learning Pipeline for Smart Energy Forecasting

---

## 📈 Project Summary

This project aims to build an end-to-end machine learning system to **predict global active power consumption** using time-series data. It involves:

✅ Data understanding & exploration  
✅ Preprocessing and feature engineering  
✅ Regression model development  
✅ Model evaluation and comparison  

---

## 🧠 Problem Statement

With growing energy demand, accurate forecasting of power consumption is essential for:

- Reducing energy waste
- Optimizing energy grid operations
- Power-aware infrastructure planning

**Goal:** Predict `Global_active_power` using regression models based on historical usage and other engineered features.

---

## 📦 Dataset Overview

| Feature | Description |
|--------|-------------|
| Date & Time | Timestamp of power consumption |
| Global_active_power | Target variable (kW) |
| Sub_metering_1/2/3 | Energy usage by different appliances |
| Voltage | Average voltage per minute |
| Global_intensity | Average current per minute |

> 📍 *Optional External Data*: Weather conditions (e.g., temperature, humidity)

---

## 🔍 Exploratory Data Analysis (EDA)

- 📊 Trend & seasonality plots
- 📈 Correlation heatmaps
- 📦 Outlier detection using boxplots
- 📉 Time-series decomposition

---

## 🔧 Data Preprocessing Steps

- ✅ Missing value treatment (interpolation, imputation)
- ⏳ Date/Time parsing into `hour`, `day`, `month`, etc.
- 🧮 Feature creation:
  - Rolling means
  - Peak hours
  - Daily averages
- 📏 Feature scaling with MinMaxScaler / StandardScaler

---

## 🏗 Feature Engineering

- 🎯 Relevant feature selection based on correlation and importance
- 🌦 Weather integration (if available)
- 🔁 Lag features and rolling windows for temporal context

---

## 🤖 Model Building

| Model | Type |
|-------|------|
| 🔹 Linear Regression | Baseline |
| 🌲 Random Forest | Tree-based ensemble |
| 🚀 Gradient Boosting (XGBoost/LightGBM) | Advanced ensemble |
| 🧠 Neural Networks (MLP) | Deep learning approach |

**Hyperparameter tuning** using `GridSearchCV` and `RandomizedSearchCV`.

---

## 🧪 Model Evaluation

| Metric | Purpose |
|--------|---------|
| 🧮 RMSE | Penalizes larger errors |
| 📉 MAE | Average absolute error |
| 📈 R² Score | Variance explained by the model |

📊 **Visualization:** Actual vs Predicted line plots, residual distribution, and error curves.

---

## 🏆 Results Summary

- ✔️ Best model: `Gradient Boosting Regressor` (example)
- 📊 RMSE: 0.192 | MAE: 0.137 | R²: 0.91
- 🔍 Found strong temporal patterns & peak hour influence

---

## 🚀 Future Enhancements

- 📡 Real-time dashboard using Streamlit / Power BI
- ⏱ LSTM-based deep learning for sequence prediction
- 🌦 External weather + holiday/event data fusion

---

## 🗂 Project Structure

```bash
.
├── data/                  # Raw and processed datasets
├── notebooks/             # EDA and modeling notebooks
├── src/                  # Python scripts for modular code
│   ├── preprocessing.py
│   ├── feature_engineering.py
│   ├── model_training.py
├── report/                # Evaluation reports, charts
├── requirements.txt
└── README.md
# House-hold-power-consumption
