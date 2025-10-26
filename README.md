#  Data Cleaning &  Exploratory Data Analysis (EDA) — 2022 World Layoffs Dataset

###  Overview
This project focuses on cleaning and analyzing the **2022 World Layoffs dataset** sourced from Kaggle.  
The dataset captures global layoffs across various industries, countries, and company stages during the post-pandemic economic downturn.

Through SQL-based **data cleaning** and **exploratory data analysis (EDA)**, I aimed to uncover patterns, trends, and insights about the global layoff landscape.

---

###  Tools & Technologies
- **Database:** MySQL  
- **Techniques:** Data Cleaning, EDA, Window Functions, CTEs, Aggregations  
- **Skills Demonstrated:**  
  - Data preprocessing and deduplication  
  - Handling missing or inconsistent values  
  - Identifying trends across years, industries, and locations  
  - Applying analytical SQL for ranking and cumulative analysis  

---

###  Data Cleaning Steps
The raw dataset was messy — it contained null values, inconsistent company names, and date format issues.  
Here’s what I did:
- Removed duplicates and null values  
- Standardized column names and formats  
- Fixed inconsistent entries (e.g., location, industry)  
- Created a clean staging table (`layoffs_staging2`) for analysis  

###  Exploratory Data Analysis (EDA)  
Key areas explored:  
- Maximum and minimum layoffs per company  
- Percentage of company workforce affected  
- Companies that completely shut down (100% layoffs)  
- Funding vs. Layoff patterns  
- Layoffs grouped by company, country, and year  
- Rolling totals of layoffs over time  

**Sample Insights:**  
- Several startups went fully out of business (100% layoffs).  
- EV company **BritishVolt** and **Quibi** stood out, with massive funding but eventual collapse.  
- The highest total layoffs occurred in **2022**, showing a sharp spike post-pandemic.

