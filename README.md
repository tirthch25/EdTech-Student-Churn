# 🎓 EdTech Student Churn Analytics (Explainable ML Project)

## 📊 Project Overview
A real-world, end-to-end **Data Analytics & Machine Learning project** focused on predicting **student churn in an EdTech platform** using behavioral engagement, assessment performance, and demographic data.

This project is designed to mirror **industry-level churn analytics**, combining:
- Behavioral data analysis
- Predictive modeling
- Explainable AI (SHAP)
- Business-driven insights
- Dashboard-ready outputs

---

## 🎯 Problem Statement
Online learning platforms face high student dropout rates, often detected **too late**.

### Objectives:
- Identify students at risk of dropping out (churn)
- Understand behavioral and academic drivers of churn
- Predict churn **before official withdrawal**
- Provide actionable retention insights for stakeholders

### Churn Definition:
- `Withdrawn` students → **Churned**
- Early warning signals:
  - ≥ 14 days of inactivity
  - Missed assessments
  - Declining engagement

---

## 🗂️ Dataset
**Open University Learning Analytics Dataset (OULAD)**  
A research-grade EdTech dataset containing student interaction logs, assessment results, and demographics.

### Key Data Files:
- `studentInfo.csv` – Demographics & final results
- `studentVle.csv` – Clickstream engagement data
- `vle.csv` – Learning resource metadata
- `assessments.csv` – Assessment details
- `studentAssessment.csv` – Scores & submissions

> Raw data is preserved for transparency and reproducibility.

---

## ⚙️ Methodology Overview

### Phase 1 – Data Understanding
- Loaded raw CSV files
- Inspected schema, missing values, and distributions
- Identified key churn indicators

### Phase 2 – Feature Engineering
- Aggregated engagement metrics (total clicks, active days)
- Engineered inactivity and consistency features
- Calculated assessment-based performance metrics
- Created churn labels and early-risk indicators

### Phase 3 – Exploratory Data Analysis (EDA)
- Compared engagement patterns of churned vs retained students
- Analyzed assessment behavior impact
- Identified correlations and behavioral trends
- Generated visual insights for decision-making

### Phase 4 – Modeling & Evaluation
- Built classification models:
  - Logistic Regression (baseline)
  - Random Forest (non-linear patterns)
- Evaluation metrics:
  - Recall (primary)
  - ROC-AUC
  - Confusion Matrix

### Phase 5 – Explainable AI (SHAP)
- Identified global churn drivers
- Explained individual student predictions
- Translated model output into business actions

---

## 📈 Key Insights
- Students inactive for 14+ days are highly likely to churn
- Engagement consistency matters more than occasional spikes
- Missed assessments strongly correlate with dropout
- Certain resource types improve retention

---

## 💡 Business Recommendations
- Trigger early alerts for prolonged inactivity
- Provide academic support for missed assessments
- Personalize learning content for low-engagement students
- Prioritize high-risk students for retention campaigns

---

## 🛠️ Tech Stack
- **Python**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Machine Learning**: Scikit-learn
- **Explainable AI**: SHAP
- **Dashboarding**: Power BI (designed)
- **Version Control**: Git & GitHub

---

## 📂 Repository Structure

```
EdTech-Student-Churn/
│
├── data/
│   ├── raw/
│   │   ├── studentInfo.csv
│   │   ├── studentVle.csv
│   │   ├── vle.csv
│   │   ├── assessments.csv
│   │   └── studentAssessment.csv
│   │
│   └── processed/
│       ├── edtech_churn_final.csv
│       └── shap_feature_importance.csv
│
├── notebooks/
│   ├── 01_data_understanding.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_exploratory_data_analysis.ipynb
│   ├── 04_modeling.ipynb
│   └── 05_explainability_shap.ipynb
│
├── dashboard/
│   └── power_bi_dashboard_design.md
│
└── README.md

```
---
## 🧹 Key Deliverables (Final)

|Phase |	Deliverable                             |Status       |
|------|------------------------------------------|-------------|
|Phase 1|	Data loading, cleaning & validation	    |✅ Completed |
|Phase 2|	Feature engineering & churn labeling	  |✅ Completed |
|Phase 3|	EDA & behavioral insights	              |✅ Completed |
|Phase 4|	ML modeling & evaluation	              |✅ Completed |
|Phase 5|	Explainable AI & churn drivers	        |✅ Completed |

---


---

## 📊 Final Outputs
- **Processed Dataset**: `edtech_churn_final.csv`
- **ML Outputs**: Churn probabilities per student
- **Explainability**: SHAP feature importance
- **Dashboard**: Power BI churn & engagement analytics

---

## 🚀 How to Run
```bash
git clone https://github.com/<your-username>/EdTech-Student-Churn.git
cd EdTech-Student-Churn
pip install -r requirements.txt
jupyter notebook notebooks/01_data_understanding.ipynb
```
---

## 📧 Contact

**Contact:** [tirthchankeshwara@gmail.com](mailto:tirthchankeshwara@gmail.com)

---
