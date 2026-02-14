# 🏠 House Price Prediction – Advanced Regression Techniques  
**Day 3 | 20 Days of AI/ML Challenge**

## 📌 Project Overview
This project is based on the Kaggle competition **House Prices – Advanced Regression Techniques**, where the task is to predict the final sale price of residential homes in Ames, Iowa using 79 explanatory variables.

Instead of relying on simple Linear Regression, this project focuses on **regularized regression techniques (Ridge and Lasso)** to handle:
- multicollinearity
- high-dimensional feature space
- overfitting after extensive encoding

The main objective was not just to improve the score, but to **understand why and when regularization works**.

---

## 📂 Dataset
- **train.csv** – Training data (1460 samples) with features and target variable `SalePrice`
- **test.csv** – Test data (1459 samples) used for final predictions
- **data_description.txt** – Detailed explanation of all features and missing value logic

---

## 🔍 Methodology

### 1️⃣ Target Variable Transformation
- `SalePrice` was heavily right-skewed.
- Applied **log transformation (`log1p`)** to normalize the distribution.
- This helps the model learn relative price differences instead of absolute values.

---

### 2️⃣ Data Cleaning
- Converted numerical categorical features (e.g. `MSSubClass`) to strings to avoid treating them as continuous values.
- Numerical missing values were filled using **median imputation** to reduce sensitivity to outliers.
- Categorical features where missing values imply absence (e.g. `GarageType`, `PoolQC`) were replaced with `"None"` based on the data dictionary.

---

### 3️⃣ Feature Engineering
Created meaningful composite features to reduce noise and improve learning:

- **TotalSF** = Total basement + 1st floor + 2nd floor area  
- **Total_Bathrooms** = Full baths + 0.5 × Half baths  
- **HouseAge** = Age of the house relative to 2010  
- **RemodAge** = Years since last renovation  

These features capture real-world housing insights more effectively than raw variables.

---

### 4️⃣ Feature Encoding
- **Ordinal Encoding** was applied to ranked categorical features (e.g. quality ratings).
- **One-Hot Encoding** was used for nominal features, expanding the dataset from ~80 to ~250 features.
- Training and test sets were aligned to ensure consistent feature columns.

---

### 5️⃣ Modeling Approach
Two regularized linear models were trained and evaluated:

- **Ridge Regression (L2)**  
  - Penalizes large coefficients
  - Helps correlated features share influence

- **Lasso Regression (L1)**  
  - Performs feature selection by shrinking irrelevant coefficients to zero
  - Useful in high-dimensional spaces

Hyperparameters were tuned using **heuristic search**, followed by validation checks.

---

## 📊 Results
Models were evaluated using **5-fold cross-validation** with **RMSE** on the log-transformed target.

| Model  | CV RMSE |
|-------|---------|
| Ridge | 0.1423  |
| Lasso | 0.1426  |

Ridge Regression performed slightly better, likely due to its ability to distribute weights among correlated features, while Lasso aggressively eliminated less informative features.


## 🧠 Key Learnings
- Regularization is essential when working with many correlated features
- Lasso helps identify important predictors, while Ridge stabilizes learning
- Understanding *why* a model works matters more than blindly optimizing scores
- Using AI tools for implementation is fine when the reasoning is your own

---

## 🚀 Next Steps
- Experiment with ElasticNet
- Try feature interaction terms
- Compare results with tree-based models (XGBoost, LightGBM)

---

**Part of my 20 Days of AI/ML Challenge — building strong foundations before moving to complex models.**
