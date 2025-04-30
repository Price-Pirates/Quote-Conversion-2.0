# Decision Tree Model Folder

## Overview

In this folder, you will find different versions of the Decision Tree model scripts, along with the final version used for the project.

- The **final version** of the Decision Tree model uses only two features:
  - **CustomerTier**
  - **PercentProfit**
- These features were specifically **feature engineered** during the data processing phase.

Earlier versions of the model scripts used a broader set of selected features from the **Quotes** dataset for training and evaluation.

## Additional Notes

- The **Sales** dataset was **not used directly** in the model because it only includes quotes that resulted in a **Won** status. Since we do not have corresponding sales data for **Lost** quotes, including it would have introduced bias.
- The **Revised** status was **dropped** from the dataset because:
  - These represent quotes that were initially **Lost**, later **Revised**, and then **Won**.
  - Including them caused duplication and confusion in the data.
  - Dropping the Revised status ensured the dataset remained clean and consistent for modeling.

**Important:** Before running any scripts, make sure the dataset paths are correctly set. Update the paths if necessary to ensure smooth execution.