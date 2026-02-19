# 📊 Customer Churn Prediction (Kaggle Challenge)

This repository contains my solution to the **Customer Churn Prediction** Kaggle competition, where the goal is to predict whether a customer will churn using real-world tabular data.

The project explores both **supervised learning** and **unsupervised clustering** techniques, and demonstrates how combining them can significantly improve model performance.

---

## 🚀 Project Overview

Customer churn prediction is a critical business problem for subscription-based companies.  
In this project, I experimented with:

- Traditional supervised ML models
- Feature engineering and preprocessing
- Unsupervised clustering to enhance predictive performance
- Model tuning and performance comparison on Kaggle’s public leaderboard

---

## 📁 Repository Structure

├── Customer.ipynb # Supervised learning approach
├── Customer_Unsuper.ipynb # Unsupervised clustering + feature enrichment
├── submission.csv # Baseline Kaggle submission
├── submission_tuned_clustered.csv # Improved submission using clustering
└── README.md


---

## 🧠 Approach

### 1️⃣ Supervised Learning (Baseline)
- Data cleaning and preprocessing
- Encoding categorical variables
- Feature scaling
- Model training (binary classification)
- Generated `submission.csv`

**Public Score:** `0.81520`

---

### 2️⃣ Unsupervised Learning + Tuning (Improved)
- Applied clustering (customer segmentation)
- Used cluster labels as additional features
- Tuned model hyperparameters
- Improved feature representation
- Generated `submission_tuned_clustered.csv`

**Public Score:** **`0.93818` 🚀**

---

## 📊 Kaggle Results

| Submission File                     | Public Score |
|------------------------------------|--------------|
| `submission.csv`                   | 0.81520      |
| `submission_tuned_clustered.csv`   | **0.93818**  |

This demonstrates how **combining unsupervised learning with supervised models** can significantly boost performance.

---

## 🛠️ Tools & Technologies

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Jupyter Notebook
- Kaggle Notebooks & Submissions

---

## 📌 Key Learnings

- Clustering can reveal hidden customer segments
- Feature enrichment often matters more than model complexity
- Iterative experimentation is key in real-world ML problems
- Leaderboard feedback helps validate improvements

---

## 📎 Competition Link

🔗 Kaggle Competition:  
**Predicting Customer Churn – A Real-World Binary Classification Challenge**

---

## ✨ Future Improvements

- Advanced ensemble models
- Cross-validation based tuning
- Feature importance analysis
- Explainability using SHAP / LIME

---

## 👤 Author

**Aditya Raj Upreti**  
B.Tech CSE | Machine Learning Enthusiast  
Building projects through a structured **20 Days of AI/ML Challenge**

---

⭐ If you found this useful, feel free to star the repository!
