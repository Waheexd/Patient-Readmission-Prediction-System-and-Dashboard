🏥 Patient Readmission Analysis using PySpark & Power BI
Overview
This project focuses on analyzing hospital patient readmission patterns using the UCI Diabetic Readmission Dataset. 
The goal is to predict patient readmissions, identify key factors driving them, and visualize insights through an interactive Power BI dashboard. 
The entire workflow — from cleaning to modeling — is automated using PySpark, enabling scalable and reproducible healthcare analytics.

🚀Project Objectives
Build an end-to-end machine learning pipeline in PySpark to predict patient readmissions.
Handle class imbalance using SMOTE and optimize model performance
Export clean, interpretable predictions for visualization in Power BI.
Deliver actionable insights to support hospital resource planning and readmission reduction strategies.

🤖Tech Stack
Data Processing: PySpark, Pandas

Balancing: SMOTE (imblearn)

Modeling: PySpark MLlib (Random Forest)

Visualization: Power BI

EDA & Charts: Matplotlib, Seaborn

Environment: Google Colab / Jupyter

⚙️Workflow

1. Data Preparation
Imported the UCI Diabetic Readmission dataset.
Cleaned and standardized columns (race, gender, age, admission_type_id, time_in_hospital, num_medications, number_diagnoses, etc.).
Removed duplicates, invalid entries (?, Unknown), and unnecessary fields.
Encoded categorical features using StringIndexer and assembled features for modeling.

2. Model Development (PySpark MLlib)
Built a pipeline using:
StringIndexer → VectorAssembler → StandardScaler → RandomForestClassifier
Applied SMOTE on sampled data to address class imbalance.
Evaluated model using AUC, Precision, and Recall metrics.
Exported predictions for visualization.

3. Visualization (Power BI)
Designed a Power BI dashboard displaying demographic and clinical readmission trends.
Created KPIs and visuals to monitor performance metrics and treatment patterns.

🎯Key Insights
Higher readmission rates are observed among patients with longer hospital stays, multiple diagnoses, and higher medication counts.
Age and treatment type (insulin/diabetesMed) have noticeable effects on readmission probability.
Certain admission and discharge types show recurring readmission patterns, suggesting operational inefficiencies.






Designed a Power BI dashboard displaying demographic and clinical readmission trends.

Created KPIs and visuals to monitor performance metrics and treatment patterns.
