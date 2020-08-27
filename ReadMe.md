# Prosper Loan Data Exploration

## Dataset
This dataset contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.
For the exploration and analysis, we have created the subset with the features we are the most interested in (23 variables in total). The main feature of our interest is The interest rate and what factor can affect it. 
This project was a part of The Data Analyst Nanodegree Program by Udacity. 
- The dataset can be downloaded from here: https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1547358770029000. 
- Here is the Prosper data dictionary to explain dataset's variables: https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0
- More information about Prosper can be found here: https://www.prosper.com/.

## Installation 
This project used Python 3 and was completed through the Jupyter Notebooks IDE. 

## Summary of Findings
In the exploration, I found that there was strong positive relationship between Interest rate and Estimated return with correlation coeffcient 0.82 and between interest rate and Estimated loss with r = 0.95. Another strong negative relationship was between Interest rate and Prosper score, r = -0.65. The main trend was: the higher Prosper score, the lower Interest rate, thus a more advantegeous for the borrower. The similar case is relationship between interest rate and Prosper rating. From the boxplot we saw that the loans who have assigned the best rating have the lowest interest rate, under 10%. We expected that the Original loan amount could have strong impact to the interest rate, but correlation coefficient was -0.41. Generally, we can say that the increase in the loan amount is associated with a decrease in the interest rate. We investigated also the terms of the loans (12,36,60 months) and we found out that only the 12 term loan have interest rate about 10%. We found out that the income range of the borrower have also impact on the interest rate. The borrowers who belong to the lowest range (1-24.999$) have the highest rate. And with increasing income ranges, the interest rate is decreasing. With the income ranges are associated also the original loan amount - the higher income range, the higher possible loan amount. We expected the Debt to income ratio will have an impact on the interest rate, but relationship between them was weak and the correlation coefficient was only 0.13. Also the relationship betweeen the interest rate and monthly income was weak, r = -0.24. 

We investigated also the homeownership and we found out that the borrowers with the Prosper score from 5 to 11 can get a better interest rate, when they have provided proof of homeownership (or with mortage debt on their credit reports) to Prosper. We compared two groups of the loans, one group was: the loans under 10.000$, the other group: loans above 10.000$. We found out that the majority of the loans have higher interest rates in the first group. We investigated income ranges with the loan amount by their terms. Generally, the major pattern was observed in the rising loan original amounts with rising income range and median loan original amount is rather similar across all income ranges for 12 months term loan. We also visualized relationship between interest rate and estimated return by terms. The major trend is observed in generally rising of the Estimated return with rising Interest rate. On the other hand, there are some cases when the 36 months term show estimated return in negative values.  


## Key Insights for Presentation
For the presentation, I focus on the Interest rate and what features can have an impact on this variable. I start by introducing The interest rate and interest rate distribution through years. Then I introduce the features that are the most associated with the interest rate such as Prosper score, Prosper rating, Loan amount, Income ranges, Term. Then there is displayed boxplot with the borrower's income ranges vs Loan amounts by the loan terms. The last ist the scatterplot showing relationship between the estimated return and interest rate by the loan terms.
















