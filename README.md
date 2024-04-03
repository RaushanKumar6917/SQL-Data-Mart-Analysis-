# SQL-Data-Mart-Analysis-
[Case Study 1 Data Mart.docx](https://github.com/RaushanKumar6917/SQL-Data-Mart-Analysis-/files/14847294/Case.Study.1.Data.Mart.docx)


**Data Mart Analysis through MySQL**
This repository contains scripts and queries for performing data mart analysis using MySQL. The focus is on cleaning and preparing the data, followed by executing various queries to answer specific questions related to the provided case study.
**
Data Cleansing Steps**
To prepare the data for analysis, the following steps are performed in a single query, resulting in a new table named clean_weekly_sales in the data_mart schema:

Adding Week Number: Assigning a week number to each week_date value.
Adding Month Number: Assigning a month number to each week_date value.
Adding Calendar Year: Assigning a calendar year value (2018, 2019, or 2020) to each week_date value.
Adding Age Band: Creating a new column age_band based on the number inside the segment value, mapping to 'Young Adults', 'Middle Aged', or 'Retirees'.
Adding Demographic: Creating a new column demographic based on the first letter in the segment values, mapping to 'Couples' or 'Families'.
Replacing Null Values: Replacing all null string values with 'unknown' in the original segment column as well as the new age_band and demographic columns.
Calculating Average Transaction: Generating a new column avg_transaction calculated as sales divided by transactions, rounded to 2 decimal places for each record.
