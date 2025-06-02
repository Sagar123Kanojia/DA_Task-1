# DA_Task-1
# Data Cleaning and Preprocessing - Customer Personality Analysis

## Task Overview
This task was part of a 15-day internship project from **Elevate Labs** focused on data analytics.  
**Task 1** required performing data cleaning and preprocessing on a raw dataset using **Excel or Python (Pandas)**.

---

## Dataset Used
- **Name:** Customer Personality Analysis
- **Source:** [Kaggle Dataset Link](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)
- **Format:** CSV

---

## Tools Used
- **Microsoft Excel**

---

## Data Cleaning Steps Performed

### 1. Removed Duplicate Rows
- Selected all rows and columns.
- Used **Data → Remove Duplicates** to eliminate repeated entries.

### 2. Handled Missing Values
- Used **Filter** to identify blank cells in columns like `Income`.
- Filled missing values in `Income` using the column **average** via the `=AVERAGE(range)` function.

### 3. Standardized Categorical Text Columns
- Cleaned inconsistent text in columns like `Marital_Status` using **Find & Replace** and formulas like:
  - `=PROPER(cell)` to capitalize properly (e.g., `widow` → `Widow`)
  - Ensured values like `single`, `SINGLE`, `Single` were standardized.

### 4. Converted Date Columns
- Ensured the `Dt_Customer` column was in consistent **dd-mm-yyyy** format using:
  - **Format Cells → Date**
  - Or formula: `=TEXT(cell, "dd-mm-yyyy")`

### 5. Cleaned Column Headers
- Renamed all headers to:
  - Be in **lowercase**
  - Use **underscores** instead of spaces (e.g., `Year_Birth`, `Marital_Status`)
  - Manually edited Row 1 (column headers)

### 6. Verified Data Types
- Ensured numeric fields like `Age`, `Income` were formatted as **Number**.
- Verified that `Dt_Customer` was formatted as **Date**.
- Used alignment (right = number, left = text) and **ISNUMBER()** to check types.

---
