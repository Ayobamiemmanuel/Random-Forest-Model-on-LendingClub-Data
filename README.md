# LendingClub Loan Repayment Prediction
In this project, we will be exploring publicly available data from LendingClub.com in order to create a model that will help predict whether or not a borrower will repay their loan in full. LendingClub connects borrowers who need money with investors who have money to lend. As an investor, we want to invest in people who have a high probability of paying us back, so we will be using this data to create a predictive model that will help us identify good investment opportunities.

## Data
The data used in this project is from LendingClub loans issued between 2007 and 2010. It has been cleaned of NA values and is available in a CSV file in this repository.

The data contains the following columns:

credit.policy: 1 if the customer meets the credit underwriting criteria of LendingClub.com, and 0 otherwise.
purpose: The purpose of the loan (takes values "credit_card", "debt_consolidation", "educational", "major_purchase", "small_business", and "all_other").
int.rate: The interest rate of the loan, as a proportion (a rate of 11% would be stored as 0.11). Borrowers judged by LendingClub.com to be more risky are assigned higher interest rates.
installment: The monthly installments owed by the borrower if the loan is funded.
log.annual.inc: The natural log of the self-reported annual income of the borrower.
dti: The debt-to-income ratio of the borrower (amount of debt divided by annual income).
fico: The FICO credit score of the borrower.
days.with.cr.line: The number of days the borrower has had a credit line.
revol.bal: The borrower's revolving balance (amount unpaid at the end of the credit card billing cycle).
revol.util: The borrower's revolving line utilization rate (the amount of the credit line used relative to total credit available).
inq.last.6mths: The borrower's number of inquiries by creditors in the last 6 months.
delinq.2yrs: The number of times the borrower had been 30+ days past due on a payment in the past 2 years.
pub.rec: The borrower's number of derogatory public records (bankruptcy filings, tax liens, or judgments).
Approach
Our goal is to create a model that will predict whether or not a borrower will repay their loan in full. We will begin by exploring the data and performing some initial analysis to better understand the relationships between the different variables. We will then preprocess the data and train several machine learning models, including logistic regression, decision trees, and random forests. We will evaluate the performance of each model and select the one that performs best on our validation set. Finally, we will use this model to make predictions on a test set and report our results.

## Requirements
This project was implemented in Python, using several libraries including NumPy, Pandas, Matplotlib, and Scikit-Learn. To run the code in this repository, you will need to have these libraries installed on your system
