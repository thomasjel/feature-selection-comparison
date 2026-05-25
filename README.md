# Shallow Learning Classification Pipeline

End-to-end supervised machine learning pipeline focused on:

- feature selection
- model comparison
- hyperparameter optimization
- ensemble methods
- external validation

The project evaluates multiple shallow learning algorithms using biomedical datasets and compares their predictive performance using robust statistical metrics.

---

# Project Objectives

This project was developed to:

- reduce dimensionality
- identify relevant predictive variables
- compare feature selection strategies
- evaluate shallow learning models
- optimize hyperparameters
- analyze model diversity
- evaluate ensemble methods
- study overfitting and model stability

---

# Datasets

Three datasets were used:

| Dataset | Purpose |
|---|---|
| 00-train.csv | Model training |
| 01-tuning.csv | Hyperparameter optimization |
| 02-external.csv | Final external evaluation |

---

# Feature Selection Methods

Two feature selection approaches were implemented:

## Filter Methods
- Mutual Information
- Chi-Squared (χ²)

## Wrapper Methods
- Sequential Forward Selection (SFS)

Subset quality was evaluated using:
- Random Forest
- Cross-validation
- Weighted F1-score

---

# Machine Learning Models

The following shallow learning models were evaluated:

- Logistic Regression
- Support Vector Machine (SVM)
- k-Nearest Neighbors (kNN)
- Random Forest

---

# Hyperparameter Optimization

Grid Search with 5-fold cross-validation was used to optimize:

- Logistic Regression
- SVM
- kNN
- Random Forest

---

# Evaluation Metrics

Models were evaluated using:

- ACC (Accuracy)
- SEN (Sensitivity)
- SPE (Specificity)
- MCC (Matthews Correlation Coefficient)
- F1-score
- Confusion Matrix

---

# Best Results

The best-performing model was:

## Random Forest

| Metric | Value |
|---|---|
| ACC | 0.834 |
| MCC | 0.278 |
| F1 | 0.882 |

The Random Forest model achieved the best overall generalization performance on the external dataset.

---

# Key Findings

- Wrapper methods produced more stable feature subsets.
- Hyperparameter optimization did not always improve model performance.
- Random Forest achieved the best balance between stability and predictive accuracy.
- kNN showed lower robustness on external validation.
- Ensemble-based approaches generalized better than linear models.

---

# Repository Structure

```text
.
├── 00-train.csv
├── 01-tuning.csv
├── 02-external.csv
├── filter_vs_wrapper.ipynb
├── base_model.ipynb
├── hyperparameter_tuning.ipynb
└── README.md
```

---

# Future Work

Possible future improvements include:

- ensemble diversity analysis
- AdaBoost/XGBoost models
- Y-Scrambling
- statistical comparison tests
- feature importance analysis
- SHAP explainability

---

# Author

Tomas Escamilla

Physics Student | Machine Learning | Quantitative Modeling
