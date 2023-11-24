# Bayesian A/B test
Continuous monitoring in A/B tests has been widely used for choosing options, variants or treatments in health care analytics. For example, A/B tests are common in the design of web products from two/multiple versions, Internet platforms and diabetic medications with continuous monitoring. It has gradually become a cutting-edge research direction of data-driven decision science.Bayesian A/B test that adopts the prior information to fit the parameters, uses the accumulated information to update the likelihood, and considers the expected loss of errors to control the false discovery rates. 

# Data description
Our dataset is the diabetes medication data. These medications were metformin (R1), glipizide (R2) and glibenclamide (R3). The "basedata" shows the dataset we used in "5.2 Bayesian A/B tests with diabetic medications". Sheet 1 shows the raw data. Sheet 2 shows the three diabetes medications with the corresponding readmissions after 30 days. Sheet 3 shows all three medications. Sheet 4,5 and 6 shows the three medication Separately. Where drug 0-3 indicates change in dose. Readmission ">30" indicates readmission after 30 days and is recorded as 1, otherwise it is recorded as 0.

We then used the raw data for propensity matching scores to obtain covariate balanced data. The dataset "matchit" shows the matching data. Sheet 1 is the raw data. Sheet 2,3 and 4 includes the R1,R2 and R3 Separately.

# Code description
We use R package "bayesAB" to analyse to get the result " Table 2 Bayesian A/B tests with diabetic medication (Taking R1/R2 testing as an example).". 

We use R package "MatchIt" to get the matched data.

we use to analyse martingale...
