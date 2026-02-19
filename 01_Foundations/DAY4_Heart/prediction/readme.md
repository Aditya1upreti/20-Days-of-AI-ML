Heart Disease Prediction (ML Classification)
📌 Overview

This project focuses on predicting heart disease using machine learning classification models.
The notebook covers data preprocessing, feature engineering, model training, and ensemble-based prediction generation.

🔍 Notebook Structure
1. Data Preprocessing

Loading the dataset

Handling missing values

Encoding categorical features

Preparing data for model training

2. Feature Engineering

Basic feature transformations

Advanced feature engineering to improve model performance

3. Model Training

Multiple classification models are trained and evaluated, including:

Logistic Regression

Random Forest

XGBoost

CatBoost

Each model is trained on the processed dataset and used to generate predictions.

4. Ensembling

Predictions from different models are combined

Ensemble strategy is used to improve robustness and overall performance

Multiple prediction files are generated for comparison

📁 Files
├── heart_competiton.ipynb
├── ensemble_submission.csv
├── optimized_ensemble_submission.csv
├── final_submission.csv
└── README.md

📊 Output

Individual model predictions

Ensemble-based predictions

Optimized final prediction file in CSV format


🛠️ Tools & Libraries
Python
NumPy
Pandas
Scikit-learn
XGBoost