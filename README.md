# SQL_Data-Cleaning-EDA

#   World Layoffs Data Cleaning & Exploratory Data Analysis (EDA)

## Project Overview
This project focuses on cleaning, transforming, and analyzing a real-world global layoffs dataset using MySQL. The workflow is divided into two major phases:

1. Data Cleaning & Transformation  
2. Exploratory Data Analysis (EDA)

The project demonstrates practical SQL skills used in real-world data analytics workflows, including data cleaning, standardization, window functions, aggregations, and trend analysis.

---

## Technical Skills Applied
- SQL (MySQL)
- Common Table Expressions (CTEs)
- Window Functions (`ROW_NUMBER`, `DENSE_RANK`)
- Joins & Self Joins
- Aggregate Functions
- Rolling Totals using `OVER()`
- Data Cleaning & Transformation
- String Functions (`TRIM`, `SUBSTRING`)
- Date Formatting (`STR_TO_DATE`)
- Exploratory Data Analysis (EDA)

---

# Phase 1: Data Cleaning & Transformation

### Duplicate Removal
- Identified duplicate records using `ROW_NUMBER()` with `PARTITION BY`
- Created staging tables to safely isolate and remove duplicate rows

### Data Standardization
- Trimmed inconsistent company names using `TRIM()`
- Standardized industry categories such as different variations of "Crypto"
- Removed trailing characters from country names for consistency

### Date Formatting
- Converted text-formatted dates into SQL `DATE` format using `STR_TO_DATE`
- Modified column data types for proper date analysis

### Handling Null & Missing Values
- Replaced blank values with `NULL`
- Used self joins to populate missing industry values based on matching company records
- Removed rows containing insufficient layoff information

---

# Phase 2: Exploratory Data Analysis (EDA)

### Layoff Trend Analysis
- Analyzed layoffs across companies, industries, countries, and time periods
- Identified companies with the highest total layoffs

### Time-Based Analysis
- Evaluated yearly and monthly layoff trends
- Calculated rolling monthly layoff totals using window functions

### Ranking & Aggregations
- Used `DENSE_RANK()` to identify the top 5 companies with the highest layoffs each year
- Performed aggregations using `GROUP BY` and CTEs to uncover business insights

---

## Tools Used
- MySQL
- SQL

---

## Learning Outcomes
Through this project, I strengthened my understanding of:
- Real-world data cleaning workflows
- Writing analytical SQL queries
- Window functions and ranking techniques
- Exploratory data analysis using SQL
- Structuring end-to-end SQL analytics projects
