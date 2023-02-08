# Project Name : Lending Club Case Study
> This is the case study for a basic understanding of risk analytics in banking and financial services and understand how data is used to minimise the risk of losing money while lending to customers.


## Table of Contents
* [General Info](#general-information)
* [Libraries Used in Python](#libraries-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements) 
* [Team Members](#teammembers)


## General Information <a name="general-information"></a>
- We are analysing the scenario for a consumer finance company which specialises in lending various types of loans to urban customers. There are two types of risks, associated with the bank’s decision for approving loan :

- If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
- If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company
- When a person applies for a loan, there are two types of decisions that could be taken by the company:

  **Loan accepted:** If the company approves the loan, there are 3 possible scenarios described below:

    * Fully paid: Applicant has fully paid the loan (the principal and the interest rate)

    * Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.

    * Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan

  **Loan rejected:** The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)

**Goal:**
Data Analysis using EDA techniques in python to find driving factors for the defaulting of loan.

**Risk associated with the problem**
- If the applicant is likely to repay the loan, then not approving loan is a loss of business (rejecting loans for non - default).
- If the applicant is not likely to repay the loan, then approving loan may lead to financial loss (approving loans for default). The given dataset contains information about past loans and each row represents the loan details of the applicants.

## Libraries Used in Python <a name="libraries-used"></a>
- numpy 
- pandas
- matplotlib.pyplot
- seaborn 
- missingno
- plotly.express 

## Conclusions <a name="conclusions"></a>
 - Following are the major driving factors which can be utilized for predicting the chance of defaulting:
    1. DTI 
    2. Grades
    3. Loan Amount and Installments
    4. Annual income
    5. Pub Record Bankruptcies

- There are few insights if we are considering smaller constraints, and can be considered as defaulters: 
    1. who have annual income in the moderate range i.e. 50000-100000
    2. who have either less working experience or more than 10+ years of experience.
    3. who take higher loan amounts
    4. who don't own house
    5. whose purpose for loan is 'debt consolidation'
    6. whose verification status is not verified


## Acknowledgements <a name="acknowledgements"></a>
- This project is given by Upgrad as an assignment case study
- All the data and requirements are provided by Upgrad.

## Team Members <a name="teammembers"></a>
- Aakash Mal
- Preity Rashmi
