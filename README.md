# Prosper Loan Data Analysis:
## Predicting the likelyhood that a loan will default or not.

### by Marvellous Onuma-Kalu


## Dataset

The data we analyze in this project is a financial dataset which is publicly
available on Prosper peer-to-peer lending platform. The data which was
downloaded from Udacity's course webpage, covers 113,937 loans funded by Prosper
between November 2005 and March 2014. The dataset has 81 variables out of which
we selected the following 24 for our research purpose;

* Loan characteristics such as
 * Loan Status, Loan Term, Loan Original Amount and Monthly Loan payment
* Borrower's financial information such as
 * Occupation, Stated monthly income, Income Verifiable, Employment status and
employment status duration
* Borrower's credit scores such as
 * Credit score range upper, credit score range lower, Prosper Score, Prosper
Rating and Credit grade
* Some indicators of credit availability such as
 * Debt-to-Income Ratio
 * Available Bankcard Credit
 * Bankcard Utilization
* Credit history such as
 * Current Delinquencies
 * Delinquencies Last Seven Years
* Listing Category and Listing Creation Date
* Borrower's state of residence
* IsBorrowerHomeowner
* BorrowerRate
* BorroweAPR

With these 24 variables, we aim to answer the research question:

### _What is the likelyhood that a borrower would default a loan or not?_

Hence our target (independent) variable is (default) Loan Status, while we use
the remaining 23 (independent) variables to predict a defaulted Loan Status.

#### Note:
Prosper would grant a loan to borrowers who have verified their income. To this
end, I filtered the data for analysisto include only listings with verified
income.

## Summary of Findings
The Loan Status distribution has 66.33% of good (completed) loans and 33.66% of
bad (including default, charge-offs and delinquencies) loans respectively.

- Borrowers on the Prosper platform include highly paid professionals like
Medical Doctors, Pharmacists, Attorneys and Dentist who are full-time workers.
- We observe that most of the borrowers
 * include professionals who want to consolidate their debt using the loans they
obtain from Propser.
 * they reside in California (CA), probably because Prosper is located in
California (CA).
 * The are non-home owners
- Similarly, about 75% of borrowers opt for loan original amount of \$8000 for a
loan term of 3 years at a borrower's interest rate of 26%.

A stronger predictive factor that indicates whether a loan would default or not
is Loan purpose, that is Listing category as described in our dataset. We
observe that Motorcycle loans, then RV loans are the least risky loans while
Green loans then Medical/Dental loan are the riskiest. In terms of loan purpose,
on average we observe that loans for higher available bankcard credit are the
least risky loans.


Furthermore, as one would expect,

* People who go for higher loan original amount will have a longer loan term and
are more likely to default. Intuitively this makes sense given that unfrtunate
life events may happen over time such as lost of job, decreased income amount,
increased responsibilities such as family and children, may affect a borrower's
plan to repay a loan. Specifically, we observe that 5 years loan are more risky
than 3 years loan while 1 year loan has to probability of default.

Although these factors are not strong indicators of default.
* Moreso, borrowers with higher monthly income, lower proportion of debt-to-
income ratio, more available Bankcard credit and lower percentage of bankcard
utilization are less likely to default their loans.

Finally, borrowers with an excellent credit history and credit scores are likely
to have lower interest rate and would less likely defaut their loans.



## Key Insights for Presentation

A barchat was first created to understand the distribution of completed vs
defaulted LoanStatus respectively. Then every independent variables related to
Loan Status were explored. A Heatmap was then created to understand the
relationship between different numerical variables. We observe that Borower rate
has the strongest relation with LoanStatus compared to other numerical
variables. The direction of the relationship is negative indicating that a
higher BorrowerRate would imply a higher likelyhood of default.

The final plot bivariate plots, then we conclude with a multivariate plot of
BorrowerRate, CredtScore Range and Loan Status.
