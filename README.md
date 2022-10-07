# Prosper Loan Data Exploration
## by Lawal Rasheed


## Dataset

The dataset consists of 114,000 rows of loan data and 81 variables which includes Loan amount, Stated Monthly Income, Debt to Income Ratio, Loan Term, Prosper Score and many others. The dataset can be found [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv), and its documentation [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0). 

## Data Wrangling

1. A subset of the dataframe was created containing 20 columns.
2. The dataframe was assessed for Data Quality and Tidiness Issues.
3. The rows with missing/null Prosper Score values were dropped.
4. Incorrect data types were converted to their respective data types.
5. The booleans in IsBorrowerHomeowner column were replaced with Home Owner for True, and Not Home Owner for False, leaving the dataframe with 74,035 listings and 20 variables.

## Summary of Findings

During exploration, it was discovered that there was a strong positive correlation/relationship between Monthly Payment and the Loan amount which was strengthened by the Loan Term. On encoding a bivariate plot, using a third variable - Loan Term, it was shown that borrowers with Long Term(36 or 60 months) received larger loan amounts.

It was also discovered that a relationship existed between Loan Amount and Categorical features, in which more loans were associated with borrowers with a longer Loan Term, a high Prosper Score, owning a home and being employed.

## Key Insights for Presentation

My focus for the presentation was on the Loan Original Amount variable, Income Range, Stated Monthly Income, Debt to Income Ratio, Prosper Score, and the Employment Status Duration. I started by introducing the Loan Original Amount variable, followed by the distribution of other variables with plotting scatterplots to show correlations.

Scatter plots showing the correlation between Loan Amount and Monthly Loan Payment was carried out, with the plot showing a strong positive correlation/relationship between the two variables, and also showing an evidence of a third variable being involved which was then explained using a multivariate plot during the forthcoming explorations.
From the observation made earlier with the strong correlation between Loan Amount and Monthly Loan Payment, a multivariate scatter and point plot was plotted to show that the two variables is being influenced by a third - Loan Term variable, which is also influenced by the Prosper Score (risk score) implying that the longer the Loan Term and the better the risk score (Prosper Score), the larger the loan amount to be given out. 