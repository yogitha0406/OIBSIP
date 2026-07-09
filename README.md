# Data Analytics — Level 2, Task 2: Wine Quality Prediction

**Intern:** Yogitha
**Track:** Data Analytics
**Task:** Level 2 — Task 2 — Wine Quality Prediction

## Objective
Train and compare multiple classification models to predict wine quality based on physicochemical properties such as acidity, density, and alcohol content.

## Tech Stack
Python, pandas, numpy, scikit-learn (Random Forest, SGD, SVC), seaborn, matplotlib, Jupyter Notebook

## Files
- `wine_quality.csv` — 900 synthetic wine samples with 11 chemical features and a quality score (3-8).
- `Wine_Quality_Prediction.ipynb` — full classification notebook, already executed.
- `Wine_Quality_Prediction_preview.html` — open in any browser to view without Jupyter.

## What's in the notebook
1. Class distribution inspection
2. EDA: feature distributions, correlation heatmap
3. Class imbalance discussion
4. Feature engineering: binning quality into Low/Medium/High
5. Stratified train/test split
6. Training 3 classifiers: Random Forest, SGD, SVC
7. Confusion matrices for all 3 models
8. Random Forest feature importance chart
9. Model comparison table
10. Conclusion on best model for deployment

## How to run
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
jupyter notebook Wine_Quality_Prediction.ipynb
```

## Key Insights
- `alcohol` and `volatile_acidity` are the most influential features in predicting wine quality.
- Binning the 6 raw quality scores into Low/Medium/High classes reduces the impact of severe class imbalance.
- **Random Forest** is the recommended model for deployment: strongest accuracy plus interpretable feature importances.
