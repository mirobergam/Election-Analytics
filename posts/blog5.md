## Predicting 2020 Presidential Election Win Margins

_By Miroslav Bergam_

_October 10, 2020_

### Methodology

Using historical voting data on presidential elections, are we able to predict Vice President Joe Biden's win or loss margin in each state for the 2020 presidential election? One way we can tackle this challenge is by creating a model with each state's history of voting for Republican and Democratic candidates, and feeding the most recent 2020 polling data into this model to produce a prediction. 

There are a few changes that can be made to refine our approach. The first is to use a logistic model rather than the typical linear model. Unlike linear models, logistic functions have an upper and lower bound. This avoids the issue of "out of support" predictions, or predictions that are outside the bounds of contextual reason, such as predicting a voteshare greater than 100%. We can also create several simulations with our models to produce a distribution of predictions, rather than relying on a single point estimate. 

### Predicted Win Margin in New Jersey 

![](../figures/njbidenwinmargin.jpg)

The distribution of these predictions, created by generating 10,000 binomial simulations of the data, predicts Biden to win by a margin of 22.5% percentage points in New Jersey this coming November. This makes sense in the context of New Jersey, a state that consistently goes blue for presidential elections. 

### Predicted Win Margin in the U.S.

![](../figures/geofacet.jpg)

By conducting the same process, we can observe the prediction distributions for each individual state. Some states, such as Vermont, don't display a prediction because there isn't sufficient historical or current polling data available. Here, we can see how key battleground areas like Florida, Pennsylvania, and Michigan have a distribution that is centered closely to 0. Biden does not have a clear win or loss margin due to their uncertainty as swing states, with a margin of -2.4, -0.55, and 1.7 for each state, respectively.

It's clear that not all of these predictions seem accurate. In Texas, for example, Biden has a predicted win margin of about 10%. Although Texas is arguably a battleground state, it is not likely that Biden will win by a margin this large in a state that historically votes Republican for presidential elections. Similarly, in Mississippi, a firmly Republican state, this model predicts that Biden will have a large win margin of 20%. For the same reasons, this is very likely untrue and raises suspicion about the performance of this model. This model could likely be improved by the weighting polls included in the model based on their prior accuracy and incorporating fundamental aspects like unemployment rates.
