# Data Analytics — Level 1, Task 3: Cleaning Data

**Intern:** Yogitha
**Track:** Data Analytics
**Task:** Level 1 — Task 3 — Cleaning Data

## Objective
Take a deliberately messy dataset and systematically transform it into a clean, analysis-ready dataset, documenting every decision along the way.

## Tech Stack
Python, pandas, numpy, Jupyter Notebook

## Files
- `messy_customer_data.csv` — the raw, intentionally messy dataset (520 rows: nulls, duplicates, inconsistent text casing, mixed date formats, wrong dtypes, outliers, negative values).
- `Data_Cleaning.ipynb` — full cleaning notebook, already executed.
- `Data_Cleaning_preview.html` — open in any browser to view without Jupyter.
- `cleaned_customer_data.csv` — the final cleaned output produced by the notebook.

## What's in the notebook
1. Data quality report (nulls, duplicates, dtype issues) — before cleaning
2. Missing value handling — median for numeric columns, mode for categorical, each justified
3. Duplicate row removal (with count of rows removed)
4. Standardising inconsistent text (Gender, City casing) and date formats
5. Outlier detection via IQR method, with documented cap/correct decisions
6. Data type correction (Age → int, JoinDate → datetime, etc.)
7. Before vs. after summary table
8. Save cleaned dataset to CSV

## How to run
```bash
pip install pandas numpy jupyter
jupyter notebook Data_Cleaning.ipynb
```

## Key Decisions
- Numeric columns (Age, Salary, PurchaseAmount) were imputed with the **median** — robust to outliers, unlike the mean.
- Categorical columns (Gender, City) were imputed with the **mode**.
- Salary outliers were **capped** (Winsorized) at IQR bounds rather than dropped, preserving valid rows.
- Negative PurchaseAmount values were corrected via absolute value, treated as sign entry errors rather than true outliers.
