# Data Cleaning Project 01 -- Decodelabs Internship

![Python](https://img.shields.io/badge/Python-Data%20Cleaning-blue)
![Pandas](https://img.shields.io/badge/Pandas-Analysis-green)
![NumPy](https://img.shields.io/badge/NumPy-Data%20Processing-blueviolet)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![DecodeLabs](https://img.shields.io/badge/Internship-DecodeLabs-red)


## Project Overview
This project focuses on cleaning and preparing a raw business dataset for further analysis and reporting.

The objective was to identify and handle data quality issues such as:
- Missing Values
- Duplicate records
- Data type inconsistencies
- Outliers
- Invalid data entries

The final cleaned dataset is ready for Exploratory Data Analysis (EDA), visulaization, and business intelligence applications.

---

# Project Objectives

- Understand dataset structure
- Perform data quality assessment
- Identify missing values
- Detect duplicate records
- Validate data types
- Analyze outliers
- Create a cleaned dataset
- Prepare data for further analytics

---

# Tools and Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook
- GitHub

---

# Project Structure

```text
decodelabs-data-cleaning-preparation/
|
|--- dataset/
|    |--- raw_dataset.xlsx
|    |--- cleaned_dataset.xlsx
|
|---notebook/
|    |--- data_cleaning_project.ipynb
|
|--- screenshots/
|    |--- business_validation.png
|    |--- cleaned_dataset_export.png
|    |--- datatypes.png
|    |--- duplicates_check.png
|    |--- final_validation.png
|    |--- missing_values_after_cleaning.png
|    |--- quality_outliers.png
|    |--- unitprice_outliers.png
|
|--- report/
|    |--- Data_Cleaning_and_preparation_project.pdf
|
|--- README.md
```

---

# Data Cleaning Process

## 1. Dataset Loading

- Imported dataset using Pandas
- Checked rows and columns
- Examined overall dataset structure

---

## 2. Data Inspection

Performed:

```python
df.info()
df.shape
df.describe()
```

Purpose:

- Understand column types
- Verify dataset dimensions
- Generate statistical summary

---

## 3. Missing Value Analysis

Used:

```python
df.isnull().sum()
```

Findings:

- Missing values detected in selected columns
- Appropriate treatment applied based on data type

Actions:
- Numerical columns -> Median Imputation
- Categorical columns -> Mode Imputation

---

## 4. Duplicate Record Check

Used:

```python
df.duplicated().sum()
```

Purpose:

- Identify repeated records
- Prevent biased analysis

Result:

- Duplicate records were checked and handled appropriately.

---

## 5. Data Type Validation

verified all column data types using:

```python
df.dtypes
```

Purpose:

- Ensure numerical fields remain numeric
- Ensure date fields remain datetime format
- Maintain data consistency

---

## 6. Outlier Analysis

Outliers were analyzed using boxplots.

Exampled:

```python
plt.boxplot(df["Quanity"])
```

Vaiables analyzed:

- Quanity
- Unit Price

Observation:

- No significant outliers were observed, indicating that the values fall within a reasonable business range and do not require treatment.

---

## 7. Final Validation

Performed final quality checks:

```python
df.isnull().sum()
df.duplicated().sum()
df.info()
```

Result:

✔️ Missing values handled

✔️ Duplicate records checked

✔️ Data Types validated

✔️ Dataset prepared for analysis.

---

# Key Findings

- Dataset structure was successfully validated.
- Missing values were identified and treated.
- Duplicate records were checked and resolved.
- Data types were verified and standardized.
- Outlier analysis was performed using visualization techniques.
- Final dataset was prepared for further analytical tasks.

---

# Project Screenshots

The repository contains screenshots demonstarting:

- Dataset Information
- Missing Value Analysis
- Duplicate Check
- Data Type Validation
- Outlier Detection
- Final Validation

---

# Deliverables

- Cleaned Dataset
- Jupyter Notebook
- Project Report
- Documentation
- Screenshots

---

# Outcome

The dataset was successfully cleaned and validated.

The final cleaned dataset is suitable for:

- Exploratory Data Analysis (EDA)
- Data Visualization
- Dashboard Development
- Business Intelligence Reporting
- Machine Learning Preparation.

---

# AUTHOR

**Srinidhi Kukutam**

Data Analyst Intern - Decodelabs Internship Program

Github: https://github.com/Sri-nidhi20
