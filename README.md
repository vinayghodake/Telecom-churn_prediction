<div align="center">

# 📡 Telecom Churn Predictor

### Turning customer data into signals that can help explain who may leave.

A Jupyter notebook exploring telecom customer churn through data cleaning, visual analysis, feature engineering, and machine learning.

![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?logo=python&logoColor=white)
![Notebook](https://img.shields.io/badge/Format-Jupyter-F37626?logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Project-Learning%20%26%20Analysis-7C3AED)

</div>

---

## ✨ What this project does

This project uses customer information—such as tenure, subscribed services, contract type, and charges—to study the patterns associated with **churn**. It then trains classification models to predict the notebook's `Churn` target and compares their results.

> **Goal:** explore how customer and service characteristics relate to churn and practice a complete machine learning workflow.

## 🔎 Inside the notebook

| Stage | What happens |
| --- | --- |
| **Explore** | Inspect customer records and compare churn patterns with tables and charts. |
| **Prepare** | Clean Yes/No fields, convert charge values, and remove the customer ID. |
| **Create features** | Derive service-count features from protection and streaming subscriptions. |
| **Train** | Split data into training and test sets; scale numeric features and encode categories. |
| **Evaluate** | Fit Logistic Regression and SGDClassifier models and review classification metrics, ROC-AUC, and accuracy. |

## 📁 Files

```text
Telecom_churn_predictor/
├── Telecom churn predictor.ipynb
├── WA_Fn-UseC_-Telco-Customer-Churn.csv
└── README.md
```

Keep the CSV beside the notebook for the simplest setup. If you use a different location, update the notebook's `pd.read_csv(...)` path.

## 🚀 Get started

### 1. Install the packages

Python 3.9 or later is recommended. From a terminal, run:

```bash
python -m pip install pandas numpy matplotlib seaborn plotly scikit-learn jupyter
```

### 2. Open the project folder

Place the notebook and CSV in one folder, then open a terminal in that folder and start Jupyter:

```bash
jupyter notebook
```

Open **Telecom churn predictor.ipynb** in the browser.

### 3. Use a relative dataset path

In the notebook's data-loading cell, use:

```python
import pandas as pd

df = pd.read_csv("WA_Fn-UseC_-Telco-Customer-Churn.csv")
```

### 4. Run the analysis

Run the notebook cells from top to bottom to reproduce the data preparation, visualizations, model training, and evaluation.

## 📊 Dataset

The notebook expects a Telco Customer Churn CSV with customer, service, contract, payment, charge, and churn fields. The expected filename is `WA_Fn-UseC_-Telco-Customer-Churn.csv`.

If you publish this repository, check the dataset's source and usage terms before uploading the CSV. If you cannot redistribute it, leave the data file out and add instructions for obtaining it.

## 🧰 Tools used

`Python` · `pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Plotly` · `scikit-learn` · `Jupyter`

## 📝 Notes

- The notebook is an educational analysis, not a deployed prediction service.
- The train/test split does not specify a fixed random seed, so results may differ between runs.
- Churn predictions are exploratory and should not be treated as guarantees about individual customers.

---

<div align="center">

**Built as a hands-on machine learning project** · If you found it useful, consider giving the repository a ⭐

</div>
