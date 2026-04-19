# Customer Churn Prediction using Machine Learning

This project predicts whether a telecommunications customer will leave (churn) based on their usage patterns and demographic data. It uses historical data to help businesses proactively retain customers.

## 🚀 Project Overview
Customer churn is a major challenge for service-based industries. This project involves:
* Data Cleaning and Exploratory Data Analysis (EDA).
* Handling class imbalance using **SMOTE** (Synthetic Minority Over-sampling Technique).
* Building and evaluating multiple classification models.
* Feature importance analysis to identify key churn drivers.

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn
* **Environment:** Jupyter Notebook / Google Colab

## 📊 Dataset
The project uses the **Telco Customer Churn** dataset, which includes information about:
* **Demographics:** Gender, seniority, partners, and dependents.
* **Services:** Phone, multiple lines, internet, online security, etc.
* **Account Info:** Tenure, contract type, payment method, and monthly charges.

## 📈 Model Performance
I evaluated multiple models on the balanced training set. The **Random Forest Classifier** was chosen as the final model based on its cross-validation stability.

* **Random Forest Classifier:** **84%** (Cross-Validation Accuracy) | **77.86%** (Final Test Accuracy)
* **XGBoost Classifier:** **83%** (Cross-Validation Accuracy)
* **Decision Tree:** **78%** (Cross-Validation Accuracy)

## 🏆 Final Result (Random Forest)
The model was tested on unseen data (test set) to ensure real-world reliability:

| Metric | Score |
| :--- | :--- |
| **Accuracy** | 77.86% |
| **Precision (Churn)** | 0.58 |
| **Recall (Churn)** | 0.59 |
| **F1-Score** | 0.58 |

## 📂 Project Structure
```text
├── data/                   # Dataset files
├── notebooks/              # Jupyter notebooks
├── models/                 # Saved .pkl model and encoders
├── README.md               # Project documentation
└── requirements.txt        # List of dependencies
