# XAI-IDS: Explainable AI-based Intrusion Detection Framework

This repository contains the official implementation of our two-stage **XAI-based IDS framework** as described in the paper:

B. Nugraha, A. V. Jnanashree and T. Bauschert, "An Efficient Explainable Artificial Intelligence (XAI)-Based Framework for a Robust and Explainable IDS," 2024 8th Cyber Security in Networking Conference (CSNet), Paris, France, 2024, pp. 173-181, doi: 10.1109/CSNet64211.2024.10851760.

Our framework integrates:
- **ANOVA** statistical feature selection
- **SHAP (SHapley Additive exPlanations)** for model-aware feature importance
- **LIME (Local Interpretable Model-Agnostic Explanations)** for cross-validating local explanations

It is designed to improve **interpretability**, **robustness**, and **efficiency** of intrusion detection models.

## Features

- **Two-stage Feature Reduction**: Combines ANOVA F-values and SHAP global importance (weighted 40% ANOVA, 60% SHAP) to select the top 10 most relevant features.
- **High Accuracy with Efficiency**: Reduces LIME explanation time by up to **87%** while sustaining F1 ≥ 99%.
- **Cross-method Validation**: Ensures consistency between SHAP and LIME local explanations.
- **Multiple Dataset Support**:
  - CIC-DDoS2019 (Portmap, SYN Flood, HTTP Flood, Slowloris)
  - CICIoT2023
  - 5G PFCP control-plane attacks
