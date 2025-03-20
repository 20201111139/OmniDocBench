# Summary of datasets

|Dataset|Total size|Training items|Testing items|Continuous attributes|Nominal attributes|Total attributes|IFN|Relief|ABB| |
|---|---|---|---|---|---|---|---|---|---|---|
|Breast|699|465|234| | | | | | | |
|Chess|3196|2155|1041| |36|36|3|5| | |
|Credit|690|451|239| | |14|2| | | |
|Diabetes|768|530|238| | | |2| | | |
|Glass|214|143|71| |0| |3| | | |
|Heart|297|197|100| | |13|3|2|4| |
|Iris|150|100|50| |59| | |2| | |
|Liver|345|243|102| | |57|5|2|4| |
|Lung-cancer|32|23| |0| | | |4| | |
|Wine|178|118|60|13| |13| |2| | |
|Average| | | | | | |16.9|3.70|2.10|3.10|

Average dimensionality reduction: 78%, 88%, 82%

We have also evaluated the performance of the classification model built directly by IFN (see Section 2.3). This model is based on the same features as "C4.5 after IFN" but the model structure may be different due to the IFN restriction of using the same feature at all splits of each layer. The error rate of all models has been measured on the same validation sets. We have also calculated the lower and upper bounds of the 95% confidence interval for the error rate of C4.5 with a full set of features and compared statistically the error rates after different feature selection methods to this base error rate. The comparison was based on the normal approximation of the binomial distribution.

# 3.2. Analysis of results

The last row of Table shows the average dimensionality reduction due to each one of the feature selection methods used (IFN, Relief, and ABB): All the methods tend to remove more than 3/4 of the available features. The best dimensionality reducer is Relief; which considers as relevant only 12% of features (on average): IFN removes the least number of features (average dimensionality reduction of 78%). These results suggest that the relevance of some features to the target may be revealed only by feature selection procedure, which is able to evaluate subsets of features.