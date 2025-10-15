# Financial ROI Prediction - Azure Data Analysis Demo

[![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)](https://www.python.org/)
[![Azure](https://img.shields.io/badge/Microsoft%20Azure-Integration-blue?logo=microsoft-azure)](https://azure.microsoft.com/)
[![Looker Studio](https://img.shields.io/badge/Looker%20Studio-Dashboard-blue?logo=looker&logoColor=white)](https://lookerstudio.google.com/)

> **Business Analytics Demo Project**  
> Predicting **Revenue and ROI** using multiple regression and model evaluation techniques.  
> The project includes **data cleaning, feature engineering**, and **Azure integration** for a modern data workflow.

---

## Overview

This repository presents a **data analysis demo** that predicts **monthly income and return on investment (ROI)** based on different business and operational factors.  
The goal is to simulate how a company can use **machine learning** and **data visualization** to support better financial decisions.

The pipeline includes:
- Data preparation and feature engineering  
- Regression modeling (Linear and Ridge)  
- Model evaluation (MSE, R², Grid Search)  
- Integration with Azure and Power BI  

---

## Business Problem

A service company wants to estimate its **next-month income and ROI** using several key metrics:
- Marketing investment  
- Number of active clients  
- Customer churn rate  
- Exchange rate (USD/ARS)  
- Operational costs  

The main objectives are:
1. Identify which variables have the highest impact on ROI.  
2. Build a **multiple regression model** to predict future performance.  
3. Improve model generalization using **Ridge Regression** and **Grid Search**.  

---

## ⚙️ Workflow

```mermaid
graph LR
A[Data Sources] --> B[ETL in Python]
B --> C[Feature Engineering]
C --> D[Regression Modeling]
D --> E[Model Evaluation]
E --> F[Power BI Dashboard]
C --> G[Azure Storage]
