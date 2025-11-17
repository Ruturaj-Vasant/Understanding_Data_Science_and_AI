# Data Science & AI — Portfolio Notebooks

Curated Jupyter notebooks showcasing coursework, projects, and exploratory analyses. The repository is organized by purpose to help reviewers navigate quickly.

## Structure

- `projects/`: end‑to‑end, outcome‑focused notebooks
  - `Telco_Churn_Prediction.ipynb`
  - `Patient_NoShow_Prediction.ipynb`
- `exploratory/`: data exploration and visualization
  - `Bilateral_Trade_EDA.ipynb`
- `practice/`: practice notebooks
  - `T1_Python_Basics.ipynb`, `T1_Python_Jupyter_Colab.ipynb`, `T4_Decision_Trees.ipynb`, `T4_Fitting_Data_Science_Models.ipynb`, `T5_Model_Assessment.ipynb`, `T5_Model_Complexity_Cross_Validation.ipynb`, `T6_Regression_Regularization_Ames.ipynb`, `T7_Basic_Neural_Networks.ipynb`, `T9_Text_Mining.ipynb`
- `data/` (git‑ignored): place local CSVs used by notebooks here

Expected filenames in `data/` (not included in the repo):
- `telco_churn.csv` (for `projects/Telco_Churn_Prediction.ipynb`)
- `SHMC_NoShows.csv` (for `projects/Patient_NoShow_Prediction.ipynb`)
- `bilateral_trade_clean.csv` (for `exploratory/Bilateral_Trade_EDA.ipynb`)

## What I Learned (One‑Liners)

- projects
  - Telco_Churn_Prediction: Tuned Decision Tree and L1‑Logistic to maximize AUC; applied cost‑aware targeting.
  - Patient_NoShow_Prediction: Engineered features and evaluated classifiers to predict no‑shows for staffing planning.
- exploratory
  - Bilateral_Trade_EDA: Explored trade with pandas/plotly; identified trends, outliers, and country patterns.
- practice
  - T1_Python_Basics: Core Python syntax, data structures, and control flow.
  - T1_Python_Jupyter_Colab: Jupyter/Colab workflows, markdown, magics, and data I/O.
  - T4_Decision_Trees: Decision tree fundamentals and scikit‑learn classification.
  - T4_Fitting_Data_Science_Models: Preprocess → split → fit → evaluate modeling workflow.
  - T5_Model_Assessment: Metrics and validation strategies; bias–variance trade‑off.
  - T5_Model_Complexity_Cross_Validation: Hyperparameter tuning and complexity control via cross‑validation.
  - T6_Regression_Regularization_Ames: Ridge/Lasso on housing data; regularization and scaling effects.
  - T7_Basic_Neural_Networks: Intro feedforward networks; training and evaluation for classification.
  - T9_Text_Mining: Text preprocessing and vectorization (TF‑IDF) with simple classifiers.

## Run Locally

1) Environment
- `python -m venv .venv && source .venv/bin/activate` (macOS/Linux)
- `python -m venv .venv && .venv\\Scripts\\activate` (Windows)
- `pip install -r requirements.txt`

2) Data
- Create a `data/` folder at the repository root (already present) and copy required CSVs there with the expected filenames above.

3) Jupyter
- Start from the repository root so relative paths to `data/` resolve: `jupyter lab` or `jupyter notebook`

## Notes

- Heavy data files and generated outputs are git‑ignored; notebooks are kept light.
- Dependencies are listed in `requirements.txt`.
