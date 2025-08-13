This repository contains the notebook **`XAI-IDS-TUC.ipynb`** for the paper *“A Versatile XAI-based Framework for Efficient and Explainable Intrusion Detection Systems.”*  
It demonstrates an end‑to‑end workflow for tabular IDS data using:
- **XGBoost** as the classifier
- **Feature selection** via **ANOVA Top‑K**, **SHAP Top‑K**, and a **combined Top‑K**
- **Ablation** with **PCA**
- **Explainability** with **SHAP** (global) and **LIME** (local) including basic **timing** measurements

## Contents
- Data loading and preprocessing (encoding + scaling)
- Model training with XGBoost
- Top‑K feature selection with ANOVA / SHAP / Combined
- PCA ablation (optional)
- Explanations using SHAP and LIME
- Evaluation (accuracy, recall, F1, confusion matrix)
