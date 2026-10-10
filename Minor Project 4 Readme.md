# Random Forest Classification -- Heart Disease Prediction

## Project Overview

This minor project uses a **Random Forest Classifier** to predict the
presence of heart disease from patient-related health attributes. It
demonstrates a machine-learning classification workflow, including data
preprocessing, exploratory data analysis (EDA), model training, and
evaluation.

> **Disclaimer:** This project is for educational purposes only. It is
> not a medical diagnostic tool and must not be used to make healthcare
> decisions.

## Objectives

-   Explore and understand the Heart Failure Prediction dataset.
-   Clean and preprocess numerical and categorical features.
-   Train a Random Forest classification model.
-   Evaluate model performance using classification metrics.
-   Examine feature importance to understand which input features
    contribute most to the model.

## Dataset

-   **Dataset:** Heart Failure Prediction
-   **Source:** [Kaggle -- Heart Failure
    Prediction](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)
-   **Target column:** `HeartDisease`
    -   `0` --- No Disease
    -   `1` --- Disease

The dataset contains a mix of numerical and categorical patient
attributes. Refer to the original Kaggle dataset page for the full
feature descriptions and dataset terms.

## Technologies Used

-   Python
-   Pandas and NumPy
-   Matplotlib and Seaborn
-   Scikit-learn
-   Jupyter Notebook / Google Colab

## Project Workflow

1.  Load the dataset and inspect its structure.
2.  Check for duplicate records and handle them as required.
3.  Perform exploratory data analysis and visualize feature
    relationships.
4.  Split the data into training and testing sets using a **stratified
    80:20 split**.
5.  Impute missing numerical values using the median and categorical
    values using the most frequent value.
6.  Apply one-hot encoding to categorical features.
7.  Train a `RandomForestClassifier`.
8.  Evaluate the model on the held-out test set.
9.  Visualize the confusion matrix, ROC curve, and feature importance.

### Model Configuration

The model was configured with the following parameters:

``` python
RandomForestClassifier(
    n_estimators=200,
    max_depth=10,
    random_state=42,
    class_weight="balanced"
)
```

Preprocessing is fitted using the training data to avoid data leakage.
Standard scaling is not required for this tree-based model.

## Results

The reported test-set evaluation metrics are:

  Metric         Score
  ----------- --------
  Accuracy      90.76%
  Precision     89.72%
  Recall        94.12%
  F1-score      91.87%
  ROC-AUC       93.41%

### Confusion Matrix

                             Predicted: No Disease   Predicted: Disease
  ------------------------ ----------------------- --------------------
  **Actual: No Disease**                        71                   11
  **Actual: Disease**                            6                   96

These scores describe performance on the project's test split. Results
can vary with different data splits, preprocessing choices, or model
parameters.

## Feature Importance

The highest-ranked features in the project's feature-importance output
include:

1.  `ST_Slope_Up`
2.  `Oldpeak`
3.  `ST_Slope_Flat`
4.  `ChestPainType_ASY`
5.  `Cholesterol`
6.  `MaxHR`
7.  `Age`

Feature importance indicates how the trained model used features for
prediction; it does not establish causation or medical significance.

## Repository Structure

A suggested GitHub repository structure is:

``` text
Random-Forest-Heart-Disease-Prediction/
├── README.md
├── Random_Forest_Minor_Project_Report_Final.pdf
├── notebook.ipynb
├── data/
│   └── heart.csv
├── outputs/
│   ├── correlation_heatmap.png
│   ├── confusion_matrix.png
│   ├── feature_importance.png
│   ├── roc_curve.png
│   ├── evaluation_metrics.csv
│   └── feature_importance.csv
└── requirements.txt
```

This is a suggested structure. Upload only the files that are actually
present in your project, and update filenames to match your repository.
Check the dataset's license and terms before redistributing the CSV;
linking to Kaggle instead may be more appropriate.

## How to Run

1.  Download the dataset from the [Kaggle dataset
    page](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction).

2.  Open the project notebook in Jupyter Notebook or Google Colab.

3.  Upload or place the CSV where the notebook expects it.

4.  Install the required libraries if they are not already available:

    ``` bash
    pip install pandas numpy matplotlib seaborn scikit-learn jupyter
    ```

5.  Update the dataset path in the notebook if necessary.

6.  Run the notebook cells in order to reproduce preprocessing,
    training, visualizations, and evaluation.

## Limitations

-   The model is trained and evaluated on one dataset and one train/test
    split.
-   Performance on other populations or datasets may differ.
-   Feature importance should not be interpreted as proof of cause and
    effect.
-   The model is intended for academic demonstration, not clinical use.

## Future Improvements

-   Use cross-validation and systematic hyperparameter tuning.
-   Compare Random Forest with other classification algorithms.
-   Add calibration and more detailed error analysis.
-   Validate the approach on independent datasets where appropriate.

## References

1.  Fedesoriano, [Heart Failure Prediction Dataset --
    Kaggle](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction).
2.  Scikit-learn, [Random Forest Classifier
    documentation](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html).
3.  Scikit-learn, [Model evaluation
    documentation](https://scikit-learn.org/stable/modules/model_evaluation.html).

------------------------------------------------------------------------

**Project:** Predictive Classification using Random Forest Ensembles\
**Student:** Pranil Shirsath\
**Institute:** Sapkal College of Engineering
