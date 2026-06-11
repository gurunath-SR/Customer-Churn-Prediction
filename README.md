# 📊 Customer Churn Prediction

## 📌 Project Overview

Customer churn is one of the biggest challenges faced by subscription-based businesses. Acquiring new customers is often more expensive than retaining existing ones. This project aims to predict whether a telecom customer is likely to leave the company (churn) based on demographic information, account details, and subscribed services.

The solution leverages Machine Learning techniques to identify customers at risk of churn, enabling businesses to implement proactive retention strategies and reduce revenue loss.

---

## 🎯 Problem Statement

Build a machine learning model that predicts whether a telecom customer will churn using historical customer data.

**Business Question:**

> Can we identify customers who are likely to leave the company before they actually churn?

---

## 🚀 Live Demo

**Deployed Streamlit Application:**

https://customer-churn-prediction-tn2m6mlmmnnst9poqemygq.streamlit.app/

---

## 📊 Dataset Information

- **Dataset:** IBM Telco Customer Churn Dataset
- **Records:** 7,043 customers
- **Features:** 21 variables
- **Target Variable:** `Churn`
  - `Yes` → Customer left the company
  - `No` → Customer stayed with the company

---

## 🛠️ Technologies Used

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Scikit-learn
- Joblib
- Streamlit

### Machine Learning Models
- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

### Tools
- Jupyter Notebook
- Git & GitHub
- Streamlit Cloud

---

## 📂 Project Structure

```text
Customer-Churn-Prediction/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── models/
│   └── churn_pipeline.pkl
│
├── notebooks/
│   ├── 01_EDA.ipynb
│   ├── 02_Feature_Engineering.ipynb
│   ├── 03_Model_Training.ipynb
│   └── 04_Pipeline_and_Deployment.ipynb
│
├── streamlit_app/
│   └── app.py
│
├── requirements.txt
├── runtime.txt
├── README.md
└── .gitignore
```

---

## 🔍 Project Workflow

### Phase 1: Data Understanding
- Loaded and explored the telecom dataset.
- Checked data types and distributions.
- Identified the target variable.

### Phase 2: Data Cleaning & Preprocessing
- Converted `TotalCharges` to numeric format.
- Handled missing values.
- Removed unnecessary columns such as `customerID`.

### Phase 3: Feature Engineering
- Applied one-hot encoding to categorical variables.
- Scaled numerical features:
  - Tenure
  - Monthly Charges
  - Total Charges
- Performed train-test split using stratification.

### Phase 4: Model Training
Trained multiple machine learning models:
- Logistic Regression
- Random Forest
- XGBoost

### Phase 5: Model Evaluation
Compared models using:
- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Score

### Phase 6: Pipeline Development
Created an end-to-end machine learning pipeline integrating:
- Feature scaling
- Prediction model

Saved the pipeline using Joblib for deployment.

### Phase 7: Deployment
Developed an interactive Streamlit application and deployed it on Streamlit Cloud.

---

## 📈 Model Performance

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---------|-----------|------------|---------|-----------|----------|
| Logistic Regression | 80.45% | 65.05% | 57.22% | 60.88% | 83.61% |
| Random Forest | 78.82% | 62.34% | 51.34% | 56.31% | 81.56% |
| XGBoost | 77.83% | 58.91% | 54.81% | 56.79% | 81.97% |

### Final Model Selected

✅ **Logistic Regression**

**Reason:**
- Best balance between predictive performance and interpretability.
- Enables business stakeholders to understand the factors influencing churn.

---

## 📌 Key Business Insights

### Factors Increasing Churn Risk
- Fiber optic internet service
- Electronic check payment method
- Month-to-month contracts
- Streaming service subscriptions

### Factors Reducing Churn Risk
- Longer customer tenure
- One-year contracts
- Two-year contracts
- Online security services
- Tech support services

### Most Influential Feature

🏆 **Customer Tenure**

Customers who have been with the company for a longer period are significantly less likely to churn.

---

## 💡 Business Impact

This solution can help telecom companies:

- Identify high-risk customers early.
- Design targeted retention campaigns.
- Improve customer satisfaction.
- Reduce customer acquisition costs.
- Increase long-term revenue.

---

## ▶️ How to Run Locally

### Clone the Repository

```bash
git clone <repository-url>
cd Customer-Churn-Prediction
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Launch the Streamlit Application

```bash
streamlit run streamlit_app/app.py
```

---

## 📸 Application Features

- Interactive user interface
- Customer churn prediction
- Churn probability estimation
- Real-time predictions based on user inputs

---

## 🎓 Learning Outcomes

Through this project, I gained practical experience in:

- Exploratory Data Analysis (EDA)
- Data preprocessing techniques
- Feature engineering
- Classification algorithms
- Model evaluation
- Pipeline creation
- Streamlit application development
- Cloud deployment using Streamlit Cloud
- End-to-end machine learning workflow

---

## 👨‍💻 Author

**Gurunath S R**

Aspiring Data Scientist passionate about solving real-world business problems using Machine Learning and Data Analytics.

- GitHub: https://github.com/gurunath-sr
- Live Demo: https://customer-churn-prediction-tn2m6mlmmnnst9poqemygq.streamlit.app/

---

⭐ If you found this project interesting, consider giving this repository a star!
