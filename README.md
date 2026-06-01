# Extreme Streamflow Event Classification Using Temporal Features

This project investigates the role of temporal dependencies in extreme streamflow event classification using daily hydro-meteorological observations and machine learning techniques.

Extreme events are defined using a percentile-based threshold ((Q_{90})) and formulated as a binary classification problem. The study focuses on understanding how temporal feature design, lookback windows, and aggregated hydro-meteorological information affect model performance.

## Implemented Models

* Logistic Regression
* Random Forest
* XGBoost
* LightGBM
* Long Short-Term Memory (LSTM)

## Implemented Analyses

* Data preprocessing
* Lag-based feature engineering
* Aggregated precipitation features
* Baseline model comparison
* Lookback window ablation study
* Feature set ablation study
* Threshold sensitivity analysis ((Q_{90}) vs (Q_{95}))
* SHAP explainability analysis
* Error-event analysis
* ROC Curve evaluation
* Precision-Recall Curve evaluation

## Key Findings

* Medium-term temporal context significantly improves predictive performance.
* Aggregated precipitation features provide substantial performance gains.
* XGBoost achieved the strongest overall performance.
* SHAP analysis identified antecedent streamflow and cumulative precipitation as the most influential predictors.
* Results suggest the presence of catchment memory effects, where antecedent hydrological conditions influence flood predictability over multiple days.

## Repository Structure

* `notebooks/` – Data preprocessing, modeling, and experiments
* `figures/` – Generated plots and visualizations
* `report/` – LaTeX report and presentation materials

## Requirements

```bash
pip install -r requirements.txt
```


