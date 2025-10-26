# 2022 Global Layoffs Data Cleaning (MySQL)

##  Overview
This project focuses on cleaning and standardizing the 2022 Layoffs dataset from [Kaggle](https://www.kaggle.com/datasets/swaptr/layoffs-2022).  
The goal was to prepare a clean, analysis-ready dataset by removing duplicates, handling null values, standardizing text fields, and ensuring consistent date formats using MySQL.

---

##  Tools & Skills
- **Database:** MySQL  
- **Techniques:** Data Cleaning, Data Standardization, Duplicate Removal, Data Validation  
- **Source:** [Kaggle – Layoffs 2022 Dataset](https://www.kaggle.com/datasets/swaptr/layoffs-2022)

---

##  Key Steps in the Process
1. **Created a staging table** to preserve raw data.  
2. **Identified and removed duplicates** using `ROW_NUMBER()` and partition logic.  
3. **Standardized values** for `industry`, `country`, and `date` fields.  
4. **Handled missing values** through conditional updates and joins.  
5. **Removed unusable records** (rows with both layoffs and percentage columns null).  
6. **Validated and finalized dataset** for exploratory analysis.

---

##  Sample SQL Snippets
```sql
-- Remove duplicates using ROW_NUMBER
DELETE FROM world_layoffs.layoffs_staging2
WHERE row_num > 1;

-- Standardize country names
UPDATE layoffs_staging2
SET country = TRIM(TRAILING '.' FROM country);

-- Convert date format
UPDATE layoffs_staging2
SET `date` = STR_TO_DATE(`date`, '%m/%d/%Y');# MySQL-Data-Cleaning-Project
Data cleaning project on the 2022 global layoffs dataset from Kaggle — removing duplicates, standardizing values, handling nulls, and preparing data for analysis using MySQL.
