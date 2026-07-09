# Data Analytics — Level 2, Task 3: Fraud Detection

**Intern:** Yogitha
**Track:** Data Analytics
**Task:** Level 2 — Task 3 — Fraud Detection

## Objective
Build a machine learning pipeline to detect fraudulent financial transactions from a heavily imbalanced dataset, addressing class imbalance as a core challenge.

## Tech Stack
Python, pandas, scikit-learn, imbalanced-learn (SMOTE), matplotlib, seaborn, Jupyter Notebook

## Files
- `credit_card_transactions.csv` — 4,620 synthetic transactions with a realistic 2.6% fraud rate.
- `Fraud_Detection.ipynb` — full pipeline notebook, already executed.
- `Fraud_Detection_preview.html` — open in any browser to view without Jupyter.

## What's in the notebook
1. Class imbalance analysis (fraud % of total)
2. EDA: transaction amount & hour patterns, fraud vs. legit
3. Discussion: why accuracy is misleading for imbalanced fraud data
4. SMOTE oversampling to handle imbalance
5. Training Logistic Regression + Random Forest
6. Evaluation: Precision, Recall, F1, AUC-ROC (not just accuracy)
7. ROC curve comparison
8. Confusion matrices
9. Discussion: Recall vs. Precision trade-off for fraud
10. Random Forest feature importance
11. Scalability discussion (handling 1M transactions/hour)

## How to run
```bash
pip install pandas scikit-learn imbalanced-learn matplotlib seaborn jupyter
jupyter notebook Fraud_Detection.ipynb
```

## Key Insights
- Fraudulent transactions typically involve larger amounts, occur more at odd hours, and happen further from home.
- Random Forest generally achieves a stronger AUC-ROC after SMOTE resampling.
- **Recall** is prioritized over Precision in fraud detection, since a missed fraud case is costlier than a false alarm.
- Production deployment at scale would need a streaming feature pipeline and periodic retraining to handle concept drift.
