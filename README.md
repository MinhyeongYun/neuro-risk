# Computational Psychiatry Prototype: Modeling Latent Cognitive Mechanisms of Risk

## Overview

This project is a computational psychiatry prototype designed to model **latent cognitive mechanisms underlying psychiatric risk** using synthetic longitudinal data.

Rather than focusing solely on prediction, the project aims to simulate how **hidden vulnerability, dynamic state changes, and decision-related processes** interact over time to generate observable risk.

This is not a clinical tool, but a research-oriented demonstration of **mechanistic modeling in computational psychiatry**.

The goal is to demonstrate how computational psychiatry approaches can be applied to simulate and predict mental health risk in dynamic, real-world-like settings.

This is **not a clinical tool**, but a methodological demonstration.

---

## Research Motivation

Psychiatric risk emerges from underlying cognitive processes such as:
- reward learning
- belief updating
- uncertainty processing

However, most real-world systems rely on static, symptom-based approaches that fail to capture these mechanisms.

This project explores how **latent cognitive processes evolve over time** and contribute to psychiatric risk, using a computational modeling framework.

---

## Key Features

- Simulation of latent vulnerability and dynamic psychiatric states
- Longitudinal modeling of evolving risk trajectories
- Proxy modeling of latent cognitive processes
- Temporal dynamics (instability, drift, change)
- Probabilistic prediction with calibration
- Uncertainty estimation (bootstrap-based)
- Model interpretability and feature attribution

---

### Conceptual Framing

This project follows a computational psychiatry perspective:

Observed variables (stress, sleep, mood)
→ reflect underlying latent states
→ which evolve dynamically over time
→ and generate observable behavior and risk

The model approximates these latent processes through engineered features and probabilistic modeling.

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
