# Portfolio
AbderrazakRaouah.github.io
# Housing Price Analysis (Python)

A small end-to-end project to analyze and model housing prices.

## Project Structure
```
housing-price-project/
├─ data/
│  └─ housing.csv
├─ src/
│  └─ analyze_housing.py
├─ figures/   # generated charts
├─ models/    # saved pipelines + metrics
└─ README.md
```

## What you'll learn
- Exploratory data analysis (EDA): distributions, correlations, group comparisons
- Feature engineering & preprocessing (scaling + one-hot encoding)
- Regression modeling with **Linear Regression** and **Random Forest**
- Evaluation metrics: **MAE**, **RMSE**, **R²**
- Saving models and feature importance plots

## Quick Start
```bash
# 1) (optional) create & activate a virtual environment
python -m venv .venv
# macOS/Linux
source .venv/bin/activate
# Windows (PowerShell)
# .venv\Scripts\Activate.ps1

# 2) Install dependencies
pip install pandas numpy seaborn matplotlib scikit-learn joblib

# 3) Run the analysis
python src/analyze_housing.py
```

## Outputs
- `figures/01_price_distribution.png` – histogram of prices
- `figures/02_price_vs_sqft.png` – scatter of price vs square footage
- `figures/03_corr_heatmap.png` – correlation heatmap (numerics)
- `figures/04_price_by_renovation.png` – boxplot by renovation flag
- `figures/05_mean_price_by_neighborhood.png` – mean price bar chart
- `figures/06_rf_feature_importance.png` – top features from RF
- `models/metrics.json` – MAE, RMSE, R² for each model
- `models/*.joblib` – trained pipelines you can reuse

## Ideas to Extend
- Add **regularization** (Ridge/Lasso), **XGBoost/LightGBM**
- Hyperparameter tuning with `GridSearchCV`
- Cross-validation and learning curves
- SHAP for model explainability
- Geo-visualizations (if you add lat/long)

## Notes
- Dataset is **synthetic** for learning purposes.
- You can swap `data/housing.csv` with a real dataset (e.g., your local market), keeping the same script.
