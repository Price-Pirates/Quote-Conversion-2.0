# Models Overview

## Introduction

This folder contains the machine learning models explored during the project. Three main models were considered:

- **Decision Tree**
- **Random Forest**
- **Gradient Boosting**

Each model has its own directory containing different script versions and development stages. Below is a summary of what was done with each model.

---

## Decision Tree

- Multiple versions of the Decision Tree model were developed.
- The **final version** uses only two **feature-engineered** inputs:
  - `CustomerTier`
  - `PercentProfit`
- Earlier versions experimented with a broader set of features selected from the **Quotes** dataset.
- The **Sales** dataset was not used directly because it contained only **Won** quotes, and we did not have comparable **Lost** data.
- The **Revised** status was dropped from the dataset to prevent duplication, as these entries represent quotes that were initially **Lost** but later **Revised** and **Won**.

---

## Random Forest

- Similar to the Decision Tree model, several versions of the Random Forest model were developed.
- The **final version** also uses only:
  - `CustomerTier`
  - `PercentProfit`
- Random Forest achieved strong predictive performance and was selected for final evaluation.
- **Output:** The `RandomForestResult.csv` file contains:
  - Actual and predicted `QuoteStatus`.
  - Prediction confidence percentages for each prediction.


---

## Gradient Boosting

- The Gradient Boosting model was evaluated but **not selected** for final use.
- It produced the **lowest accuracy** among all models considered.
- As a result, this model was dropped, and focus shifted to the Decision Tree and Random Forest models.

---

## Important Notes

- Always verify that your dataset paths are set correctly in the scripts before running them.
- Each folder (`DecisionTree`, `RandomForest`, `GradientBoosting`) contains multiple versions of scripts to show the model development process.
- Final model scripts are clearly labeled inside each folder.

---

If you have any questions about the models or the scripts, please refer to the comments inside each script 