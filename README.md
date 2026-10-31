# Medical Insurance Cost Prediction

This repository contains a Jupyter notebook exploring and predicting individual medical insurance charges with linear regression. The analysis and model are in `Linear_Regression/Untitled.ipynb`; the notebook uses the `insurance.csv` dataset in the same directory.

## Project structure

```text
Machine_Learning/
├── README.md
└── Linear_Regression/
    ├── Untitled.ipynb
    └── insurance.csv
```

The dataset has 1,338 records and these columns: `age`, `sex`, `bmi`, `children`, `smoker`, `region`, and `charges`. The model predicts `charges`.

## Run the notebook

From the repository root, install the notebook dependencies and launch Jupyter:

```bash
python -m pip install jupyter numpy pandas seaborn matplotlib scipy scikit-learn
jupyter notebook
```

Open `Linear_Regression/Untitled.ipynb` and run its cells in order. The notebook reads `insurance.csv` using a relative path, so set the notebook's working directory to `Linear_Regression` if your Jupyter setup does not do so automatically.

## Analysis and modeling

The notebook:

1. Explores the data with summary statistics, missing-value checks, plots, and numeric correlations.
2. Removes duplicate rows; encodes sex and smoking status; one-hot encodes region; and creates BMI categories.
3. Standardizes age, BMI, and number of children, then explores feature associations using Pearson correlation and chi-square tests.
4. Trains a scikit-learn `LinearRegression` model using an 80/20 train-test split (`random_state=42`).
5. Reports R² and adjusted R² on the held-out test data.

The final model uses age, sex, BMI, children, smoking status, and the obese BMI indicator as predictors. The notebook fits the scaler before splitting the data, so test-set information contributes to the scaling parameters; fitting preprocessing on training data only would avoid this data leakage.
