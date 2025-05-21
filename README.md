# Pandas Data Cleaning Project
## Table of Contents

## Introduction
This repository contains a Jupyter Notebook for cleaning and preprocessing customer data using Python Pandas library. This Project demonstrates practical data cleaning steps, including handling missing values, standardizing formats, removing duplicates, and preparing the dataset for analysis. 

## Dataset Overview
The dataset simulates a real-world scenario where customer data contains:
• Duplicate records
• Unnecessary columns
• Inconsistent formatting (Phone numbers, names) 
• Invalid or missing values

## Columns
1. CustomerID
2. First_Name
3. Last_Name
4. Phone_Number
5. Address
6. Paying Customer
7. Do_Not_Contact
8. Not_Useful_Column

## Data Cleaning Steps
1. Removed Duplicates: Used 'drop_duplicates()' to eliminate repeated rows.
2. Dropped Unnecessary Columns: Removed Not_Useful_Column as it had no analytical value.
3. Cleaned Name Fields: Stripped extra spaces and unwanted characters in 'Last_Name'.
4. Standardized Phone Numbers:
   • Removed all non-numeric characters using regex.
   • Formatted valid numbers to 'xxx-xxx-xxxx'.
   • Replaced invalid phone entries with 'NaN'.
5. Cleaned and Standardized Categorical values: Converted 'Paying Customer' values and 'Do_Not_Contact' to 'Y' or 'N'.
6. Filtered Out Unusable Rows:
   • Removed all rows where 'Do_Not_Contact' == 'Y'.
   • Dropped rows with missing phone numbers.
7. Reset Index: After filtering, reset the DataFrame index.

## Key Learnings
• Regular expressions and string operations in Pandas.
• Identifying and handling missing or invalid data.
• Basic data wrangling logics using boolean filters.
• Importance of data cleaning in the analytics pipeline. 

## Acknowledgements
Dataset provided as part of pandas tutorial from [Alex the Analyst Youtube Channel.](https://www.youtube.com/watch?v=bDhvCp3_lYw)
