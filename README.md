# 🏥 Medical Insurance Cost Prediction

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat-square&logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-Regression-orange?style=flat-square&logo=scikit-learn)
![R2](https://img.shields.io/badge/R²-0.87%20Random%20Forest-brightgreen?style=flat-square)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)

> Predicting individual medical insurance charges using regression — quantifying financial risk from personal health and demographic attributes.

> **Legacy / Learning Project.** One of my early ML notebooks, kept public as a record of the learning path (classic scikit-learn pipelines, EDA, model comparison). Superseded in portfolio terms by the shipped risk/fraud/governance systems in [Jeevan-0508](https://github.com/Jeevan-0508) — this repo is archived, not deleted.

## 📌 Problem Statement
Accurate insurance cost prediction is critical for premium pricing, underwriting, and financial risk planning. This project builds a regression pipeline estimating annual charges from policyholder attributes.

## 🎯 Key Objectives
- Predict continuous insurance charges (regression)
- Identify the strongest cost-driving risk factors
- Compare linear vs non-linear models
- Quantify each feature's risk contribution

## 🔬 Models Used
| Model | R² Score | Notes |
|-------|----------|-------|
| Linear Regression | 0.74 | Baseline, interpretable |
| Ridge / Lasso | ~0.75 | Regularised, handles multicollinearity |
| Random Forest | **0.87** | Best performer |
| Gradient Boosting | 0.85 | Fine-tuned ensemble |

## 📦 Dataset
`insurance.csv` — 1,338 policyholders × 7 features: age, sex, BMI, children, smoker, region, charges

## 🛠️ Tech Stack
`Python` · `pandas` · `scikit-learn` · `matplotlib` · `seaborn` · `Jupyter`

## 📊 Key Findings
- **Smoking status** explains ~60% of cost variance — single biggest risk factor
- **BMI > 30 + Smoker** → charges 3× the average (super-high-risk segment)
- **Age** shows strong positive linear correlation
- Region alone has minimal impact

## 🚀 Run Locally
```bash
pip install pandas scikit-learn matplotlib seaborn jupyter
jupyter notebook "JK Project9_Medical_Insurance_Cost_Prediction.ipynb"
```

## 🔗 Relevance to Risk Management
Actuarial risk quantification is core to insurance and financial risk. Translating personal attributes into risk scores mirrors credit scoring, fraud risk tiering, and operational risk modelling.

---
*Jeevan Siddhabhaktula · Risk & Data Science Portfolio*
