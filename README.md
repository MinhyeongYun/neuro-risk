# Psychiatric Risk Modeling Prototype

## Overview

This project is a research-oriented prototype for modeling **psychiatric risk using synthetic longitudinal data**.

The goal is to demonstrate how computational psychiatry approaches can be applied to simulate and predict mental health risk in dynamic, real-world-like settings.

This is **not a clinical tool**, but a methodological demonstration.

---

## Research Motivation

Psychiatric crises (e.g., suicide risk, acute instability) often occur in real-world environments where decisions must be made under uncertainty.

Current approaches are typically:
- static
- retrospective
- not deployable in real-time

This project explores how **longitudinal modeling + probabilistic prediction** can address this gap.

---

## Key Features

- Synthetic longitudinal psychiatric dataset
- Latent vulnerability modeling
- Temporal feature engineering (trend, instability, change)
- Predictive modeling (logistic regression, ensemble models)
- Model calibration (Brier score, calibration curve)
- Uncertainty estimation (bootstrap)
- Ablation study (feature contribution analysis)
- Model interpretability (permutation importance)

---

## Methods

### Data Generation
- Simulates individuals with latent psychiatric vulnerability
- Models daily evolution of:
  - stress
  - sleep
  - depression
  - anxiety
  - social support

### Modeling
- Logistic regression (baseline & dynamic)
- Random Forest
- Gradient Boosting

### Evaluation
- ROC-AUC
- Brier Score (calibration)
- Precision-Recall
- Confusion Matrix

### Advanced Components
- Bootstrap uncertainty estimation
- Feature ablation study
- Permutation feature importance

---

## How to Run

```bash
pip install numpy pandas scikit-learn matplotlib joblib
python app.py
