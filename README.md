# LendingClubCaseStudy
Exploratory data analysis case study

# Business Goal
Reduce the number of defaulted loans without significantly reducing business potential by rejecting borrowers who will pay off.

# Data issues and cleaning
- Lot of variables contain high amount (>90%) of missing data. (solution: remove variables)
- Variables have unique data, not useful for analysis. (solution: remove variables)
- Rows still contain missing variables. Data Imputation (global/local mean, median, mode) (not applied in this assignment)
- Dates are read as string and converted to date type
- Term parsed and rewritten to remove space
- Interest rate: % removed, converted to float

# Derived variables
- installment_monthly_income_ratio
- loan_amount_income_ratio
- funded_percentage
- issue_imonth

# Main problem
14.6% of borrowers default on the loan.

# Summary of Recommendations
- Annual Income (strong predictor)
- Instalment / Monthly income ratio
- Term (longer = higher risk) (strong predictor)
- Grade (strong predictor)
- Subgrade (A-D reliable)
- Annual income used in conjunction with grade can be a good predictor
- Small business loans represent higher risk (check other predictors)
- Moderate underfunding does not increase default
- Employment length not relevant (do not use)
- High interest rate = high risk (strong predictor)
- Loan amount >15000 elevated risk, check other predictors