## Final 2020 Presidential Election Prediction

_By Miroslav Bergam_

_November 1st, 2020_

### Introduction

2020 has disrupted the status quo of predicting elections. While a data scientist's instinct is typically to consider as many useful factors as possible in creating a final prediction for a presidential election, the events of this last year, such as a global pandemic that has affected the economy in unprecedented ways, has made typically reliable measures like GDP largely useless as a predictor for this election's outcome. 

The predictors I've decided to use in my final model are whether or not a candidate is incumbent or a member of the incumbent party, their average approval rating in the last few months of their term if they are the incumbent, their polling averages following their party's convention, and the outcome for their party in the previous election. The formula is as follows: 

`pv2p ~ incumbent + incumbent_party + average_poll + last_election + approval`

I found that these predictors were the most informative in generating a reasonable prediction for the 2020 election. Two predictors I worked with but ended up excluding were economic data and COVID-19 data

(2) model description and justification, 
(5) model validation (recommended to include both in-sample and out-of-sample performance unless it is impossible due to the characteristics of model and related data availability), 
(6) uncertainty around prediction (e.g. predictive interval)
(7) graphic(s) showing your prediction


![](../figures/summarytable.png)

Overall, our model has a moderately strong in-sample fit, with a R-squared of 0.892. All of our coefficients are statistically significant.  Incumbent candidates, like President Trump, experience a boost of 2.38 percentage points on average; however, being a member of the incumbent party leads to a loss of 8.89 percentage points on average. This comports with the earlier findings on this blog that incumbency comes with both advantages and disadvantages. While being a direct incumbent can boost a candidate because the electorate is most familiar with that candidate, among other reasons, members of an incumbent party can also experience a loss of votes as voters react to whoever was previously in office. 

Additionally, it finds that each additional point in a candidate's pre-election polling average in a given state leads to a 0.41% increase in their voteshare for that state on average. Each point that a candidate's party won in a given state in the previous presidential election results in a 0.71% increase in their voteshare for that state on average. Finally, each point an incumbent candidate

Based on all of


### Predictions

By feeding our model Trump's most recent approval ratings, his polling averages since the first presidential debate, and the state-level outcomes of the 2016 election, I've generated this prediction on the electoral map for the 2020 election:

![](../figures/finalpredmap.jpg)



![](../figures/finalelectoral.jpg)

### Uncertainty

I generated confidence intervals along with my point-estimate predictions on the voteshare for each state in the coming election. You can explore the table below to see the uncertainty surrounding Trump's win and loss margins by state. 

![](../figures/finaltable.html)