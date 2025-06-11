# 🏠 California Housing Price Prediction with XGBoost

This project focuses on predicting housing prices in California using the powerful **XGBoost Regressor** algorithm. We utilize the `California Housing Dataset` available in `scikit-learn`, and apply both a baseline model and an optimized model using **GridSearchCV** for hyperparameter tuning.

---

## 📊 Dataset

We use the built-in `fetch_california_housing()` dataset from `scikit-learn`, which includes data about housing in California districts. The target variable is:

- `MedHouseVal`: Median house value (in hundreds of thousands)

**Features include:**
- Median income
- Average number of rooms
- Population
- Latitude and longitude

---

## 🔧 Technologies Used

- Python
- Scikit-learn
- XGBoost
- GridSearchCV
- Matplotlib & Seaborn (for visualization)

---

## 🚀 Project Workflow

### 1️⃣ Baseline XGBoost Model

We trained a basic XGBoost Regressor using default parameters.

**Results on Test Set:**
- **Mean Squared Error (MSE):** `0.26`
- **R² Score:** `0.80`

---

### 2️⃣ Optimized XGBoost Model with GridSearchCV

We performed hyperparameter tuning with `GridSearchCV` using the following search space:

`
param_grid = {
    'n_estimators': [50, 100],
    'learning_rate': [0.01, 0.1],
    'max_depth': [3,4, 5],
}
`
**Results on Test Set:**
- **Mean Squared Error (MSE):** `0.2436`
- **R² Score:** `0.8141`
