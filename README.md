# Learning Naive Bayes

Two Gaussian Naive Bayes classification examples implemented in one Jupyter notebook.

## Contents

- `learning_naive_bayes.ipynb`: classifies Iris species from the built-in scikit-learn dataset.
- The same notebook predicts lunch/dinner (`time`) from the Seaborn tips dataset after encoding categorical features.
- Both examples split data into training and test sets and display accuracy, confusion matrices, and classification reports.

## Run locally

Use Python 3 and run Jupyter from the repository directory.

```bash
git clone https://github.com/Sanskar1314/Learning_Naive_Bayes.git
cd Learning_Naive_Bayes
python -m venv .venv
source .venv/bin/activate
python -m pip install jupyterlab numpy pandas seaborn scikit-learn
jupyter lab
```

On Windows, activate the environment with `.venv\Scripts\activate`. Open the notebook listed above and run its cells in order. Results and visualizations appear in the notebook.

## Reproduction notes

Iris is included with scikit-learn. Seaborn may download the tips dataset on first use. Some metric calls pass predictions before true labels; use `classification_report(y_test, y_pred)` and `confusion_matrix(y_test, y_pred)` when interpreting per-class results.
