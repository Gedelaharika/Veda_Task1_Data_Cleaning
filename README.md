# Data Cleaning and Preprocessing

## Veda Technology Internship – Task 1

### Project Overview

This project focuses on data cleaning and preprocessing using Python and Pandas. The Sample Superstore dataset was analyzed to identify and handle common data quality issues such as duplicate records, missing values, formatting issues, invalid numerical values, and potential outliers.

The objective is to prepare a clean and validated dataset suitable for further analysis.

---

## Dataset

**Dataset:** Sample Superstore

**Original file:** `SampleSuperstore.csv`

The dataset contains 9,994 rows and 13 columns.

### Columns

- Ship Mode
- Segment
- Country
- City
- State
- Postal Code
- Region
- Category
- Sub-Category
- Sales
- Quantity
- Discount
- Profit

---

## Tools and Technologies

- Python
- Pandas
- NumPy
- Jupyter Notebook

---

## Data Cleaning Process

### 1. Dataset Inspection

The dataset was loaded using Pandas and inspected using:

- `head()`
- `info()`
- `isnull().sum()`
- `duplicated().sum()`

### 2. Missing Value Check

Missing values were checked across all columns.

**Result:** No missing values were found.

### 3. Duplicate Records

Exact duplicate rows were identified and removed.

- Original rows: **9,994**
- Duplicate rows removed: **17**
- Final rows: **9,977**

### 4. Text Formatting Check

Text columns were checked for leading and trailing whitespace.

**Result:** No extra whitespace was found.

### 5. Numerical Validation

The following numerical fields were validated:

- Sales
- Quantity
- Discount
- Profit

Validation included checking for:

- Negative Sales
- Invalid Quantity values
- Invalid Discount values

**Result:**
- Negative Sales: **0**
- Invalid Quantity: **0**
- Invalid Discount: **0**

### 6. Outlier Analysis

The Interquartile Range (IQR) method was used to identify potential outliers.

Potential outliers identified:

- Sales: **1,167**
- Quantity: **170**
- Discount: **855**
- Profit: **1,881**

These potential outliers were **not removed**, because extreme values can represent legitimate business transactions. Removing them without business justification could result in loss of useful information.

---

## Final Dataset Validation

After cleaning:

- Rows: **9,977**
- Columns: **13**
- Missing values: **0**
- Duplicate rows: **0**
- Negative Sales: **0**
- Invalid Quantity: **0**
- Invalid Discount: **0**

The cleaned dataset was saved as:

`cleaned_superstore.csv`

---

## Project Files

| File | Description |
|---|---|
| `Data_Cleaning_Task1.ipynb` | Jupyter Notebook containing the complete cleaning process |
| `SampleSuperstore.csv` | Original dataset |
| `cleaned_superstore.csv` | Final cleaned dataset |
| `README.md` | Project documentation |
| `CHANGELOG.md` | Detailed record of data cleaning changes |

---

## Conclusion

The Sample Superstore dataset was successfully inspected, cleaned, and validated using Python and Pandas. Duplicate records were removed, data quality checks were performed, and potential outliers were analyzed without unnecessarily deleting legitimate business data.

The resulting dataset is ready for further data analysis and visualization.

---

## Author

**Gedela Harika**

**Veda Technology Internship – Task 1**
