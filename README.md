# Excel-Data-Cleaning
This shows the use of excel to clean dirty data, by applying best-practice data cleaning techniques to transform the dataset into a well-structured, consistent, and analysis-ready format.

## Project Overview
This project focuses on cleaning a small dataset using Microsoft Excel to prepare it for accurate analysis. The dataset simulated a real-world scenario where manual data entry resulted in inconsistencies such as irregular formatting, duplicate records, missing values, and input errors.


## Objectives
- Identify and correct inconsistent and inaccurate data entries  
- Improve dataset structure, readability, and usability  
- Ensure data integrity for reliable analysis

![Before Cleaning](messy_data)

## Data Cleaning Process

### 1. Autofit Columns and Rows
- Used `Home → Cells → Format → AutoFit` to standardize row height and column width.  
- Improved readability and made anomalies easier to detect.  

### 2. Remove Duplicate Records
- Applied `Data → Remove Duplicates` to eliminate repeated entries across key columns.  
- Ensured the dataset contained only unique, valid records.  

### 3. Remove Unnecessary Spaces
- Used the `TRIM()` function to remove leading, trailing, and extra spaces, particularly in the Name column.  
- Standardized text values to avoid errors in lookups or analysis.  

### 4. Handle Missing Data
- Identified blank cells using `Go To Special → Blanks` and removed entire rows with missing values.  
- **Note:** Best practice is to assess the impact before deletion. Given the dataset’s small size and low business impact, removing the rows was appropriate.  

### 5. Convert Data into a Table
- Converted the cleaned dataset into an Excel Table using `Insert → Table`.  
- Enabled structured referencing, easier filtering, sorting, and improved formatting.  

### 6. Correct Data Entry Errors
- **Quantity column:** Used an `IF()` formula to fix invalid zero values without altering correct numbers.  
- **Price Per Unit column:** Replaced “inf” via `Find & Replace (Ctrl + H)` to ensure all values were valid numbers.  

### 7. Final Review
- Performed manual review
- Confirmed consistency across dates, quantities, names, and pricing values.


## Tools and Excel Functions Used
**Excel Tools:** Remove Duplicates, Find & Replace, Go To Special, Convert to Table, Filters  
**Functions:** `TRIM`, `IF`  


## Outcome

The dataset was successfully cleaned and transformed into a structured, consistent, and analysis-ready table. Key improvements included:
- Removal of duplicate and invalid entries  
- Consistent text formatting  
- No critical missing data  
- Numeric fields validated and suitable for calculations  
- Improved structure for readability and downstream analysis

![After Cleaning](cleaned_data)

## Key Learnings

- Data cleaning requires both technical skill and judgment.  
- Minor inconsistencies such as hidden spaces can significantly affect analysis.  
- Handling missing values should be context-driven rather than automatic.  
- Structuring data (e.g., using Tables) enhances efficiency in future analysis.  

## Potential Next Steps

If this were a real or ongoing client project, the following steps are recommended:

- Implement data validation rules to prevent future incorrect entries  
- Use Power Query for scalable and automated data cleaning  
- Build a simple Excel dashboard to summarize key insights  
