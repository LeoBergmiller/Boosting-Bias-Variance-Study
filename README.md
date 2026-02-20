# Boosting Methods & Bias–Variance Tradeoff

Comparative Analysis of how boosting methods improve generalization performance compared to single decision trees on an imbalanced classification task (UCI Bank Marketing dataset).

---

## Overview

This project compares:

- Decision Tree (baseline)
- Gradient Boosting (sklearn)
- XGBoost
- LightGBM

Key focus areas:
- Bias–variance tradeoff
- Training vs validation loss dynamics
- AUC-PR vs ROC-AUC under class imbalance
- Hyperparameter regularization effects

---

## Key Results (Test Set)

| Model | AUC-PR | AUC-ROC |
|-------|--------|---------|
| XGBoost | **0.456** | 0.798 |
| LightGBM | 0.449 | 0.801 |
| Gradient Boosting | 0.445 | 0.792 |
| Decision Tree | 0.388 | 0.756 |

Boosting methods significantly improved ranking quality compared to a single tree baseline.

---

## Why This Matters

- Demonstrates practical bias reduction via additive ensembles
- Shows how shrinkage and subsampling control variance
- Illustrates why AUC-PR is preferred in rare-event prediction
- Includes staged training diagnostics and feature importance analysis

---

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook
