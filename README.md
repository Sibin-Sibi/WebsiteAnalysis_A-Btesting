# WebsiteAnalysis_A-Btesting
Project to run A/B testing to help the company understand if they should implement the new page, keep the old page, or perhaps run the experiment longer to make their decision.


## Overview
The project conducted A/B testing of user conversions on an old and new wepage. 

Steps included handling mismatched condition and page assignment, removing duplicate ids, hypothesis testing via bootstrapping and standard statistical tests, and multiple regression modelling. 


## Technologies Used
- Python, Numpy, Pandas, Matplotlib, StatsModels, Scipy
- Jupyter Notebook


### Statistical Analysis
We used the following three approach to see whether the company should implement a new page or keep the old page. 
* Probability based approach
* A/B test
* Regression approach

## Key Findings
#### Probability based approach:
The probablity that an individual received the new page is 50%, which means that there was an equal chance that an    individual will land in old or the new page.

#### A/B tesing:
Generated null and alternative hypothesis.  Null Hypothesis: Probablity of old page is greater than or equal to the new page. Alternative Hypothesis: Probablity of old page is less than New page.
We simulated user_groups with respect to conversion.
We obtained a p-value of .905, which is high, which means that we fail to reject the null hypothesis

#### Regression:
With logistic Regression, we looked at the two possible outcomes.
with a two-tailed case we had a p-value of 0.190.
By further adding geographic location,we tried to identify countries impact on conversion value.
As p-value of both countries where greater than 0.05, we failed to reject the null hypothesis.
We accept the null hypothesis. 

Based on the dataset and the different approaches we could say that new page does'nt increase the number of users in buying the product.
