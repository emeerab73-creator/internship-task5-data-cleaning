# Internship Task 5 – Data Cleaning & Standardization

## Objective
Clean and standardize a raw internship applicant dataset to ensure data accuracy, as part of the Internee.pk Data Analytics Internship (Task 5).

## What was done
- **Missing values**: Identified and handled gaps in `age`, `city`, `skills`, and `email` — filled non-critical fields (age, skills, city) using median/placeholder values, and dropped rows missing `email` since it's essential contact information.
- **Outliers**: Detected and corrected impossible age values (e.g. -5, 150) before filling missing data, to avoid skewing the average.
- **Duplicates**: Identified and removed exact duplicate applicant records.
- **Standardization**: Fixed inconsistent text formatting in the `city` column (casing, spelling, extra whitespace) so entries like "Lahore", "lahore", and "LAHORE " are unified into one consistent value.

## Tools used
- Python
- Pandas
- Google Colab

## Files
- `internship_applicants_raw.csv` — original messy dataset
- `internship_applicants_cleaned.csv` — final cleaned dataset
- Notebook with full step-by-step cleaning process

## Result
Reduced from 126 raw rows to 113 clean, de-duplicated rows with zero missing values across all columns.
