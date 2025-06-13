# 🌦️ Australian Rainfall Prediction

This project focuses on predicting whether it will rain **tomorrow** in Australia based on historical weather data using supervised machine learning models. The goal is to support decision-making for agriculture, logistics, and weather-dependent activities.

---

## 📂 Dataset Description

- **Source**: Australian Government Bureau of Meteorology  
- **Kaggle Link**: [Weather Dataset - Rattle Package](https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package)
- **Duration**: 2008 to 2017  
- **Locations**: Multiple Australian weather stations  
- **Target Variable**: `RainTomorrow` — whether it will rain the next day (`Yes` or `No`)

---

## 📋 Key Features

- `Date` — used to extract **Season**
- `Temperature`, `Rainfall`, `Wind`, `Humidity`, `Pressure` — various weather measurements
- `RainToday`, `RainTomorrow` — binary indicators for rain

---

## 🧹 Data Preprocessing & Feature Engineering

- Handled missing values using **SimpleImputer** for both numerical and categorical data.
- Encoded categorical features using **OrdinalEncoder**.
- Extracted a new feature: **Season** from the `Date` column.
- Used **ColumnTransformer** for unified preprocessing of numerical and categorical columns.

---

## 🧠 Machine Learning Models

Two classification pipelines were built using:

- **Random Forest Classifier**
- **XGBoost Classifier**

Each model was wrapped in a `Pipeline` with preprocessing steps.

---

## 📊 Evaluation Metrics

- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **Confusion Matrix**

---

## ✅ Results

| Model         | Accuracy | Precision | F1 Score |
|---------------|----------|-----------|----------|
| Random Forest | 86%      | Moderate  | Moderate |
| XGBoost       | **87%**  | ✅ High   | ✅ High  |

> 🏆 **Best Model**: XGBoost Classifier with 87% accuracy and solid precision/F1-score.

---

## 📈 Visualizations

- Correlation Heatmap for feature analysis
- Confusion Matrix
- Seasonal Rain Distribution
- Bar plots for categorical feature impact

---
