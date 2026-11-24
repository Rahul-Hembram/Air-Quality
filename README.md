# 🌍 Bhagalpur Air Quality Prediction System

An Machine Learning-based Air Quality Prediction System designed to analyze historical air pollution data and explore next-day PM2.5 predictions for Bhagalpur, Bihar.

The project combines data analysis, regression models, model evaluation, feature importance analysis and an interactive Streamlit dashboard to visualize air quality trends and model predictions.

---

## 📌 Project Overview

Air pollution is a growing environmental concern that affects public health and quality of life. Monitoring pollutant concentrations and understanding their patterns can help in analyzing environmental conditions.

This project focuses on analyzing air quality data from Bhagalpur, Bihar, and predicting next-day PM2.5 concentrations using Machine Learning regression models.

The system provides an interactive dashboard where users can explore historical pollution trends, examine model performance, visualize important features and investigate PM2.5 predictions.

---

## 🚀 Project Features

- 📊 Interactive Air Quality Dashboard
- 🌫️ Historical PM2.5 Analysis
- 🤖 Next-Day PM2.5 Prediction
- 📈 Machine Learning Model Comparison
- 🌲 Random Forest Feature Importance
- ⚡ XGBoost Feature Importance
- 📉 Actual vs Predicted Visualization
- 📑 Automated Model Evaluation Reports
- 🔍 Data Validation and Preprocessing

---

## 🖥️ Dashboard Preview

![Bhagalpur Air Quality Dashboard](Screenshot%202026-11-24%20215520.png)

The dashboard provides an overview of air quality data, model-related information and visualizations to help users explore pollution patterns.

---

## 🧠 Machine Learning Models

The project explores multiple regression models for next-day PM2.5 prediction.

| Model | Description |
|---|---|
| Linear Regression | Baseline regression approach for modelling linear relationships between input features and PM2.5 |
| Random Forest Regressor | Ensemble learning model that combines multiple decision trees |
| XGBoost Regressor | Gradient boosting algorithm used for predictive modelling |
| Persistence Baseline | Uses the current day's PM2.5 value as an estimate of the next day's PM2.5 |

The trained models are evaluated and compared using multiple regression metrics to identify their relative performance.

---

## 📊 Model Evaluation

The models are evaluated using the following metrics:

- **MAE (Mean Absolute Error):** Measures the average absolute difference between predicted and actual values.
- **MSE (Mean Squared Error):** Measures the average squared prediction error.
- **RMSE (Root Mean Squared Error):** Represents prediction error in the same unit as the target variable.
- **R² Score:** Measures how well the model explains the variance in the target variable.

### Model Performance

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 27.239 | 28.596 | -75.444 |
| Random Forest | 4.419 | 5.284 | -1.610 |
| XGBoost | 2.743 | 3.337 | -0.041 |

*The metrics above represent the evaluation results available in the project files. The test dataset is small, so these results should be interpreted cautiously.*

---

## 📈 Visualizations

The project generates visualizations to help understand model performance and dataset patterns.

- Model Performance Comparison
- Actual vs Predicted PM2.5 Values
- Random Forest Feature Importance
- XGBoost Feature Importance
- Historical PM2.5 Trends
- Other Pollutant Analysis

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical computation |
| Matplotlib | Data visualization |
| Scikit-learn | Machine learning and model evaluation |
| XGBoost | Gradient boosting model |
| Joblib | Model serialization |
| Streamlit | Interactive dashboard |

---

## 📂 Project Structure

```text
Bhagalpur-Air-Quality-Prediction/
│
├── data/
│   └── bhagalpur_daily_data.csv
│
├── models/
│   ├── linear_regression.joblib
│   ├── random_forest.joblib
│   ├── xgboost.joblib
│   └── best_model.joblib
│
├── outputs/
│   ├── graphs/
│   │   ├── actual_vs_predicted_best_model.png
│   │   ├── model_comparison.png
│   │   ├── random_forest_feature_importance.png
│   │   └── xgboost_feature_importance.png
│   │
│   └── reports/
│       ├── model_metrics.csv
│       ├── baseline_metrics.csv
│       └── project_report.pdf
│
├── src/
│   ├── config.py
│   ├── data_utils.py
│   ├── models.py
│   ├── pipeline.py
│   ├── reporting.py
│   └── validation.py
│
├── app.py
├── main.py
├── requirements.txt
└── README.md
