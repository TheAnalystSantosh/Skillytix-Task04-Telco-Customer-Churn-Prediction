# Telco Customer Churn Prediction  
**Skillytix Data Analytics Internship — Task 04**

## Project Overview
This project analyzes the **Telco Customer Churn** dataset and builds machine learning models to predict whether a customer is likely to churn (leave the service).  
The goal is to apply a full ML workflow including:

- Data cleaning  
- Exploratory Data Analysis (EDA)  
- Feature engineering  
- Preprocessing (OneHotEncoding + Standard Scaling)  
- Model building (Logistic Regression & Random Forest)  
- Model evaluation  
- Feature importance analysis  
- Saving the trained model pipeline  

---

## Dataset  
**Dataset used:** Telco Customer Churn  
Source: https://www.kaggle.com/blastchar/telco-customer-churn  

**Target Variable:** `Churn`  
- Yes → Customer left  
- No → Customer stayed  

**Removed Columns:**  
- `customerID` (identifier; not useful for prediction)

---

## Tools & Libraries
- Python  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- Scikit-Learn  
- Joblib  

---

## Data Preprocessing Steps
✔ Handled missing values  
✔ Converted `TotalCharges` to numeric  
✔ Dropped identifier column (`customerID`)  
✔ Encoded categorical features using **OneHotEncoder**  
✔ Scaled numerical features using **StandardScaler**  
✔ Applied `handle_unknown='ignore'` to avoid unseen-category errors  

---

## Models Trained
### 1️ Logistic Regression  
- Works well for baseline classification  
- Evaluated using Accuracy, Classification Report & ROC–AUC  

### 2️ Random Forest Classifier  
- Performed best in experimentation  
- Used to extract **feature importances**  
- Saved as deployable model pipeline  

---

## Evaluation Metrics
Models evaluated on:

- Accuracy  
- Precision  
- Recall  
- F1-Score  
- ROC–AUC  
- Confusion Matrix  

Random Forest achieved the best performance overall.

---



