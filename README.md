# Insurance Premium Prediction

Predicting annual medical insurance premiums for new applicants with sklearn and XGBoost.

## What it does

Regression models that predict a new applicant's annual insurance premium using only information known at signup (demographics, lifestyle, vitals, medical history, chosen plan). Claims and utilization data are excluded on purpose to avoid leakage.

## Files

- `insurance_premium_prediction.ipynb`

## Tools

pandas, numpy, scikit-learn, XGBoost, SHAP, matplotlib, seaborn, kagglehub

## Dataset

[Medical Insurance Cost Prediction (Kaggle)](https://www.kaggle.com/datasets/mohankrishnathalla/medical-insurance-cost-prediction)

The dataset is not included in this repo.

## Results

From the saved notebook outputs:

Linear Regression: RMSE 357.35, MAE 218.61, R2 0.198 | Random Forest: RMSE 360.86, R2 0.182 | XGBoost: RMSE 359.01, R2 0.190. The signup-only feature set gives modest explained variance, as expected without claims history.

## How to run

1. Open the notebook in Google Colab or Jupyter.
2. Install dependencies: `pip install -r requirements.txt`.
3. Download the dataset from the link above (some notebooks fetch it with `kagglehub`, which asks for Kaggle credentials) and update the data path if needed.
4. Run all cells.

## Author

Mark Ayman
