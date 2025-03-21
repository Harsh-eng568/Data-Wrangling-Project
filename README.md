# Data-Wrangling-Project
This project focuses on data cleaning, transformation, and integration of clinical trial datasets. The goal is to identify and correct inconsistencies, handle missing data, and restructure tables to ensure high-quality, well-organized data for analysis
Dataset Description
The project works with three tables:

Patients – Contains demographic and health-related details of trial participants.
Treatments & Treatments_cut – Records medications administered and corresponding dosages.
Adverse_reactions – Logs any side effects experienced by participants.
Data Issues Identified
Dirty Data
Patients Table:

Inconsistent name formatting and duplicate entries.
Mixed state name formats (full vs. abbreviation).
Invalid or missing zip codes, incorrect data types.
Unrealistic height/weight values.
Treatments & Treatments_cut Tables:

Medication names contain errors (extra characters, hyphens as NaNs).
hba1c_change column has incorrect/missing values.
Duplicate entries for some patients.
Adverse_reactions Table:

Given name and surname are all in lowercase.
Messy Data
Patients Table:

contact column contains both phone numbers and emails (should be separated).
Treatments & Treatments_cut Tables:

Dosage columns should be split into start_dose and end_dose.
The two tables should be merged.
Adverse_reactions Table:

Should be integrated into the main dataset rather than existing separately.
Data Cleaning Process
The following steps were taken to clean and wrangle the data:

Fixing Data Types:

Converted sex to a categorical type.
Standardized zip_code to a string with leading zeros.
Converted birthdate to a datetime format.
Handling Missing Data:

Imputed missing values where applicable.
Standardized NaN values across all tables.
Correcting Errors & Inconsistencies:

Fixed name spellings and duplicate entries.
Standardized state names to abbreviations.
Cleaned and split medication dosage columns.
Restructuring Tables:

Merged the Treatments and Treatments_cut tables.
Integrated Adverse_reactions into the main dataset.
Technologies Used
Python (Pandas, NumPy, Regex)
SQL (for structured data transformations)
Jupyter Notebook / Google Colab
Project Status
✅ Completed Data Cleaning
