# Random Forest Model Folder

## Overview

In this folder, you will find different versions of the Random Forest model scripts, along with the final version used for the project.

- The **final version** of the Random Forest model uses only two features:
  - **CustomerTier**
  - **PercentProfit**
- These features were specifically **feature engineered** during the data processing phase.

Earlier versions of the model scripts used a broader set of selected features from the **Quotes** dataset for training and evaluation.

## Additional Notes

- The **Sales** dataset was **not used directly** in the final model because it only includes quotes that resulted in a **Won** status. Since we do not have corresponding sales data for **Lost** quotes, including it would have introduced bias.
- The **Revised** status was **dropped** from the dataset because:
  - These represent quotes that were initially **Lost**, later **Revised**, and then **Won**.
  - Including them caused duplication and confusion in the data.
  - Dropping the Revised status ensured the dataset remained clean and consistent for modeling.

## Output File

- The `RandomForestResult.csv` file shows:
  - The **actual** and **predicted** `QuoteStatus`.
  - The **prediction confidence percentage** for each prediction.



**Important:** Before running any scripts, make sure the dataset paths are correctly set. Update the paths if necessary to ensure smooth execution.e 
