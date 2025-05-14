# 📊 Telco Customer Churn Prediction

Welcome to my Telco Churn Prediction project! This repository demonstrates a complete data science workflow—from exploratory data analysis (EDA) to building and evaluating machine learning models—to predict customer churn for a telecommunications company.

---

## 🚀 Project Overview

Customer churn is a critical business problem for telecom companies. Accurately predicting which customers are likely to leave enables proactive retention strategies and improved business outcomes.

In this project, I:
- Explored and visualized the Telco customer dataset
- Engineered features and handled missing values
- Built and evaluated multiple machine learning models
- Tuned models and addressed class imbalance
- Deployed the best model with a modern web UI

---

## 🗂️ Repository Structure
├── EDA.ipynb # Exploratory Data Analysis notebook ├── Model Building.ipynb # Model training, evaluation, and deployment ├── main dataset.csv # Raw Telco customer data ├── tel_churn.csv # Processed data after feature engineering ├── templates/ │ └── home.html # Modern Bootstrap web UI for predictions ├── model2.sav # Final pickled model └── README.md # Project documentation

---

## 📈 Exploratory Data Analysis (EDA)

- Visualized churn distribution and feature relationships
- Identified key drivers of churn (e.g., contract type, tenure, monthly charges)
- Engineered new features (e.g., tenure groups)
- Handled missing values and outliers
- Key insights:
  - 📉 **Month-to-month contracts** and **electronic check payments** have higher churn
  - 🔒 Lack of **online security** and **tech support** increases churn risk
  - 💰 **Higher monthly charges** and **lower tenure** are linked to higher churn

---

## 🤖 Model Building & Evaluation

- **Preprocessing:** One-hot encoding, feature scaling, and class balancing (SMOTEENN)
- **Models:** Decision Tree, Random Forest (with and without SMOTEENN), PCA for dimensionality reduction
- **Evaluation:** Accuracy, precision, recall, F1-score, ROC-AUC, confusion matrix
- **Hyperparameter Tuning:** Grid search for optimal Random Forest parameters
- **Feature Importance:** Identified top predictors of churn

**Best Model:**  
Random Forest with SMOTEENN balancing  
- ROC-AUC: **0.84**
- High recall for churners (catching more customers at risk)

---

## 🌐 Web App

- Built a modern, responsive UI using **Bootstrap 5**
- Users can input customer details and get instant churn predictions with probability
- Ready for deployment as a Flask app

---

## 🛠️ How to Run

1. **Clone the repository**
2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
