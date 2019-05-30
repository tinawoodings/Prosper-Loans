# Prosper Loan Exploration
## by Cristina Woodings


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


## Key Insights for Presentation

For the presentation, I focused on what predictors could lead to a borrower charging off. I started with understanding how many loans were late or defaulted. Then I looked at the variables I thought could predict whether an account charged off first individually and then bivariately. I also looked at how these changed over time.

I used box plots to evaluate the entire range of possibilies between credit scores and estimated returns and clustered bar charts to understand how predicted risk changed over the years. These seems to be the easiest to interpret, which deviated from what I originally explored. Additionally, my initial curiosity during exploration was characteristics of someone who was applying for loan. When correlations did not pan out, I became more interested in trying to predict which loans were less likely to be charged off, which I thought could be an important indicator for investment success.

Initial feedback I recevieved on my explanatory analysis largely had to do with clarification- labeling the graphs more explicitly and clearly. Examples of this were making the estimated return tick labels percentages (10% rather than .10) and writing what the 1-7 estimated return rating meant. Outliers were also distracting.

