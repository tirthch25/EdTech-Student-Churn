🎓 EdTech Student Churn Analytics (Explainable ML Project)

A data-driven analysis of student dropout behavior in online education platforms — identifying early churn signals, analyzing engagement patterns, building predictive models, and delivering explainable insights to improve student retention.

👥 Project Author

Tirth Chankeshwara

🎯 Problem Statement

Online EdTech platforms face high student dropout rates, leading to revenue loss and reduced learning outcomes.
This project aims to:

Identify early indicators of student churn

Analyze behavioral engagement and assessment patterns

Predict student dropout using machine learning

Explain why students churn using Explainable AI (SHAP)

Provide actionable retention strategies for EdTech platforms

🗂️ Data Sources

Open University Learning Analytics Dataset (OULAD) — a real-world academic dataset widely used in EdTech research.

Key Data Files Used:

studentInfo.csv – demographics, final results

studentVle.csv – student clickstream activity

vle.csv – learning resource metadata

assessments.csv – assessment structure

studentAssessment.csv – assessment submissions & scores

Integration Strategy:

Merged datasets using id_student, code_module, code_presentation

Aggregated clickstream data to create engagement metrics

Derived churn labels from final student outcomes

⚙️ Methodology Overview
Phase 1 – Data Understanding & Cleaning (Completed)

Loaded and validated raw CSV files

Handled missing values, duplicates, and inconsistent categories

Standardized demographic and categorical variables

Verified data integrity before feature engineering

Phase 2 – Feature Engineering (Completed)

Engineered behavioral engagement metrics:

Total clicks

Active days

Engagement consistency

Resource-type usage

Created early churn indicators:

Long inactivity gaps

Missed assessments

Low average scores

Generated binary churn label:

Withdrawn → Churned

Pass / Distinction → Retained

Phase 3 – Exploratory Data Analysis (Completed)

Univariate and bivariate analysis of churn vs engagement

Resource-type usage comparison for churned vs retained students

Demographic impact analysis (age, education level)

Correlation analysis on numerical engagement features

Key Insights:

Students inactive for 14+ days have high churn probability

Engagement consistency matters more than total clicks

Missed assessments strongly correlate with dropout

Certain learning resources improve retention

Phase 4 – Modeling & Evaluation (Completed)

Models Implemented:

Logistic Regression (interpretable baseline)

Random Forest Classifier (non-linear patterns)

Evaluation Metrics:

Recall (primary metric – identify at-risk students)

ROC-AUC

Confusion Matrix

Results:

Random Forest achieved superior recall and ROC-AUC

Model successfully detects churn before final withdrawal

Phase 5 – Explainable AI (Completed)

Applied SHAP (SHapley Additive exPlanations)

Identified global and individual churn drivers

Saved SHAP feature importance for reporting

Top Churn Drivers Identified:

Prolonged inactivity

Low engagement consistency

Poor assessment performance

Reduced interaction with core learning resources

📁 Repository Structure
EdTech-Student-Churn/
│
├── README.md
│
├── data/
│   ├── raw/                         # Original OULAD datasets
│   │   ├── studentInfo.csv
│   │   ├── studentVle.csv
│   │   ├── vle.csv
│   │   ├── assessments.csv
│   │   └── studentAssessment.csv
│   │
│   └── processed/                   # Cleaned & engineered datasets
│       ├── edtech_churn_final.csv
│       └── shap_feature_importance.csv
│
├── notebooks/                       # Jupyter notebooks by phase
│   ├── 01_data_understanding.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_exploratory_data_analysis.ipynb
│   ├── 04_modeling.ipynb
│   └── 05_explainability_shap.ipynb
│
└── dashboard/                       # (Optional future dashboards)

🧹 Key Deliverables (Final)
Phase	Deliverable	Status
Phase 1	Data loading, cleaning & validation	✅ Completed
Phase 2	Feature engineering & churn labeling	✅ Completed
Phase 3	EDA & behavioral insights	✅ Completed
Phase 4	ML modeling & evaluation	✅ Completed
Phase 5	Explainable AI & churn drivers	✅ Completed
📊 Final Outputs

Processed Dataset: edtech_churn_final.csv

Explainability: shap_feature_importance.csv

Models: Logistic Regression, Random Forest

Insights: Engagement-driven churn prediction

Visuals: Engagement plots, churn comparisons, SHAP summaries

🛠️ Tech Stack

Python

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

SHAP

Jupyter Notebook

Git & GitHub

🚀 Business Impact

Enables early identification of at-risk students

Helps EdTech platforms reduce dropout rates

Supports data-driven retention strategies

Demonstrates production-ready analytics thinking

📧 Contact

Author: Tirth Chankeshwara
Domain: Data Analytics | Machine Learning | AI
Contact: tirthchankeshwara@gmail.com
