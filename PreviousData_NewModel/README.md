# Previous Teams Dataset with current teams model.

## Overview

In this folder, we used a feature-engineered dataset created by a previous team, named `filtered_customer_tier_data.csv`. 

- This dataset contains only two features:
  - **CustomerTier**
  - **PercentProfit**
- These two features were used to train and evaluate our models, specifically:
  - **Random Forest**
  - **Decision Tree**

## Output Files

- **`DecisionTreeResult.csv`** and **`RandomForestResult.csv`** contain:
  - The **actual** and **predicted** `QuoteStatus`.
  - The **confidence percentage** of each model's prediction.


## Important Notes

- Ensure that the file path to `filtered_customer_tier_data.csv` is correct before running any scripts.
- If needed, update the dataset path at the start of the notebooks or scripts to avoid loading errors.

