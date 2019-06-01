# Prosper-Loans
Prosper is a peer to peer personal loan company. They tailor small loans for anything from consolidating debt to home improvement. This particular data set contains over 100,000 loans with 81 pieces of information on each loan. The loans are from between 2005 and 2014 and the loan term ranges between 5 and 60 months. The loan amount ranges from $1000 to $35,000.

## Dataset

This particular data set contains over 100,000 loans with 81 pieces of information on each loan. The loans are from between 2005 and 2014 and the loan term ranges between 5 and 60 months. The loan amount ranges from $1,000 to $35,000.

The prosper dataset used can be found here:
https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv.

With variable definitions found here: 
https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0

Two key wrangling items were:
* Verifying the monthly income with the annual income, deleting entries that did not match.
* Creating a new column called "ChargedOff" indicating whether an borrower charged off the loan or not. This value was based on the "LoanFirstDefaultedCycleNumber".

## Summary of Findings

In the exploration, I found there was very little correlation between the nearly 20 variables I looked at. The ones that had correlations above/below 0.5 were:
* Borrower Rate
* Credit Score Range (barely)
* Prosper Rating
* Estimated Return

When looking to choose a loan in hopes it will not charge off, look to invest in ones that have a Prosper Rating of 4 and higher and have a term of 12 or 60 months. Credit score is not necessarily a good indication for whether or not a borrower chargers off.
