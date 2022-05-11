# Lending Case Study
> Minimizing the potential losses for the lending club company by identifying the potential loan defaulters using Exploratory Data Analysis


## Table of Contents
* [Problem Statement](#Problem-Statement)
* [Technologies Used](#technologies-used)
* [Data Cleaning](#Data-Cleaning)
* [Analysis Flow](#Analysis-Flow)
* [Conclusions](#conclusions)

<!-- You can include any other section that is pertinent to your problem -->

## Problem Statement
- we work for a consumer finance company which specializes in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:
- If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
- If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company
 - Find out how consumer attributes and loan attributes influence the tendency of default?

## Technologies Used
- Pandas
- numpy
- Seaborn
- Matplotlib



## Data Cleaning
- We received a data set containing 111 columns with 39717 records
- Out of 111 columns we have removed 57 columns as those columns contain 40% to 100% of data as Nan values.
- Removed the Customer Behavior 20 variables which are not available at the time of loan application
- Removed the columns which have only 1 value (and NaN values) across the users as there is no variance
- Removed the categorical variables whose distribution is widespread i.e., lot of unique entries are present and hence those columns can be removed
- After removing all the unwanted and non meaning full columns we are left with 18 columns and null values are less than 3 %. 
- Term column represents loan tenure in months. So removing the “months” value and keeping only the number in term column
- Clean the numerical data which has postfix strings added




## Analysis Flow
- Univariate analysis was performed on categorical and numerical variables respectively
- Bivariate analysis was performed on numerical and categorical data respectively
- Based on the insights from univariate and bivariate analysis special situations were considered for segmented analysis
- Segmented analysis for special situations to avoid losses and for long term expansion plans were derived



## Conclusions
- Over the years, although the customer base of loan applicants is increasing(which is a positive sign), the default rate(Charged off Customers) is at ~20% which is a significant number, because the total amount lended to these customers is Company's loss

### To avoid Loss
1. The most immediate step we can take is to avoid lending loans to customers from "NE" state whose annual income is comparable to the loan amount and revol_util is high(>80%). The default rate for these customers is >65% i.e., 65 out of 100 customers are Charged off Customers.
2. Customers who took loans for "Small Business" purpose tend to Charge off their laon if they have high revol_util value(>35%). We can experiment these customers by marginally reducing the interest rates to the high Grade, low revol_util customers so that chances of Paying off loans increases
3. Customers with low annual incomes(<12000 dollars) and low grading are to be offered less loan amount with slightly higher interest rates as these customers have high chances of defaulting the money.

### To increase Profit Margins
1. For the 'A' Grade customers with high Annual income(>40000 dollars) and low revol_util(<25%), we can either offer them marginally more loan amount as per their requirement or slightly increase the interest rates(less suggestible)
2. For the long-term growth, We can expand our services to states like "IA", "ME" where we have very less customer base and almost 0% default rate and target the customers who have Home Ownership as "Rent" or "Mortgage" as these are the potential customer base we observed from our previous records


## Contact
Created by [@https://github.com/SuryaV21][]
 - feel free to contact me!
