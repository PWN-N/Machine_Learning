# Linear Regression: Medical Insurance Costs

This directory contains a Jupyter notebook that analyzes medical insurance data and trains a linear regression model to predict insurance charges.

## Files

- `Untitled.ipynb` — data exploration, preprocessing, statistical analysis, and model training/evaluation.
- `insurance.csv` — dataset with 1,338 records and columns for age, sex, BMI, children, smoking status, region, and charges.

## Run the notebook

Install the required Python packages and launch Jupyter from this directory:

```bash
python -m pip install jupyter numpy pandas seaborn matplotlib scipy scikit-learn
jupyter notebook
```

Open `Untitled.ipynb` and run the cells in order. The notebook reads `insurance.csv` using a relative path, so its working directory should be this directory.

The notebook prepares the data, explores feature associations, and evaluates a `LinearRegression` model using an 80/20 train-test split. Its preprocessing currently fits the scaler before splitting; fitting preprocessing only on the training data would prevent test-set information from influencing the scaling parameters.
