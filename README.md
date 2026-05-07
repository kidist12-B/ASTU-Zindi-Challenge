# East African Financial Inclusion Prediction

Machine learning solution for predicting whether an individual owns a bank account using ensemble learning and stacking models.

---

# Project Overview

This project was developed for the **East African Financial Inclusion Challenge**.

The objective is to predict:

- `1` → Individual has a bank account
- `0` → Individual does not have a bank account

The solution combines:
- Feature engineering
- Hyperparameter optimization
- Ensemble learning
- Model stacking
- Threshold optimization

---

# Models Used

The project uses an ensemble of:

- CatBoostClassifier
- XGBoostClassifier
- LightGBMClassifier

Final predictions are stacked using:

- Logistic Regression (Meta Model)

---

# Features Engineering

Custom engineered features include:

| Feature | Description |
|---|---|
| `is_stable` | Indicates stable household structure |
| `edu_job_interaction` | Combines education and job type |
| `household_pressure` | Household size relative to age |
| `edu_score` | Numerical encoding of education level |

Additional preprocessing:
- Missing value handling
- Age clipping
- Categorical processing

---

# Project Structure

```bash
├── Train.csv
├── Test.csv
├── main.py
├── final_submission.csv
└── README.md
