# Francis Affonah
**ML Engineer · Insurance & HealthTech · RAG Systems · Clinical ML**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Francis_Affonah-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/francis-affonah-23745a205/)
[![GitHub](https://img.shields.io/badge/GitHub-faffonahjn-181717?style=flat&logo=github)](https://github.com/faffonahjn)
[![Insurance API](https://img.shields.io/badge/Live%20API-Insurance%20Risk-success?style=flat&logo=microsoftazure)](https://insurance-risk-api.redsand-37d94e81.eastus.azurecontainerapps.io/docs)
[![Fertility API](https://img.shields.io/badge/Live%20API-Fertility%20Classifier-success?style=flat&logo=microsoftazure)](https://fertility-api.redsand-37d94e81.eastus.azurecontainerapps.io/docs)
[![PharmIQ API](https://img.shields.io/badge/Live%20API-PharmIQ-success?style=flat&logo=microsoftazure)](https://pharmiq-api.redsand-37d94e81.eastus.azurecontainerapps.io/docs)

---

Registered nurse turned ML engineer. Clinical practice changes how I read data — an abnormal value carries meaning before it becomes a feature, a missing value can be the signal rather than the noise, and a wrong prediction in healthcare is never just a metric problem.

Five production systems built and deployed. Two target the insurance domain directly. One is a full agentic RAG system built without LangChain.

---

## Core Stack

| Layer | Tools |
|---|---|
| **LLM / RAG** | Groq · HuggingFace Transformers · pgvector · Hybrid Search · Prompt Engineering |
| **Languages** | Python · SQL · R |
| **ML & Analysis** | XGBoost · LightGBM · Scikit-learn · Pandas · NumPy · SHAP · Optuna |
| **Deployment** | FastAPI · Docker · Azure Container Apps · GitHub Actions CI · MLflow · pytest |
| **Visualization** | Streamlit · Tableau · Power BI · Matplotlib · Seaborn |
| **Workflow** | Git · GitHub · Jupyter · VS Code |

---

## Production Systems

### ClinicalMind RAG — Agentic Multi-Domain RAG System *(Dockerized · Azure-Ready)*

Production agentic RAG pipeline built without LangChain. Three-agent architecture: RouterAgent classifies domain and retrieval strategy, RetrievalAgent executes hybrid search with Reciprocal Rank Fusion and cross-encoder reranking, SynthesisAgent generates citation-enforced answers grounded exclusively in retrieved documents.

**71/71 tests passing · Hybrid search (pgvector + BM25 + RRF) · Cross-encoder reranking · Groq LLaMA-3.3-70B**

Raw agent orchestration · PostgreSQL + pgvector HNSW index · sentence-transformers embeddings · FastAPI REST API · Streamlit UI · Docker Compose · Multi-domain: clinical, insurance, pharma, general

[**GitHub →**](https://github.com/faffonahjn/RAG_MultiDomain)

`Python` `pgvector` `PostgreSQL` `BM25` `RRF` `sentence-transformers` `Groq` `FastAPI` `Streamlit` `Docker`

---

### RAG Insurance Portal *(Live on GitHub)*

End-to-end RAG pipeline for insurance document Q&A. Upload a policy PDF, ask questions in plain English, get answers grounded in the actual document with source citations. Built on a real Ghanaian insurance policy — SIC Insurance Homeplus — not a generic demo.

**80% retrieval accuracy on 5-question eval suite**

LangChain orchestration · Chroma vector database · HuggingFace `all-MiniLM-L6-v2` embeddings · Groq Llama 3.1 generation · FastAPI REST API · Streamlit chat UI · Docker · GitHub Actions CI

[**GitHub →**](https://github.com/faffonahjn/RAG_InsurancePortal)

`Python` `LangChain` `Chroma` `HuggingFace` `Groq` `FastAPI` `Streamlit` `Docker` `GitHub Actions`

---

### Medical Insurance Risk Classifier *(Live on Azure)*

Predicts high-cost insurance claimants (charges above the 75th percentile, $16,658) from demographic and lifestyle features. At one point the model hit AUC 1.0 — I stopped rather than celebrated, found a 100% deterministic target leak, tore it down and rebuilt the label using actuarial logic. The defensible AUC is 0.899. SHAP explainability, threshold tuned to 0.35 for maximum recall, 4-tab Streamlit dashboard.

**AUC 0.899 · Sensitivity 76.1% · Specificity 95.5% · 21 tests passing**

[**Live API →**](https://insurance-risk-api.redsand-37d94e81.eastus.azurecontainerapps.io/docs)

`Python` `XGBoost` `FastAPI` `Streamlit` `Docker` `Azure Container Apps` `SHAP` `MLflow`

---

### PharmIQ — Pharmaceutical Intelligence Platform *(Live on Azure)*

Three-model unified system on 273,000+ Indian medicines: Generic Alternative Recommender (ranked cheaper alternatives by unit cost savings), Price Tier Classifier (AUC 0.8701, category-relative tiering — a ₹200 injection is cheap, a ₹200 tablet is expensive, most systems miss that), and Therapeutic Category Classifier (AUC 0.97, 13 categories from salt composition alone). Caught data leakage at AUC 1.0, rebuilt from scratch. Drift detection in production.

**AUC up to 0.97 · 98 tests passing · Drift detection in production**

[**Live API →**](https://pharmiq-api.redsand-37d94e81.eastus.azurecontainerapps.io/docs)

`Python` `XGBoost` `LightGBM` `Optuna` `FastAPI` `Streamlit` `Docker` `Azure Container Apps` `MLflow`

---

### Fertility Outcome Predictor *(Live on Azure)*

Predicts pregnancy success probability from couples' health, lifestyle, and treatment profiles. 62.5% of Treatment_Type nulls were filled as "None" — those couples received no treatment at all, and imputing the mode would have been clinically wrong. Engineered Female_Age × Motility% interaction feature. Threshold set at 0.40, not 0.50, because missing a high-risk couple closes the treatment window.

**AUC 0.9504 · Average Precision 0.9802 · 24 tests passing**

[**Live API →**](https://fertility-api.redsand-37d94e81.eastus.azurecontainerapps.io/docs)

`Python` `XGBoost` `FastAPI` `Streamlit` `Docker` `Azure Container Apps` `pytest`

---

### SDI Health Facility ML Pipeline

End-to-end pipeline analyzing 5,223 health facilities across 10 African countries using World Bank SDI data. Found 5.2% competency in eclampsia management across the dataset. Kenya scored 38.5% — 71% above average — which meant the solution already existed somewhere. Generated 18 evidence-based policy recommendations.

`Python` `Scikit-learn` `Pandas` `Public Health Analytics`

---

## Background

I came to ML from nursing. That background is useful in ways that don't show up on a skills list — I read clinical data differently, I understand care delivery constraints before they appear in operational data, and I know why a threshold is a clinical decision as much as a statistical one.

Currently building in the insurance and financial services space, alongside continued work in African health systems.

---

## Certifications

- IBM Data Science Professional Certificate
- Clinical Data Science Certificate — University of Colorado
- Registered Nurse Certificate

---

*Open to ML engineering roles in insurance, financial services, and HealthTech — based in Accra, Ghana.*

> *"So built we the wall... for the people had a mind to work."* — Nehemiah 4:6
