# Panic-Disorder-Predictive-Model-Using-ML
Predictive Modeling of Panic Disorder Using Machine Learning
Overview
This project focuses on predicting the likelihood of Panic Disorder diagnosis using a combination of demographic, clinical, and lifestyle features. Leveraging a dataset of 12,000 individuals, we developed multiple classification models to support early detection, personalized intervention, and better mental health outcomes. This project is part of a collaborative academic initiative at Indiana University – Purdue University Indianapolis.

Objectives
Predict whether an individual is likely to be diagnosed with Panic Disorder using profile data.

Identify the most influential features using chi-square testing.

Compare classification models including Logistic Regression, Decision Tree, Random Forest, and XGBoost.

Address class imbalance using SMOTE.

Visualize and interpret model results using SHAP and Tableau.

Dataset Description
The dataset contains 12,000 rows × 16 features, including:

Demographics: Age, Gender, Family History, Personal History

Mental Health: Symptoms, Severity, Impact on Life, Psychiatric History

Lifestyle: Coping Mechanisms, Social Support, Lifestyle Factors

Target: Panic Disorder Diagnosis

Source: Kaggle - Panic Disorder Detection Dataset

Methodology
Preprocessing:
Imputation of missing values using mode

Removal of duplicates

Chi-square test for feature selection

Label encoding for categorical features

SMOTE for class balancing

Feature scaling

Models Used:
Logistic Regression

Decision Tree

Random Forest

XGBoost

Evaluation Metrics:
Accuracy

Precision, Recall, F1-Score

ROC-AUC

Confusion Matrix

Results Summary
Model	Accuracy	F1-Score	Precision	Recall	AUC
Logistic Regression	96.4%	0.59	0.60	0.59	0.98
Random Forest	99.9%	1.00	1.00	1.00	0.99
Decision Tree	99.9%	1.00	1.00	1.00	1.00
XGBoost	99.5%	0.95	0.93	0.97	0.9856

Chi-square analysis revealed that all variables except Gender were statistically significant in predicting Panic Disorder.

Tableau Dashboard Features
Gender- and age-stratified risk scores

Heatmaps for lifestyle risk triggers

Drill-down comparison: predicted vs. actual severity

Follow-up nonadherence patterns

Folder Structure
pgsql
Copy
Edit
Panic_Disorder_Prediction/
├── data/
│   └── panic_disorder_dataset.csv
├── scripts/
│   └── Project_Draft.ipynb
├── report/
│   ├── Project Report - Intro to Info.docx
│   └── Panic_Disorder_Project_Report.pdf
├── dashboard/
│   └── Presentation.pptx
├── images/
│   ├── confusion_matrix_rf.png
│   ├── shap_summary_plot.png
│   └── feature_importance_xgb.png
└── README.md
🛠 Tools & Technologies
Python: pandas, seaborn, scikit-learn, XGBoost, SHAP

Tableau for interactive visualization

Jupyter Notebook for model development

GitHub for collaboration and version control

Interpretation
Tree-based models (Random Forest, Decision Tree, XGBoost) achieved excellent performance, though overfitting was identified in Decision Tree. Logistic Regression provided a more interpretable baseline. SHAP and chi-square testing highlighted features such as current stressors, severity, coping mechanisms, and psychiatric history as key predictors.

Conclusion
This project demonstrates how machine learning techniques can be used to predict Panic Disorder diagnosis with high accuracy and explainability. The insights could inform early screening tools in mental health care and support digital biomarker development.

Team Members & Roles
Name	Contribution
Neha Kowtharapu	Data Visualization, Report Editing
Samantha Sanjeev	Model Training, Statistical Testing
Puja Darshana Mishra	Preprocessing, Tableau Dashboard
Deborupa Pal	EDA, Code Development
Amatul Raheem Safia	Hypothesis Testing, Documentation
Sai Datta Prashanth	Data Analysis, Presentation Design

Contact
For questions or suggestions, contact:
Neha Kowtharapu - nehakowtharapu@gmail.com
