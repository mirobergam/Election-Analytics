## Local vs National Economy to Predict Voting Behvaior

_By Miroslav Bergam_

_September 18th, 2020_

### Voting based on the economy

Do voters in Georgia care more about the local or national economy when assessing the incumbent party's performance in office and casting their new vote? For which major party does retrospection on the economy matter more?

[Retrospective theory](https://hollis.harvard.edu/primo-explore/fulldisplay?docid=TN_cdi_askewsholts_vlebooks_9781400888740&context=PC&vid=HVD2&search_scope=everything&tab=everything&lang=en_US) is the concept of basing one's vote on the results of the previous administration's efforts in office. This practice spares voters of feeling they cast uninformed votes, as one doesn't need a wealth of technical knowledge to know how things changed for them under the previous administration. This leads to a level of *retroactive accountability* on the part of the incumbent, who want voters to reflect on their impact positively so they vote for them or their party again. 

One form of retrospective voting is voting based on the economy, as an individual can easily measure how their personal, local, or even national financial status has changed under the last administration based on a host of metrics. One metric commonly used to determine the economic efficacy of an administration is [unemployment rates](https://www.jstor.org/stable/10.1017/s0022381614000437). 

### Election Year or Full Term?

When assessing unemployment, recent memory wins in the minds of voters. Rather than assessing overall changes in the economy during all four years of  the incumbent party's, voters care more about the [last two quarters](https://journals.sagepub.com/doi/abs/10.1177/1532673X01293008) before the election (Q1 and Q2 of election year). This is known as the [end-heuristic](https://hollis.harvard.edu/primo-explore/fulldisplay?docid=TN_cdi_gale_infotracacademiconefile_A354446646&context=PC&vid=HVD2&search_scope=everything&tab=everything&lang=en_US): either subconsciously or for lack of ability to assess long term economic changes, voters substitute a full four-year reflection on the economy for its most recent state. 

Let's return to our guiding question: do voters care more about their state or national economy when choosing who they vote for. To measure this, we'll model the both the unemployment rate of a specific state, Georgia, and the national unemployment rate against the two-party vote share for the incumbent party in Georgia. We will use the average unemployment during the first two quarters of the election year as our predictor for both plots because of what we know about voter's tendency to disproportionately weigh the final two quarters of the economy before the election.

### National unemployment

![](../figures/usunemployed.jpg)

### New Jersey unemployment

![](../figures/GAunemployed.jpg)

### Party

An interesting finding in [Burden and Wichowsky](https://www.jstor.org/stable/10.1017/s0022381614000437) is that Republican incumbents are more harmed by higher unemployment rates. If we create two linear models -- one that depicts how 

![](../figures/usunemployed_party.jpg)

![](../figures/GAunemployed_party.jpg)

### Model Limitations

