# Healthcare_Provider_Fraud
Fraud detection with Graph Analytics: Leveraging network structure to increase predictive performance

# Problem Statement:
1. Identifying potentially fraudulent providers by analyzing their filed claims
2. Determining key variables crucial for detecting suspicious behavior among providers

# Common Fraudulent Problems:
There are four main types of fraud that are majorly present in the healthcare sector:
1. Billing a service not actually provided
2. Submitting multiple claims for the same service
3. Misrepresenting the service provided
4. Overcharging for a service beyond what was provided

# Data Used:
Inpatient claims, Outpatient claims and Beneficiary details of each provider

# Modelling:
Scenario 1 - Baseline: Information about claim and patient
Scenario 2 - Baseline + Graph's Features: Degree of nodes representing provider as well as physicians, closeness centrality, eigenvector centrality and BiRank
Scenario 3 - Baseline + Graph's Features + Modularity class community algorithm

![image](https://github.com/meghavi1610/Healthcare_Provider_Fraud/assets/56384838/a78dac6a-d2c9-4c78-afa6-f1f5000139b4)


We used random forest and gradient boosting - split the dataset into training and test dataset and look at the AUC score and see what performs the best.

# Results:
We see a significant increase when we use the graph features as compared to the baseline features. The AUC increases to around 0.92 from 0.68.

# Similar fraud detection algorithms can be used in banks and financial instutions which are more nuanced as compared to just using the base features.
