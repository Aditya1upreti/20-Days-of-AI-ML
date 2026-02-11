# 🚢 Titanic Survival Prediction

## 📌 Problem Statement
Predict whether a passenger survived the Titanic disaster using machine learning classification models.

This project focuses on:
- Data preprocessing
- Feature engineering
- Model comparison
- Hyperparameter tuning
- Performance evaluation

---

## 📊 Dataset
- Kaggle Titanic Dataset  
- 891 training samples  
- 418 test samples  

Target Variable:
- `Survived` (0 = No, 1 = Yes)

---

## 🔎 Exploratory Data Analysis

Key Observations:
- Female passengers had significantly higher survival rates.
- Higher passenger class (Pclass 1) had better survival probability.
- Age and Fare distributions impacted survival outcomes.
- Cabin had too many missing values and was dropped.

---

## 🧹 Data Cleaning & Preprocessing

### Handling Missing Values
- **Age** → Filled using median grouped by `Pclass`
- **Embarked** → Filled using mode
- **Fare (Test set)** → Filled using median

### Columns Dropped
- PassengerId
- Name
- Ticket
- Cabin

### Encoding
- Sex → Female: 0, Male: 1
- Embarked → S:0, C:1, Q:2

---

## 🤖 Models Implemented

### 1️⃣ Random Forest
Initial Accuracy: **80.45%**

After GridSearch Tuning:
- Best Accuracy: **82.72%**
- Best Parameters:
  - max_depth = 11
  - max_features = sqrt
  - min_samples_split = 4
  - n_estimators = 100

---

### 2️⃣ Gradient Boosting
Initial Accuracy: **82.68%**

After GridSearch Tuning:
- Best Accuracy: **83.85%**
- Best Parameters:
  - learning_rate = 0.07
  - max_depth = 3
  - max_features = sqrt
  - n_estimators = 100
  - subsample = 1.0

---

## 🧠 Feature Importance

Top Influential Features:
1. Sex (Most important)
2. Pclass
3. Fare
4. Age

This insight guided further feature engineering.

---

## 🚀 Feature Engineering

Created new features:
- `IsBoy` → Male under 14 years
- `FamilySize` → SibSp + Parch + 1
- `IsAlone` → Whether passenger was alone

After retraining with engineered features:

**Final Accuracy: 83.73%**

---

## 📁 Final Output
Generated Kaggle submission file:

---

## 📈 Final Model Summary
Best Model: **Gradient Boosting Classifier**

Achieved:
- ~84% Cross-Validation Accuracy
- Improved performance through feature engineering and hyperparameter tuning

---

## 🎯 Key Learnings

- Importance of feature engineering in structured data
- GridSearchCV for systematic hyperparameter tuning
- Tree-based models handle non-linear relationships effectively
- Domain-driven features improve predictive power

---

## 🛠️ Tech Stack
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib (if used)
- GridSearchCV

---

## 📌 Future Improvements
- Use XGBoost / LightGBM
- Try stacking ensemble
- Perform cross-validation with StratifiedKFold
- Add SHAP value interpretation
