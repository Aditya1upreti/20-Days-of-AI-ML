👇

🏪 Rossmann Store Sales Forecasting

Forecast daily sales for Rossmann stores using historical sales, promotion, and competitor data.

🔗 Competition: Rossmann Store Sales (Kaggle)
📊 Model Score:

Public Score: 0.12104

Private Score: 0.13800

Submission File: submission.csv

Submitted by: Aditya Raj Upreti

📌 Problem Statement

Rossmann operates over 3,000 drug stores across Europe.
Store managers need accurate daily sales forecasts to optimize inventory, promotions, staffing, and logistics.

The goal of this project is to predict daily sales for each store using:

Store information

Promotion data

Competitor data

Historical sales records

📂 Project Structure
📦 Rossmann-Store-Sales
 ┣ 📜 rosemann.ipynb
 ┣ 📜 submission.csv
 ┣ 📜 README.md
 📊 Dataset Description

The dataset contains:

Store – Store ID

DayOfWeek – Day of the week

Date – Date of sales

Sales – Target variable

Customers – Number of customers

Open – Whether store was open

Promo – Promotion status

StateHoliday – Holiday indicator

SchoolHoliday – School holiday indicator

StoreType – Type of store

Assortment – Assortment level

CompetitionDistance – Distance to nearest competitor

Promo2 – Ongoing promotion flag

🔎 Approach
1️⃣ Data Preprocessing

Handled missing values

Converted date into useful time-based features (Year, Month, Week, etc.)

Encoded categorical variables

Removed closed stores where necessary

2️⃣ Feature Engineering

Extracted temporal features

Promotion-based features

Competitor-based features

Holiday impact features

3️⃣ Model Training

Trained regression model for sales prediction

Optimized using validation split

Evaluated using RMSPE (Root Mean Square Percentage Error)

📈 Evaluation Metric

The competition uses:


Lower score = Better model performance.

🚀 Results
Metric	Score
Public Leaderboard	0.12104
Private Leaderboard	0.13800

The model successfully captures promotional effects and seasonal trends in sales.

🛠 Tech Stack

Python

Pandas

NumPy

Scikit-learn

Matplotlib / Seaborn

Jupyter Notebook

📌 Key Learnings

Importance of time-series feature engineering

Handling retail promotional effects

Working with large real-world datasets

Kaggle submission workflow

Model evaluation using RMSPE