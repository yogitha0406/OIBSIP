# Data Analytics — Level 1, Task 1: EDA on Retail Sales Data

**Intern:** [Your Full Name]
**Track:** Data Analytics
**Task:** Level 1 — Task 1 — Exploratory Data Analysis on Retail Sales Data

## Objective
Perform a thorough Exploratory Data Analysis on a retail sales dataset to uncover patterns, customer behaviour trends, and actionable business insights.

## Tech Stack
Python, pandas, matplotlib, seaborn, Jupyter Notebook

## Dataset
`retail_sales_dataset.csv` — 1,200 transaction-level retail records with columns:
`Transaction ID, Date, Customer ID, Gender, Age, Product Category, Product Name, Quantity, Price per Unit, Total Amount, Region`.

> Note: replace this file with a dataset of your choice from Kaggle (search "retail sales dataset", "superstore sales") if you'd like to run the analysis on real-world data instead — the notebook code will work with any dataset that has the same column names.

## What's in this notebook (`EDA_Retail_Sales.ipynb`)
1. Data load + initial inspection (shape, dtypes, nulls, duplicates)
2. Descriptive statistics (mean, median, mode, std)
3. Monthly & quarterly sales trend line charts
4. Customer demographics: age group distribution, gender breakdown
5. Product analysis: top 10 best-sellers, revenue by category
6. Correlation heatmap of numerical variables
7. Additional insight: regional revenue vs. average order value
8. Markdown commentary after every chart
9. Conclusion with 3 actionable business recommendations

## How to run
```bash
pip install pandas matplotlib seaborn jupyter
jupyter notebook EDA_Retail_Sales.ipynb
```

## Key Insights
- Electronics drives disproportionate revenue relative to its unit volume.
- The 26–35 age band is the largest customer segment.
- Regions differ in whether they are volume-driven or value-driven, which should inform different marketing tactics.

## Business Recommendations
1. Bundle accessories with high-ticket Electronics items to raise average order value.
2. Focus core campaigns on the 26–35 age segment while running growth campaigns for under-represented groups.
3. Apply region-specific strategy: volume promotions where order count is high, premium upsell where average order value is high.
