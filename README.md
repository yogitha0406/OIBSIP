# Data Analytics — Level 1, Task 2: Customer Segmentation Analysis

**Intern:** Yogitha
**Track:** Data Analytics
**Task:** Level 1 — Task 2 — Customer Segmentation Analysis

## Objective
Apply clustering algorithms to segment an e-commerce company's customer base into distinct groups based on purchasing behaviour, enabling targeted marketing strategies.

## Tech Stack
Python, pandas, scikit-learn (KMeans), matplotlib, seaborn, Jupyter Notebook

## Files
- `ecommerce_customer_data.csv` — 600 synthetic customers with Recency, Frequency, and Monetary (RFM) values.
- `Customer_Segmentation.ipynb` — full clustering notebook, already executed.
- `Customer_Segmentation_preview.html` — open in any browser to view without Jupyter.

## What's in the notebook
1. Load, clean (nulls + duplicates)
2. Descriptive statistics
3. RFM feature selection
4. Standardisation with `StandardScaler`
5. Elbow Method to choose optimal K
6. K-Means clustering (K=4)
7. Cluster visualisation (2 feature-pair scatter plots)
8. Cluster profiling (mean RFM values per cluster)
9. Customers-per-cluster bar chart
10. Marketing recommendations per segment

## How to run
```bash
pip install pandas scikit-learn matplotlib seaborn jupyter
jupyter notebook Customer_Segmentation.ipynb
```

## Key Insights
- Four natural customer segments emerge: high-value "Champions", lapsed big spenders, frequent low-value shoppers, and at-risk/inactive customers.
- Each segment warrants a different marketing action — loyalty rewards, win-back campaigns, bundle upsells, or re-engagement offers respectively.
