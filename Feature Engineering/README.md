

## Overview

This folder contains Jupyter notebooks and datasets used to process, prepare, and model customer data. The notebooks perform feature engineering steps like calculating **PercentProfit** and assigning **CustomerTiers**, and the datasets are used for building and evaluating machine learning models.

## Notebooks

### 1. `PercentProfit.ipynb`
- This notebook outlines the process taken to calculate the **PercentProfit** for the dataset.
- **Important:** Ensure that the file path is correct when loading the dataset. Update the path if necessary to successfully run the notebook.



### 2. `CustomerTier.ipynb`
- This notebook details the steps to compute the **CustomerTier** for each customer.
- **Important:** Make sure the file path is accurate when loading the data. If not, update the path.



## Data Files

### 1. `customer_profit_status.csv`
- This is the final CSV file generated after completing both notebooks.
- It includes the following columns:
  - **CustomerTier**
  - **PercentProfit**
  - **QuoteStatus**
- This file is used for the final prediction models: **Random Forest** and **Decision Tree**.

### 2. `PercentProfit.csv`
- This is the overall dataset.
- It contains:
  - **PercentProfit**
  - **CustomerTier**
  - **UnitCost**
  - Other relevant features.



