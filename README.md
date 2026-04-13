# Francis Affonah
**Data Scientist · Healthcare Analytics · ML Engineering**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Francis_Affonah-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/francis-affonah-23745a205/)
[![GitHub](https://img.shields.io/badge/GitHub-faffonahjn-181717?style=flat&logo=github)](https://github.com/faffonahjn)
[![Live API](https://img.shields.io/badge/Live%20API-Azure%20Deployed-success?style=flat&logo=microsoftazure)](https://insurance-risk-api.redsand-37d94e81.eastus.azurecontainerapps.io/docs)

---

Registered nurse turned data scientist. I work at the intersection of clinical domain expertise and production machine learning building systems that don't just model health outcomes, but reflect how care actually works.

My anchor project: a **Medical Insurance Risk Classifier** deployed live on **Azure Container Apps** — full production ML pipeline from data leakage forensic audit through XGBoost training, FastAPI serving, Streamlit clinical dashboard, Docker containerization, and 21 automated tests. The most important engineering decision wasn't the model — it was rejecting a perfect AUC of 1.0.

---

## Core Stack

| Layer | Tools |
|---|---|
| **Languages** | Python · SQL · R |
| **ML & Analysis** | XGBoost · Scikit-learn · Pandas · NumPy · Statsmodels · SHAP |
| **Deployment** | FastAPI · Docker · Azure Container Apps · MLOps |
| **Visualization** | Tableau · Power BI · Matplotlib · Seaborn · Streamlit |
| **Workflow** | Git · GitHub · Jupyter · MLflow |

---

## Selected Projects

### 🏦 Medical Insurance Risk Classifier *(Live on Azure)*
Production ML system predicting high-cost insurance patients (charges > P75) from demographic and lifestyle features. Includes full **data leakage forensic audit** caught a 100% deterministic target rule (AUC 1.0), rebuilt label with actuarial intent, yielding defensible AUC of 0.899. SHAP explainability, threshold sensitivity analysis, and a 4-tab Streamlit clinical dashboard. Deployed publicly on **Azure Container Apps**.

**Test AUC: 0.899 | Sensitivity: 76.1% | Specificity: 95.5% | 21 tests passing**

[**Live API →**](https://insurance-risk-api.redsand-37d94e81.eastus.azurecontainerapps.io/docs)

`Python` `XGBoost` `FastAPI` `Streamlit` `Docker` `Azure Container Apps` `SHAP`

---

### 🧬 Fertility Outcome Classifier *(Production ML)*
End-to-end clinical ML system predicting pregnancy success from couples' health, lifestyle, and treatment features. Key engineering decisions: **informative NaN strategy** (Treatment_Type and Alcohol_Intake nulls domain-filled rather than statistically imputed), **Female_Age × Motility interaction feature** (age-adjusted reproductive potential), and **threshold tuned to 0.40** for Failure class recall — missing a high-risk couple closes the treatment window. FastAPI REST API, 4-tab Streamlit dashboard, Docker Compose, 24-test suite.

**Test AUC: 0.950 | Avg Precision: 0.980 | 24 tests passing**

`Python` `XGBoost` `FastAPI` `Streamlit` `Docker` `SHAP` `Clinical Feature Engineering`

---

### 🏥 SDI Health Facility ML Pipeline
End-to-end pipeline classifying health facility competency gaps across **5,000+ facilities in 10 African countries** using World Bank SDI data. Identified maternal health crisis: 5-6% competency in emergency obstetric care. Generated 18 evidence-based policy recommendations for governments and international partners.

`Python` `Scikit-learn` `FastAPI` `Docker` `Pandas` `Public Health Analytics`

---

### ❤️ Heart Disease Risk Prediction
Clinical classification model predicting cardiovascular risk from patient-level features. Emphasis on model interpretability alongside predictive performance built for clinical utility, not just accuracy metrics.

`Python` `Scikit-learn` `Feature Engineering` `Model Evaluation`

---

### 🧠 Stroke Risk Prediction
Full analytics lifecycle: raw clinical data → preprocessing → EDA → predictive model. Documents clinical reasoning behind feature selection decisions.

`Python` `EDA` `Classification` `Healthcare Analytics`

---

### 📊 Customer Sales Performance Dashboard
Interactive Tableau dashboard surfacing sales trends, customer segmentation, and KPI performance for business stakeholders.

`Tableau` `SQL` `Business Analytics`

---

### 📈 Stress Pattern Analysis
Behavioral and physiological indicator analysis linking data patterns to stress outcomes. Exploratory and statistical in nature.

`Python` `Statistical Analysis` `EDA`

---

## Background

I came to data science from nursing — which means I read clinical datasets differently. I understand what an abnormal lab value means before it becomes a feature, what care delivery constraints look like before they appear in operational data, and why health equity isn't just a keyword but a modeling decision.

That clinical grounding shapes how I build: interpretable models over black boxes where it matters, domain-aware feature engineering, and outputs designed for people who make care decisions not just people who read dashboards.

Currently deepening expertise in **Azure Data Engineering**, **TensorFlow**, and **medical imaging analytics (Computer Vision)**.

---

## Certifications

- IBM Data Science Professional Certificate
- Clinical Data Science Certificate
- Registered Nurse Certificate

---

*Open to health data science roles, healthcare analytics positions, and collaborations at the intersection of clinical domain and ML engineering.*

> *"So built we the wall... for the people had a mind to work."* — Nehemiah 4:6
