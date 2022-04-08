# EDA Credit Loan case Study
This repository contains my first EDA Case Study project on Loan data. 

## Problem Statement:

There are two datasets provided Application Dataset and Previous Application.
When a loan is granted , the applicant may default it or pay up timely. 
If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company.
If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company.
The company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.

## My Approach

* Import both files through pandas. Process and analyze them sequentially.
* Load Application Data file.
* Routine review of the file through info , describe, head options. 
* Find out columns with high null percentage. Drop cols with 40% above null data. 
* Impute missing data for rest of columns.
* Standardize data (fix negative values, rectify datatypes)
* Outlier analysis and Action (Binning)
* Univariate Analysis for defaulters and non-defaulters
* Bivariate Analysis /Multivariate Analysis
* Then same approach and steps on Previous Application data file. 
* Lastly merge both the files. 

## My Conclusion:

### Positive factors (leads to Timely Repay)
* Company should grant more Revolving Loans as they default less hence beneficial. 
* Applicants with 800K+ loans default less
* Very High Income group  (Income 2,25,000+) defaults less
* Higher education people pay up timely.
* Old age groups 55-65 are very safe to grant loans.
* Females default less compared to Males.
* State Servants and Pensioners are more likely to pay timely.
* As the kids count increases , frequency of people applying loan decreases.
* As Price of Goods is high the Amount of loan requested will also be high. Which is quite obvious as people will need high loan to purchase expensive goods. 
* Old age people have generally high income and pay up timely.
* Maximum loans are done on Tuesday.
* For DAYS_DECISION median is around 500 days, which means generally people apply for another loan after 2 years . 
* Consumer Loans get approved very easily in comparison to others. 
* Most of the applications are for Cash loan and Consumer loan. Cash loans are refused more often and Consumer Loans get approved very easily.
* People prefer to repay the loan directly through to the bank.

### Negative factors (leads to Default)
* More Defaults on cash loans.
* Age group of 25-30 most risky.
* Working class people default more. 
* Single and Unmarried default more. 
* Young age people have generally low income and default more. 
* Married people who are unemployed or on Maternity likely to default more. 
* Applicants who have changed the ID recently are more likely to default.
* Maximum set of loan requestors were repeater. Maximum loans are requested to buy phones; Payments are done through POS. 
* Frequency of Cash Loans is high, and they default more as well. 
* Loan passed(AMT_CREDIT) is always equal or lower than loan requested (AMT_APPLICATION). However if the amount is below 10,00,000 then loan passed is even more than requested but that is only happening for Repeaters.
* When the loan amount is too low it may end up as cancelled or unused by the applicant.



