# Decision Tree: Titanic Survival

This directory contains a Jupyter notebook that trains a decision tree classifier to predict passenger survival using Seaborn's Titanic dataset.

## Run the notebook

Install the required packages and launch Jupyter:

```bash
python -m pip install jupyter numpy pandas seaborn matplotlib scikit-learn
jupyter notebook
```

Open `Untitled.ipynb` and run the cells in order. The notebook loads the dataset with `sns.load_dataset('titanic')`, so an internet connection may be needed on the first run.

The notebook drops redundant columns, fills missing ages, removes rows without embarkation data, and label-encodes categorical features. It uses an 80/20 train-test split (`random_state=42`), trains a `DecisionTreeClassifier`, and reports accuracy, a confusion matrix, and a classification report.
