# Linear Regression: Medical Insurance Costs

This directory contains a Jupyter notebook that explores medical insurance data and trains a linear regression model to predict insurance charges.

## Files

- `Untitled.ipynb` — data exploration, preprocessing, feature analysis, and model evaluation.
- `insurance.csv` — 1,338 records with age, sex, BMI, children, smoking status, region, and charges.

## Run the notebook

Install the required packages and launch Jupyter from this directory:

```bash
python -m pip install jupyter numpy pandas seaborn matplotlib scipy scikit-learn
jupyter notebook
```

Open `Untitled.ipynb` and run the cells in order. It reads `insurance.csv` using a relative path, so the notebook's working directory should be this directory.

The notebook preprocesses the data, explores feature associations, and evaluates a `LinearRegression` model with an 80/20 train-test split (`random_state=42`). The scaler is currently fit before splitting; fitting preprocessing only on training data would prevent test-set information from influencing scaling.
