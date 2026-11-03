# Machine Learning Projects

This repository contains Jupyter notebooks demonstrating several machine learning classifiers on the Titanic dataset, plus a linear regression project for predicting medical insurance charges.

## Projects

| Directory | Project |
|---|---|
| `Decision_Tree/` | Decision tree classification of Titanic passenger survival |
| `KNN/` | K-nearest neighbors classification of Titanic passenger survival |
| `Logistic_Regression/` | Logistic regression classification of Titanic passenger survival |
| `Naive_Bayes/` | Gaussian Naive Bayes classification of Titanic passenger survival |
| `Support_Vector_Machine/` | Support vector classification of Titanic passenger survival |
| `Linear_Regression/` | Medical insurance charge prediction using linear regression |

Each project directory contains its own README with details and instructions for running its notebook. The insurance regression notebook and dataset are also available at `Logistic_Regression/Machine_Learning/Linear_Regression/`.

## Requirements

The notebooks use Python with Jupyter, NumPy, pandas, seaborn, matplotlib, and scikit-learn. The insurance regression notebook also uses SciPy.

```bash
python -m pip install jupyter numpy pandas seaborn matplotlib scipy scikit-learn
jupyter notebook
```

Open the notebook in the project directory you want to explore and run its cells in order. The Titanic notebooks load their data using `sns.load_dataset('titanic')`, which may require an internet connection the first time. The insurance notebook reads `insurance.csv` using a relative path, so run it with its directory as the notebook's working directory.
