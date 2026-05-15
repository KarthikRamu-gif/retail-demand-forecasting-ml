# Retail Demand Forecasting using Machine Learning

## Project Overview

This project focuses on short-term retail demand forecasting using Machine Learning techniques on the M5 Forecasting Dataset.

The study specifically analyzes the **CA_1 Walmart Store** and **FOODS product category** to predict **1-day ahead retail demand** using machine learning models.

The project compares the forecasting performance of:

- Random Forest
- XGBoost
- Optimized XGBoost

The objective is to improve retail demand prediction to support inventory planning and operational decision-making.

---

## Dataset

Dataset used:

**M5 Forecasting Accuracy Dataset (Kaggle)**

https://www.kaggle.com/competitions/m5-forecasting-accuracy/data

Dataset files used:

- `sales_train_validation.csv`
- `calendar.csv`
- `sell_prices.csv`

---

## Project Structure

```text
├── docs/
│   └── Dissertation report and project documentation
│
├── notebooks/
│   └── google collab for preprocessing, EDA and modelling
│
├── results/
│   └── Model outputs, plots and evaluation results
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Methods Used

### Data Preprocessing
- Data filtering (CA_1 + FOODS)
- Wide-to-long transformation
- Missing value handling
- Calendar merging

### Feature Engineering
- Lag features (`lag_7`)
- Rolling statistics (`rolling_mean_7`)
- Temporal variables
- SNAP indicators
- Event features

### Machine Learning Models
- Random Forest
- XGBoost
- Optimized XGBoost

---

## Model Evaluation Metrics

The following evaluation metrics were used:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Coefficient of Determination (R²)

---

## Key Results

| Model | MAE | RMSE | R² |
|--------|------|------|------|
| Random Forest | 1.3079 | 2.4034 | 0.6827 |
| XGBoost | 1.3010 | 2.3910 | 0.6860 |
| Optimized XGBoost | 1.3010 | 2.3899 | 0.6863 |

The Optimized XGBoost model achieved the strongest forecasting performance.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

---

## Author

Karthik Ramu

MSc IT for Business Data Analytics
