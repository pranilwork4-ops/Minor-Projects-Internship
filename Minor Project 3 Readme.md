# Diabetes Prediction Using Logistic Regression

## Project Overview
This minor project uses **Logistic Regression** to predict the diabetes outcome in the Pima Indians Diabetes dataset. It demonstrates a basic machine-learning workflow, including data inspection, preprocessing, model training, and evaluation.

> **Disclaimer:** This project is for educational purposes only. It is not a medical diagnostic tool and must not be used to make healthcare decisions.

## Dataset
- **Dataset:** Pima Indians Diabetes Database
- **File:** `diabetes.csv`
- **Records:** 768
- **Columns:** 9

### Features
The model uses these eight input features:
- `Pregnancies`
- `Glucose`
- `BloodPressure`
- `SkinThickness`
- `Insulin`
- `BMI`
- `DiabetesPedigreeFunction`
- `Age`

**Target column:** `Outcome`
- `0` = No diabetes
- `1` = Diabetes

Dataset source: [Kaggle — Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)

## Tools and Libraries
- Python
- Google Colab / Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Project Workflow
1. Load and inspect the dataset.
2. Check data types, missing values, duplicate rows, and outcome distribution.
3. Treat zero values in `Glucose`, `BloodPressure`, `SkinThickness`, `Insulin`, and `BMI` as missing measurements.
4. Split the data into training and testing sets using an 80:20 split with stratification.
5. Use median imputation to handle missing measurements.
6. Standardize features using `StandardScaler`.
7. Train a Logistic Regression model with `class_weight="balanced"`.
8. Evaluate the model using classification metrics and plots.

Preprocessing is performed in a Scikit-learn pipeline so that imputation and scaling are fitted using the training data.

## Model Evaluation
The notebook evaluates the model using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion matrix
- ROC curve

**Add your actual results here after running the notebook:**

| Metric | Result |
|---|---|
| Accuracy | Add result |
| Precision | Add result |
| Recall | Add result |
| F1-score | Add result |
| ROC-AUC | Add result |

## Repository Contents
A suggested repository structure is:

```text
Diabetes-Prediction-Logistic-Regression/
├── README.md
├── diabetes.csv
├── diabetes_prediction.ipynb
└── Diabetes_Prediction_Logistic_Regression_Minor_Project_Report.pdf
```

Your filenames may differ. Include the dataset only if you are allowed to redistribute it; otherwise, download it from the Kaggle source linked above.

## How to Run
1. Download or clone this repository.
2. Open the notebook in Google Colab or Jupyter Notebook.
3. If the dataset is not included, download `diabetes.csv` from the Kaggle link above and upload it to the notebook environment.
4. Run the notebook cells from top to bottom.
5. Review the printed evaluation metrics and plots.

## Key Learning Outcomes
- Understanding a binary classification problem.
- Cleaning and preparing tabular data.
- Using a train-test split and a preprocessing pipeline.
- Training a Logistic Regression classifier.
- Interpreting classification metrics and a confusion matrix.

## Limitations
- The dataset is relatively small and represents a specific population.
- Results may not generalize to other populations.
- The model identifies statistical patterns and does not establish a medical diagnosis.

## References
1. [Pima Indians Diabetes Database — Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
2. [Pandas Documentation](https://pandas.pydata.org/docs/)
3. [NumPy Documentation](https://numpy.org/doc/)
4. [Scikit-learn Documentation](https://scikit-learn.org/stable/)
5. [Matplotlib Documentation](https://matplotlib.org/stable/)

---

**Project:** Diabetes Prediction Using Logistic Regression  
**Type:** Internship / Minor Project  
**Author:** Pranil Shirsath
