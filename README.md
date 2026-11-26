# Customer Churn & Revenue Analytics — Data Engineering Capstone Project

**Submitted By:** Shruti Gupta  
**Roll Number:** 2601201028  
**GitHub Profile:** [sshrutiigupta36-web](https://github.com/sshrutiigupta36-web)

---

## Project Overview
This capstone project implements an end-to-end, reproducible AI-ready data engineering, visual analytics, and machine learning pipeline for **Retail Customer Churn & Revenue Analytics**. It transforms raw, noisy customer records into validated, engineered, ML-ready datasets alongside automated preprocessing pipelines and MLflow experiment tracking.

## Repository Structure
    Customer-Churn-Analytics-Capstone/
    ├── data/
    │   ├── raw_data.csv             # Raw ingested customer records with missing/duplicate entries
    │   └── ml_ready_data.csv        # Cleaned, imputed, scaled & one-hot encoded ML-ready dataset
    ├── models/
    │   └── trained_pipeline.pkl     # Exported Scikit-Learn ColumnTransformer + Random Forest pipeline
    ├── notebooks/
    │   └── Customer_Churn_Analytics_Capstone.ipynb  # Complete executable workflow notebook
    ├── screenshots/
    │   └── analytics_dashboard.png  # 4-panel EDA & business insights dashboard
    └── README.md                    # Project documentation & execution instructions

## Key Workflow Stages
1. **Data Acquisition & Validation:** Automated ingestion with schema checks, duplicate detection, and missing-value auditing.
2. **Data Cleaning & Imputation:** Duplicate removal, median imputation for numerical features, and mode imputation for categorical attributes.
3. **Exploratory Data Analysis (EDA) & Dashboards:** Multi-panel visual dashboard analyzing churn rates across segments, spending distributions, city-wise revenue, and feature correlations.
4. **Feature Engineering & Reusable Pipelines:** Engineered domain features (`spend_per_month_tenure`, `high_ticket_flag`) integrated into a reusable `ColumnTransformer` and `SelectKBest` pipeline.
5. **Experiment Tracking & Model Export:** Tracked parameters, accuracy metrics, and serialized artifacts using **MLflow** and **Joblib**.
6. **End-to-End Testing:** Verified deserialized pipeline inference on unseen test samples.

## How to Execute
1. Clone the repository:
   `git clone https://github.com/sshrutiigupta36-web/Customer-Churn-Analytics-Capstone.git`
2. Install required dependencies:
   `pip install pandas numpy scikit-learn matplotlib seaborn mlflow joblib`
3. Open and run `notebooks/Customer_Churn_Analytics_Capstone.ipynb` in Google Colab or Jupyter Notebook.
