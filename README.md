# Diabetes Prediction Classification using Machine Learning 

Classifying individuals as diabetic or non-diabetic using health and demographic data.

## Framework

Following the standard 6-step ML framework:
1. Problem Definition
2. Data
3. Evaluation
4. Features
5. Modelling
6. Experimentation

## 1. Problem Definition

The goal is to use machine learning algorithms to classify individuals as diabetic or non-diabetic.

## 2. Data

A detailed dataset comprising health and demographic data of 100,000 individuals, aimed at facilitating diabetes-related research and predictive modeling.

- Source: [Diabetes Clinical Dataset (100k rows), Kaggle](https://www.kaggle.com/datasets/ziya07/diabetes-clinical-dataset100k-rows)

## 3. Evaluation

Since this is a classification problem, the model will be evaluated based on **mean accuracy**, **precision**, **recall**, **f1-score**, **AUC (ROC curve)**, **confusion matrix**, and **classification report**.

**Evaluation goal:** _fill in — e.g. a target accuracy or recall threshold that would make this model a useful proof-of-concept._

## 4. Features

This dataset comprises 100,000 entries, each representing an individual's health and demographic data pertinent to diabetes research. The dataset includes 16 columns:

1. `year`
2. `gender`
3. `age`
4. `location`
5. `race:AfricanAmerican`
6. `race:Asian`
7. `race:Caucasian`
8. `race:Hispanic`
9. `race:Other`
10. `hypertension`
11. `heart_disease`
12. `smoking_history`
13. `bmi`
14. `hbA1c_level`
15. `blood_glucose_level`
16. **`diabetes`** (target attribute / label)
17. `clinical_notes`

> **Note:** The raw dataset CSV is not tracked in this repository (see `.gitignore`). Download it separately from the Kaggle link above and place it in a local `data/` folder to reproduce this project.

## 5. Modelling

- Train/test split (before any preprocessing decisions, to avoid data leakage)
- Preprocessing — encode categorical features (`gender`, `location`, `smoking_history`), handle the one-hot-encoded `race:*` columns, consider whether `clinical_notes` (likely free text) needs NLP-style handling or should be dropped
- Baseline model comparison (e.g. Logistic Regression, Random Forest, KNN)
- Hyperparameter tuning on the best-performing baseline

## 6. Experimentation

| Metric | Score |
|--------|-------|
| Accuracy |  |
| Precision |  |
| Recall |  |
| F1 |  |
| AUC (ROC) |  |

## Project Structure

```
.
├── README.md
├── .gitignore
├── diabetes-prediction-classification.ipynb   # main notebook
└── data/                                       # (not tracked in git — download separately)
```

## Tools & Libraries

- Python
- pandas, NumPy
- scikit-learn (classification models)
- Matplotlib / Seaborn (visualization)
- Jupyter Notebook
