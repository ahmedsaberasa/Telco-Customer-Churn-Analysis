# 📡 Telco Customer Churn Analysis

<p align="center">
  <img src="Customer Churn Analysis/images/churn_cover_card.png" alt="Telco Churn Analysis Cover" width="100%"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10-blue?style=flat-square&logo=python" />
  <img src="https://img.shields.io/badge/Scikit--learn-ML-orange?style=flat-square&logo=scikit-learn" />
  <img src="https://img.shields.io/badge/Pandas-EDA-green?style=flat-square&logo=pandas" />
  <img src="https://img.shields.io/badge/Google%20Colab-Notebook-yellow?style=flat-square&logo=google-colab" />
  <img src="https://img.shields.io/badge/Dataset-IBM%20Telco-lightblue?style=flat-square" />
</p>

---

## 📌 Project Overview

An end-to-end machine learning project analyzing customer churn in the telecom industry using the **IBM Telco Customer Churn dataset** (7,043 customers, 21 features).

The goal: identify **why customers leave**, **predict who is at risk**, and build a **data-driven retention strategy** that directly addresses business impact.

> **$2.86M in annual revenue at risk** — a 26.5% churn rate that we can now predict and act on.

---

## 📊 Key Findings

<p align="center">
  <img src="Customer Churn Analysis/images/churn_findings_card.png" alt="Key Churn Drivers" width="100%"/>
</p>

| Risk Factor | Churn Rate |
|---|---|
| Month-to-Month Contract | 42.7% |
| No Online Security | 41.8% |
| Fiber Optic (High Bill) | ~40% |
| Senior Citizens | Elevated |
| Tenure < 12 months | Critical window |

---

## 🤖 Model Results

<p align="center">
  <img src="Customer Churn Analysis/images/model_results_card.png" alt="Model Comparison Results" width="100%"/>
</p>

Four classification models were trained and evaluated:

| Model | Accuracy | ROC-AUC | Notes |
|---|---|---|---|
| Logistic Regression | Baseline | — | Good interpretability |
| Decision Tree | Medium | — | Prone to overfitting |
| Random Forest | High | — | Solid generalization |
| **Gradient Boosting** | **80%** | **0.85** | ✅ Best overall |

> **Gradient Boosting** was selected as the final model based on highest ROC-AUC and best recall on churners (minimizing missed at-risk customers).

---

## 💡 Retention Strategy

<p align="center">
  <img src="Customer Churn Analysis/images/retention_strategy_card.png" alt="Retention Strategy" width="100%"/>
</p>

Based on the analysis, four high-impact interventions were identified:

1. **Lock in early** — Incentivize long-term contracts during the first 12 months (the highest churn window)
2. **Bundle security services** — Customers with Online Security churn significantly less
3. **Reassess Fiber Optic pricing** — Value perception is the issue, not the service quality
4. **Deploy ML model** — Use the Gradient Boosting classifier to proactively flag high-risk customers

---

## 🗂️ Project Structure

```
telco-churn-analysis/
│
├── images/                          # Visualization cards used in README
│   ├── churn_cover_card.png
│   ├── churn_findings_card.png
│   ├── model_results_card.png
│   └── retention_strategy_card.png
│
├── Telco_Churn_Full_Analysis.ipynb  # Main Jupyter notebook (full pipeline)
├── Telco_Churn_Analysis.pptx        # Executive presentation
└── README.md
```

---

## 🔧 Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.10 | Core language |
| Pandas / NumPy | Data manipulation & EDA |
| Matplotlib / Seaborn | Data visualization |
| Scikit-learn | ML modeling & evaluation |
| Google Colab | Development environment |
| IBM Telco Dataset | Source data |

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/telco-churn-analysis.git
cd telco-churn-analysis

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# Open the notebook
jupyter notebook Telco_Churn_Full_Analysis.ipynb
```

Or open directly in **Google Colab**:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1dVOLt-3v2KYFOZdgqTojetT5YuXK1zGn?usp=sharing)

---

## 📁 Dataset

**IBM Sample Data Sets — Telco Customer Churn**
- 7,043 customers
- 21 features (demographics, services, contract type, billing, churn label)
- Available on [Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

---

## 👤 Author

**[Ahmed Saber]**
Data Analyst | ML Enthusiast

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat-square&logo=linkedin)](https://linkedin.com/in/1ahmedsaber)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=flat-square&logo=github)](https://github.com/ahmedsaberasa)

---

*If you found this project useful, feel free to ⭐ star the repo!*
