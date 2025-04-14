# 🏥 Hospital Readmission Predictive Models for Diabetes

## 📊 Introduction

The dataset spans a decade (1999–2008) of clinical care across 130 U.S. hospitals and integrated delivery networks (obtained from Machine Learning Repository website).  
Each record reflects a patient diagnosed with diabetes, including details about their hospital stay (up to 14 days), lab tests, and medications.

Inadequate diabetes management not only escalates hospital operational costs due to frequent readmissions but also worsens patient outcomes by increasing the risk of diabetes-related complications, morbidity, and mortality.


## 🎯 Business Objective

The goal of this project is to identify and understand the key factors contributing to early hospital readmissions among diabetic patients.

Although various treatment strategies have proven effective in improving clinical outcomes for diabetes, a significant portion of patients either do not receive these treatments or fail to adhere to them after discharge.

This gap in diabetes care leads to costly hospital readmissions and puts patients at increased risk of serious health complications.

By analyzing historical patient data, we aim to build predictive models that can flag individuals at high risk of readmission — supporting proactive care planning and ultimately improving both health outcomes and hospital resource efficiency.

## 🤖 Model Development and Evaluation

In this project, several machine learning models were developed and evaluated — including:

- **XGBoost**
- **LightGBM**
- **Random Forest**
- **Ensemble Model** (combining XGBoost and Random Forest)

Each model was implemented in two configurations:
- **Default** settings
- **Tuned** using hyperparameter optimization

Model performance was assessed using metrics such as **Accuracy**, **Precision**, **Recall**, **F1-score**, and **AUC**, along with **ROC curves** for visual comparison.

To further evaluate model reliability, test data from **five real patients** was used to assess how accurately each model predicts hospital readmission:

- **XGBoost**, **Random Forest**, and the **Ensemble model** each correctly predicted readmission status for all five patients (100% accuracy).
- **LightGBM** correctly predicted four out of five patient outcomes.

This demonstrates a high degree of predictive accuracy, especially in models using ensemble and tree-based strategies.

## 🚀 Final Product & Dashboard

The final prototype product is delivered as an interactive **Dash/Plotly web dashboard**.

This dashboard includes:
- A single tab interface showcasing key metrics and charts.
- Visualizations of each model’s performance using ROC curves and grouped bar charts for KPIs.
- A prediction output table showing how each selected model predicts readmission for five example patients.

Users can select and compare one or more models interactively, making the dashboard a valuable tool for data exploration, validation, and presentation to stakeholders.
