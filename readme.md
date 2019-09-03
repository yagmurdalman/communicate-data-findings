# Prosper Loan Data Exploration

## Dataset

This data set contains 113,937 loans with 81 variables on each loan, including Borrower APR, Prosper Score, Loan Amount, Loan Status, Stated Monthly Income, and many others. I choose 14 variables for my analysis. The variable definitions are available
[here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0).


## Summary of Findings

I'm most interested in understanding what features are best for predicting the Borrower APR in the dataset. Also, I investigate the interaction between Prosper Score, Loan Original Amount, Debt to Income Ratio, Stated Monthly Income, and the other variables.


In my bivariate exploration the main findings are as the following:

- There is almost a strong negative relationship between Borrower APR and Prosper Score. 
- There is a negative interaction between Borrower APR and Loan Amount.
- Borrower APR and Stated monthly income are negatively correlated.
- Borrower APR and Debt to Income Ratio are positively and weakly correlated.
- There is a weak positive correlation between Borrower APR and Delinquencies in Last 7 Years.
- 36-month loans have the highest average Borrower APR while 12-month loans have the lowest.
- Loan Amount increases in Prosper Score, they are weakly correlated.
- Prosper Score and Stated Monthly Income are positively and weakly correlated. 
- There is a negative interaction between Prosper Score and Debt to Income ratio.
- As delinquencies in last 7 years increases the Prosper Score falls but they are weakly correlated.
- There is a moderate positive correlation between Loan Amount and Stated monthly income.
- Homeowners take larger amount of loans.

In my multivariate exploration, I investigate that how the categorical variables affect the relationship between the numerical variables. The main findings are as follows:

- Term does not have a fixed effect on the relationship between Borrower APR and Prosper Score. However, it has a consistent behavior if we do our analysis by dividing scores into intervals. While the borrowers with score greater than 7 pay more for the 60-month loans while it is the opposite for the scores from 3 to 7.
- Homeowners pay more for the loans comparing to the non homeowners for each Prosper Score except 1 but this difference is pretty low.
- For each term level there is a positive relationship between Loan Amount and Borrower APR. One thing to be noted is that the loans are mostly squeezed into a smaller range of Loan Amount for 12-month, this range becomes larger when the term increases.
- For the fixed Prosper Score, the borrowers take higher amount of loans in average when the term increases.
- For the fixed Prosper Score, it seems like home ownership matters, the homeowners are able to take out larger amount of loans comparing to the non homeowners.
- In general,'Very Bad' type borrowers have the highest average Borrower APR while the 'Very Good' types have the lowest one for the fixed Prosper Score. 
- For the Debt to income ratios between 0-0.3, while the Borrower APR changes from 0.05 to 0.035 for 12-month and 36-month loans, its range is gets narrower for 60-month loans.


## Key Insights for Presentation

In the presentation, I first display the distributions of Borrower APR, Prosper Score, Loan Original Amount and Debt to Income Ratio variables.

Then I provide the relationship between Borrower APR & Prosper Score, Borrower APR & Loan Original Amount, Borrower APR & Debt to Income Ratio, Prosper Score & Loan Original Amount, Borrower APR & Term by using scatter, heat, line and box plots.

Afterwards, I use point plots of Borrower APR & Prosper Score across term. I give heat plots to show the effect of term on the relationship between Borrower APR & Loan Original Amount by Term. I again provide heat plots for Borrower APR & Debt To Income Ratio across Terms. I create a new variable called 'Borrower Type' by categorizing borrowers with respect to their delinquency numbers and use barplots to show the role of borrower type on the interaction of Borrower APR vs. Prosper Score. I use boxplots to display how home ownership influences the interaction of Loan Original Amount and Prosper Score. Finally, I present point plots of Prosper Score vs. Loan Original Amount across terms.
