# Project Name
This case study aims to give an idea of applying EDA in a real business scenario. In this case study, we will apply the EDA techniques towards developing a basic understanding of risk analytics in financial services and understand how data is used to minimise the risk of defaulting customers when financial institues lend money.

This case study aims to identify patterns which indicate if a client has difficulty paying their instalments which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.

This will ensure that the consumers capable of repaying the loan are not rejected. Identification of such applicants using EDA is the aim of this case study.


## Table of Contents
* [General Info](#general-information)
* [Data Cleaning and Outlier Management](#DC-OM)
* [Analysis of Univariate and Bivariate](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Info
- Raw data provided contains data of individuals and their respective loans data
- Data contains 111 Columns and 39717 Rows
- We need to analyse this data and derive data that could help identify patterns which indicate if a client has difficulty paying their installments. 


## Data Cleaning and Outlier Management
- Annual_Inc - Column had multiple outlier. So outlier have been treated and replaced with median
- int_rate - Removed % from the text, replaced blanks with 0 and changed data type to float
- Purpose - For data that has "Others" as value, we derive the value based on Title and Desc columns
- issue_d, last_credit_pull, earliest_cr_line - Split the field into Year and Month
- emp_length - 
	1. if <1 and NA yes, consider 0 
   	2. 10 + Years = 10 
   	3. Remaining (Example: 5 Years)  - R	emove years (Example: 5). 
   	4. Convert to INT
- term, - remove "months" convert to int64
- For 70 columns with more than 50% missing data or all rows containing same data are dropped


## Analysis of Univariate and Bivariate
-
-
-


## Technologies Used
- Jupyter Notebook 6.5.2
- GitHub 


## Acknowledgements
Give credit here.
- Upgrad tutorials


## Contact
Created by [@mvinayvenkatesh] - feel free to contact me!

