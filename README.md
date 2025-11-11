# Hospital Readmission Prediction for Diabetic Patients

## Project Overview

This project predicts hospital readmission risk for diabetic patients using machine learning, with a focus on integrating social determinants of health and demographic context to improve upon traditional clinical-only models.

## Objectives

- Predict 30-day hospital readmission risk for diabetic patients
- Identify high-utilization patients for targeted interventions
- Analyze fairness and bias across demographic subgroups
- Provide interpretable features for clinical decision-making

## Datasets

**Primary Dataset:**
- [UCI Diabetes 130-US Hospitals (1999-2008)](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008)
- 101,766 admissions across 130 US hospitals
- 47 clinical and demographic features

**Additional Dataset (to be merged):**
- [BRFSS CDC Data](https://www.kaggle.com/datasets/lplenka/brfss-data)
- 491,775 survey responses with demographic and behavioral health data
- Features: BMI, high blood pressure, cholesterol, physical activity, smoking, income, education, healthcare access
- Aggregated by race/age/gender and merged with UCI data

## Workflow

| Stage | Description | File/Link | Done by |
|-------|-------------|-------------|-------------|
| **Data Integration** | Merge UCI dataset with BRFSS demographic health data | [data_merging.ipynb](https://github.com/kristenlowe/hospital-readmission/blob/main/data_merging.ipynb) | Kristen |
| **Data Cleaning and Feature Engineering** | Handle missing values; Create literature-based predictive features: polypharmacy burden (medication count thresholds), glycemic control proxy (HbA1c testing + diabetes medication changes), discharge instability score (admission urgency + procedure volume + length of stay) | | |
| **EDA** | Explore patterns, correlations, and disparities | | |
| **Modeling and Evaluation** | Logistic regression (L1 penalty), comparison with other models, accuracy, fairness metrics, feature importance | | |
| **Blog Report** | Blog-based project report | | |
| **Presentation** | In-class Powerpoint presentation | | |
