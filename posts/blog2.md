## Do Georgians Care More About the Local or National Economy?

_By Miroslav Bergam_

_September 18th, 2020_

### Voting based on the economy

In presidential elections, do voters in Georgia care more about the local or national economy when assessing the incumbent party's performance in office and casting their vote for a new leader? For which major party does retrospection on the economy matter more in Georgia?

[Retrospective theory](https://hollis.harvard.edu/primo-explore/fulldisplay?docid=TN_cdi_askewsholts_vlebooks_9781400888740&context=PC&vid=HVD2&search_scope=everything&tab=everything&lang=en_US) is the concept of basing one's vote on the results of the previous administration's efforts in office. This practice spares voters of feeling that they cast uninformed votes, as one doesn't need a wealth of technical knowledge to see how things changed under the previous administration. This leads to a level of *retroactive accountability* on the part of the incumbent, who want voters to reflect on their impact positively so they vote for them or their party again. 

One form of retrospective voting is voting based on the economy, as an individual can easily measure how personal, local, or even national finances have changed under the last administration based on a host of metrics. One metric commonly used to determine the economic efficacy of an administration is [unemployment rates](https://www.jstor.org/stable/10.1017/s0022381614000437). 

### Election Year or Full Term?

When assessing unemployment, recent memory wins in the minds of voters. Rather than assessing overall changes in the economy during all four years of the incumbent party's leadership, voters care more about the [last two quarters](https://journals.sagepub.com/doi/abs/10.1177/1532673X01293008) before the election (Q1 and Q2 of election year). This is known as the [end-heuristic](https://hollis.harvard.edu/primo-explore/fulldisplay?docid=TN_cdi_gale_infotracacademiconefile_A354446646&context=PC&vid=HVD2&search_scope=everything&tab=everything&lang=en_US): either subconsciously or for lack of ability to assess long term economic information, voters substitute a full four-year reflection on the economy for its most recent developments. 

Let's return to our guiding question: do voters care more about their state or national economy when choosing who they vote for? To measure this, we'll model the both the unemployment rate of a specific state, Georgia, and the national unemployment rate against the two-party vote share for the incumbent presidential party in Georgia. We will use the average unemployment rate during the first two quarters of the election year as our predictor for both plots because of what we know about voter's tendency to disproportionately weigh the final two quarters of the economy over the last four years. 

### State vs. national Unemployment

![](../figures/usunemployed.jpg)

When modeling the national unemployment rate against Georgia's voteshare for the incumbent presidential party, we can observe a weak, negative correlation. There is a correlation of -0.015, meaning that with each one percent increase in national unemployment, the incumbent party voteshare decreases by -0.015%. This negative correlation is intuitive: if the unemployment rates are higher at the end of a presidential term, voters in Georgia (and likely everywhere) would be less inclined to vote for that candidate's party again. However, this is a very weak correlation, with an $R^2$ value of 0.008. We can see if voters care more about state-level unemployment (and if there is a stronger correlation between the two) by replacing the national unemployment rate with Georgia's own unemployment rate as the predictor variable. 

![](../figures/GAunemployed.jpg)

This correlation appears to be slightly stronger and slightly more negative. There is a correlation of -0.066, meaning that with each one percent increase in Georgia's unemployment rate, the incumbent party voteshare decreases by -0.066%. For the same reason as before, this negative relationship makes sense. This model has a $R^2$ value of 0.11, which is notably stronger than the last relationship but still quite weak. 

### The effect of unemployment on voting by party

Perhaps the effect of unemployment on voting is correlated more strongly with which party is the incumbent. Let's graph the same data, but run two linear regressions: one for elections in which the Republican party was incumbent and one for election in which the Democratic party was incumbent. 

![](../figures/usunemployed_party.jpg)

This plot tells us a much different story. The negative correlation seen earlier does not exist for Democratic incumbents, while the correlation is even more negative for Republicans than in the previous model using national unemployment data, with a -0.5% decrease in Georgian's voteshare for each percentage point of unemployment. The correlation, too, is stronger: an $R^2$ value of 0.21. 

Let's see how these relationships change when we replace national unemployment with unemployment in Georgia. 

![](../figures/GAunemployed_party.jpg)

Once again, the correlation for Democrats is no longer negative. However, the correlation for Republicans is even stronger and more negative. For each one percent increase in Georgia's unemployment rate, the incumbent Republican candidate's voteshare in Georgia decreases by 0.1%. This relationship has a moderately strong $R^2$ of 0.72, notably stronger than any of the previous relationships. 

Both of these graphs aligns with an interesting finding in [Burden and Wichowsky (2014)](https://www.jstor.org/stable/10.1017/s0022381614000437): that Republican incumbents are more susceptible to a loss of votes due to high unemployment rates. 

### Conclusions and Model Limitations

Based on these models, it seems that voters in Georgia care more about state-level unemployment than national unemployment when deciding whether or not to vote for the incumbent party, but only when the incumbent party is Republican. This is in keeping with the findings of [Burden and Wichowsky (2014)](https://www.jstor.org/stable/10.1017/s0022381614000437), which concludes that Republicans incumbents have more to lose from high unemployment rates during their term in office. 

There are several limitations to this model. The first is that these findings cannot be generalized to different states. These models were generated using data on Georgian voters, therefore, while it may be true that several other states experience a similar trend, these analysis must be run on another state's voting data to draw this conclusion. Additionally, most of the relationships in these models had weak $R^2$ values, with the exception of modeling Georgian unemployment against Republican incumbent vote share. Thus, these findings should be taken cautiously. Individuals rarely vote solely on unemployment rates: these models can be improved and the role of unemployment in voting can be better understood by constructing a more comprehensive model with more predictors.