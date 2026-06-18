# 📊 Telco Customer Churn Prediction

## Project Overview

Customer churn is one of the most critical challenges faced by telecommunications companies. Retaining existing customers is significantly more cost-effective than acquiring new ones. This project focuses on predicting customer churn using machine learning techniques and identifying the key factors influencing customer retention.

The objective is to build a robust predictive model capable of identifying customers likely to leave the service, enabling businesses to take proactive retention measures.

---

## Business Problem

Telecommunication companies lose revenue when customers discontinue their services. By accurately predicting churn, organizations can:

* Improve customer retention strategies
* Reduce revenue loss
* Optimize marketing campaigns
* Enhance customer satisfaction
* Identify high-risk customer segments

---

## Project Objectives

* Perform exploratory data analysis (EDA)
* Identify patterns and drivers of customer churn
* Preprocess and engineer features
* Handle class imbalance using SMOTE
* Compare multiple machine learning models
* Select the best-performing model using cross-validation
* Interpret model predictions using SHAP Explainability
* Save the trained model for future deployment

---

## Dataset Information

Dataset: WA_Fn-UseC-Telco Customer Churn Dataset

The dataset contains customer demographics, account information, service subscriptions, and churn status.

### Features Include

* Customer Demographics
* Gender
* Senior Citizen Status
* Partner Information
* Dependents
* Tenure
* Internet Services
* Phone Services
* Contract Type
* Payment Method
* Monthly Charges
* Total Charges

### Target Variable

* Churn

  * Yes = Customer left the service
  * No = Customer retained

---

## Project Workflow

### 1. Data Collection

* Load Telco Customer Churn dataset
* Understand dataset structure

### 2. Data Cleaning

* Handle data quality issues
* Convert data types
* Remove unnecessary columns

### 3. Exploratory Data Analysis (EDA)

* Churn Distribution Analysis
* Contract Type Analysis
* Monthly Charges Analysis
* Tenure Analysis
* Internet Service Analysis
* Correlation Heatmap

### 4. Data Preprocessing

* Label Encoding
* One-Hot Encoding
* Feature Preparation
* Train-Test Split

### 5. Handling Class Imbalance

SMOTE (Synthetic Minority Oversampling Technique) was used to address class imbalance and improve model learning.

### 6. Model Development

The following models were evaluated using 5-Fold Cross Validation:

* XGBoost Classifier
* LightGBM Classifier
* Random Forest Classifier

### 7. Model Evaluation

Evaluation Metrics:

* ROC-AUC Score
* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

### 8. Model Explainability

SHAP (SHapley Additive exPlanations) was used to:

* Understand feature importance
* Explain individual predictions
* Improve model interpretability

### 9. Model Persistence

The final model was saved using Joblib for future deployment and inference.

---

## Model Comparison Results

| Model         | ROC-AUC Score |
| ------------- | ------------- |
| XGBoost       | 0.9301        |
| LightGBM      | 0.9306        |
| Random Forest | 0.9288        |

🏆 Best Performing Model: LightGBM

---

## Key Findings

* Customers with month-to-month contracts exhibit higher churn rates.
* Customers with shorter tenure are more likely to churn.
* Higher monthly charges are associated with increased churn probability.
* Contract type significantly impacts customer retention.
* SHAP analysis confirmed tenure and contract type as major churn drivers.

---

## Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Imbalanced-Learn
* LightGBM
* XGBoost
* SHAP
* Joblib

---

## Project Structure

```text
Telco-Customer-Churn-Prediction/
│
├── data/
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
│
├── plots/
│   ├── churn_distribution.png
│   ├── correlation_heatmap.png
│   ├── confusion_matrix.png
│   └── shap_summary.png
│
├── models/
│   └── telco_churn_model.pkl
│
├── Telco_Customer_Churn.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

---

## How to Run

### Clone Repository

```bash
git clone <repository-url>
```

### Navigate to Project Directory

```bash
cd Telco-Customer-Churn-Prediction
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Notebook

```bash
jupyter notebook
```

---

## Future Improvements

* Hyperparameter Optimization
* Streamlit Deployment
* Docker Containerization
* CI/CD Integration
* Cloud Deployment

---

## Author

S.PADMANABHAN

Aspiring AI Engineer | Machine Learning Enthusiast | Data Science Practitioner
