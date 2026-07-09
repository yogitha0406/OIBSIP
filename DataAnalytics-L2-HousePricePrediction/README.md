# Data Analytics — Level 2, Task 1: Predicting House Prices with Linear Regression

**Intern:** Yogitha
**Track:** Data Analytics
**Task:** Level 2 — Task 1 — Predicting House Prices with Linear Regression

## Objective
Build and evaluate a linear regression model that predicts house prices based on area, location, number of rooms, and age.

## Tech Stack
Python, pandas, scikit-learn, matplotlib, seaborn, Jupyter Notebook

## Files
- `house_prices.csv` — 700 synthetic house records (Area, Bedrooms, Bathrooms, Age, Location, Price).
- `House_Price_Prediction.ipynb` — full regression notebook, already executed.
- `House_Price_Prediction_preview.html` — open in any browser to view without Jupyter.

## What's in the notebook
1. EDA: nulls, stats, target distribution
2. Feature selection discussion
3. Missing value handling + One-Hot Encoding of Location
4. Correlation heatmap vs. Price
5. Train/test split (80/20)
6. Linear Regression training
7. Evaluation: MSE, RMSE, R²
8. Actual vs. Predicted scatter plot
9. Residual plot
10. Coefficient analysis
11. Bonus: Ridge & Lasso comparison

## How to run
```bash
pip install pandas scikit-learn matplotlib seaborn jupyter
jupyter notebook House_Price_Prediction.ipynb
```

## Results
- **R² ≈ 0.93** on the test set — the model explains ~93% of price variance.
- **RMSE ≈ $22,300**, a reasonably tight margin given price ranges of $50k-$700k+.
- `Area_sqft` is the strongest positive driver of price; `Age_years` has a negative coefficient, as expected.
- Ridge/Lasso regularisation perform nearly identically to plain Linear Regression here, since multicollinearity between features is low.
