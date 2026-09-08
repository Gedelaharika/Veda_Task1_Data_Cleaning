# Data Cleaning Change Log

## Project
Veda Technology – Internship Task 1

## Dataset
SampleSuperstore.csv

## Changes Performed

### 1. Duplicate Rows
- Original rows: 9,994
- Duplicate rows identified: 17
- Duplicate rows removed: 17
- Final rows: 9,977

### 2. Missing Values
- Missing values were checked in all columns.
- Result: 0 missing values.
- No missing-value treatment was required.

### 3. Text Formatting
- Text columns were checked for leading and trailing spaces.
- No extra whitespace was found.
- No text-formatting changes were required.

### 4. Numerical Validation
- Negative Sales: 0
- Invalid Quantity (less than or equal to 0): 0
- Invalid Discount (less than 0 or greater than 1): 0
- No invalid numerical values were found.

### 5. Outlier Analysis
The IQR method was used to identify potential outliers.

- Sales: 1,167 potential outliers
- Quantity: 170 potential outliers
- Discount: 855 potential outliers
- Profit: 1,881 potential outliers

Potential outliers were **not removed**, because extreme values can represent legitimate business transactions and should not be deleted without business justification.

## Final Dataset Validation
- Rows: 9,977
- Columns: 13
- Missing values: 0
- Duplicate rows: 0
- Negative Sales: 0
- Invalid Quantity: 0
- Invalid Discount: 0

## Output
The cleaned dataset was saved as:

`cleaned_superstore.csv`