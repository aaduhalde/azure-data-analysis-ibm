# PROJECT_DOCUMENTATION.md  
**Project:** Financial ROI Prediction – Azure Data Analysis Demo  
**Author:** Alejandro Adrián Duhalde  
**Role:** Technical Business Analyst | Data Engineer  

---

## 1. Purpose
This document provides the **functional and technical specification** of the *Financial ROI Prediction* project.  
It describes how the system is structured, the data flow, Azure integration, and the technical steps required to reproduce and maintain the analysis.

---

## 2. Business Context
This demo simulates a financial analytics scenario where a company predicts **monthly revenue and ROI** using operational and market data.  
The purpose is to demonstrate a **data-driven approach** leveraging Azure services, Python-based machine learning, and Looker dashboards.

The project showcases:
- How data preprocessing and regression modeling work together.  
- How to integrate analytics pipelines with cloud storage and visualization tools.  
- How statistical validation (MSE, R²) ensures model reliability.

---

## 3. Functional Requirements

| Category | Description |
|-----------|--------------|
| **Input Data** | CSV files containing marketing, operational, and financial KPIs |
| **Data Sources** | Local dataset (CSV), optionally Azure Blob Storage |
| **Processing** | Cleaning, feature transformation, regression modeling |
| **Output Data** | Model metrics (MSE, R²), plots, CSV with predictions |
| **Visualization** | Looker Studio dashboard connected to output results |
| **Dependencies** | Python 3.10+, pandas, scikit-learn, numpy, matplotlib, Azure SDK |

---

## 4. Technical Architecture

```mermaid
graph TD
    A[Raw Data (CSV or Azure Blob)] --> B[Data Cleaning & Feature Engineering (Python)]
    B --> C[Regression Models (Linear & Ridge)]
    C --> D[Hyperparameter Tuning (Grid Search)]
    D --> E[Model Evaluation (MSE and R2)]
    E --> F[Results Export (CSV and Looker Dashboard)]
    C --> G[Azure Integration (Data Upload / Storage)]
```
