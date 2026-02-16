# ❤️ Heart Disease Prediction using Machine Learning  
**Day 4 | 20 Days of AI/ML Challenge**

## 📌 Project Overview
This project focuses on predicting the presence of heart disease in patients using supervised machine learning techniques. The goal is to build an interpretable and reliable classification model using clinical and lifestyle-related health indicators.

This project emphasizes **end-to-end ML workflow**: data understanding, preprocessing, model training, evaluation, and interpretation.

---

## 📂 Dataset
The dataset contains patient health records with features such as:
- Age
- Sex
- Chest pain type
- Resting blood pressure
- Cholesterol levels
- Fasting blood sugar
- ECG results
- Maximum heart rate
- Exercise-induced angina

**Target Variable:**
- `target` → 1 (Heart Disease Present), 0 (No Heart Disease)

---

## 🔍 Methodology

### 1️⃣ Exploratory Data Analysis (EDA)
- Checked dataset shape, data types, and class distribution
- Identified potential correlations between features and target variable
- Ensured no major class imbalance issues

---

### 2️⃣ Data Preprocessing
- Handled categorical features using encoding techniques
- Scaled numerical features where required to ensure fair model learning
- Split the dataset into training and testing sets

---

### 3️⃣ Model Building
Trained and evaluated multiple classification models to compare performance:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Decision Tree (if applicable)

---

### 4️⃣ Model Evaluation
Models were evaluated using:
- Accuracy Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)

This ensured performance was assessed beyond accuracy alone, especially for medical prediction tasks.

---

## 📊 Results
- Logistic Regression showed strong baseline performance and interpretability
- Distance-based models benefited from feature scaling
- Model comparison helped identify trade-offs between simplicity and performance


---

## 🧠 Key Learnings
- Classification problems require different evaluation metrics than regression
- Feature scaling significantly impacts distance-based models
- Simpler models like Logistic Regression can perform competitively
- Understanding false positives vs false negatives is critical in healthcare ML problems

---

## 🚀 Future Improvements
- Hyperparameter tuning using GridSearchCV
- ROC-AUC curve analysis
- Feature importance visualization
- Trying ensemble models (Random Forest, Gradient Boosting)

---

**Part of my 20 Days of AI/ML Challenge — transitioning from regression to classification while strengthening ML fundamentals.**
