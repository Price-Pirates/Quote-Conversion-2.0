# Dataset Cleaning Notebook (`dataset_cleaning.ipynb`)

This Jupyter notebook performs comprehensive cleaning and preprocessing of two datasets related to sales and quotes data. The notebook follows a structured approach to ensure the data is ready for analysis.

## Datasets Processed
1. **Quotes Data**: `Intuilize_MNSU_ACME_QuotesData.csv`
   - Contains information about customer quotes (2,254,818 rows, 20 columns)
2. **Sales Data**: `Intuilize_MNSU_ACME_SalesData.csv`
   - Contains information about completed sales (1,214,881 rows, 21 columns)

## Cleaning Steps Performed

### 1. Data Loading
- Loaded both CSV files into Pandas DataFrames
- Initial inspection of the first few rows of each dataset

### 2. Data Inspection
- Checked basic information (number of rows, columns, data types) using `df.info()`
- Identified mixed data types in some columns (addressed during cleaning)

### 3. Missing Value Handling
- Identified columns with missing values:
  - Quotes Data: `Ship2City` (4,525), `Ship2State` (20,359), `ConvertedToOrderNumber` (700,091), `ConversionDate` (700,091)
  - Sales Data: `Ship2City` (2,453), `Ship2State` (10,914)
- Dropped columns where more than 50% of values were missing
- Filled remaining missing values with 'Unknown'

### 4. Duplicate Handling
- Checked for and removed duplicate rows
- Found no duplicates in either dataset

### 5. Data Type Correction
- Converted date columns to proper datetime format:
  - Quotes Data: `QuoteDate`, `ExpirationDate`, `ConversionDate`
  - Sales Data: `OrderDate`, `SalesDate`
- Converted all ID columns to string type to ensure consistent formatting

### 6. Final Data Validation
- Generated descriptive statistics for both datasets
- Verified all cleaning steps were properly applied
- Confirmed data is now in a clean, analysis-ready state

## Key Findings During Cleaning
- The quotes dataset has significantly more records than the sales dataset
- About 31% of quotes were not converted to orders (missing `ConvertedToOrderNumber`)
- The most common salesperson is "MR GUY HANSON" (ID: SREP2)
- The most common branch is "JOHNHAVEN BRANCH"
- The most common product group is "PROD.Group3"

