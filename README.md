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
- issue_d, last_credit_pull, earliest_cr_line - Split the field into Year and Month
- emp_length - 
	1. if <1 and NA yes, consider 0 
   	2. 10 + Years = 10 
   	3. Remaining (Example: 5 Years)  - R	emove years (Example: 5). 
   	4. Convert to INT
- term - remove "months" convert to int64
- For 70 columns with more than 90% missing data or all rows containing same data are dropped


## Analysis of Univariate and Bivariate
- Following driver variables were used for analysis: 
- 1. Annual Income 
- 2. Region
- 3. Term
- 4. Loan Amount
- 5. Employee Length
-
- Univariate:
- Observation
- 1. For Short Term tenure, among charged off members, higher number of charged off is when the loan amount is between 500-8000.
- 2. 30k-50k is the peak income of charged off members while 50k-60k is the peak income of fully paid members. 
- Bi/Multi Variate:
- Observation
- 1. For all 3 loan status (Current, Charged off and Fully paid), the average annual income is increasing with the Employee Length.
- 2. For Loan Status - Charged Off, the average annual income is lower compared to all other Loan status considered. 
- 3. The loan amount taken by Charged off members between 25-75 percentile range is slightly higher than the loan amount taken by Fully paid members.  
- 4. There is a clear outlier that members with purpose as "Credit Card" and "Debt consolidation" are at higher risk of loan defaulting
- 5. It can be observed from percentages pf defaulters that members with purpose as "Small Business" are at higher risk of loan defaulting
- 6. Members from state of CA, FL, NY have higher count of defaulters. 
- 7. From a percentages perspective the states (NE ( although count is low), NV, SD and FL) have higher defaulters and thus risk states to grant loans to members.


## Technologies Used
- Jupyter Notebook 6.5.2
- GitHub 


## Acknowledgements
Give credit here.
- Upgrad tutorials


## Contact
Created by [@mvinayvenkatesh] - feel free to contact me!

