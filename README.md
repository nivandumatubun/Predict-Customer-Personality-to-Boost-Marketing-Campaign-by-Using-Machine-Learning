# **Predict Customer Personality to Boost Marketing Campaign by Using Machine Learning**

## Overview
A company can develop rapidly when it knows its customers' personality behavior, so that it can provide better services and benefits to customers who have the potential to become loyal customers. By processing historical marketing campaign data to improve performance and target the right customers so they can make transactions on the company's platform, from this data insight our focus is to create a cluster prediction model to make it easier for companies to make decisions.

## Objective
- Analyze Customers' Behavior on Campaigns
- Generate Cluster Prediction Model

[Documentation Detail](https://github.com/nivandumatubun/Predict-Customer-Personality-to-Boost-Marketing-Campaign-by-Using-Machine-Learning/blob/master/Pdf%20predict%20customer%20personality.pdf)

### Data Preparation
- Fill Data Null
- Drop Unnecessary Data

### Feature Engineering
- Age & Group Age
- Datetime
- Total Children & Parents
- Total Spending
- Total Accepted Campaign
- Total Transaction
- Conversion Rate

### Exploratory Data Analysis
- Initial EDA
  - Conversion Rate Based on Marital Status
  ![marital_vs_cvr.png](https://github.com/nivandumatubun/Predict-Customer-Personality-to-Boost-Marketing-Campaign-by-Using-Machine-Learning/blob/master/marital%20vs%20cvr.png)

  - Conversion Rate Based on Age (Group Age)
  ![age_vs_cvr.png](https://github.com/nivandumatubun/Predict-Customer-Personality-to-Boost-Marketing-Campaign-by-Using-Machine-Learning/blob/master/age%20vs%20cvr.png)

### Modelling (Clustering)
- Elbow Method
![elbowmethod.png](https://github.com/nivandumatubun/Predict-Customer-Personality-to-Boost-Marketing-Campaign-by-Using-Machine-Learning/blob/master/elbowmethod.png)

- Cluster Segmentation
![cluster.png](https://github.com/nivandumatubun/Predict-Customer-Personality-to-Boost-Marketing-Campaign-by-Using-Machine-Learning/blob/master/cluster.png)

### Evaluation
![silscore.png](https://github.com/nivandumatubun/Predict-Customer-Personality-to-Boost-Marketing-Campaign-by-Using-Machine-Learning/blob/master/silscore.png)

### Cluster Analysis
![clusterdist.png](https://github.com/nivandumatubun/Predict-Customer-Personality-to-Boost-Marketing-Campaign-by-Using-Machine-Learning/blob/master/clusterdist.png)

#### Cluster Summary
1. **Risk of Churn** :
- This group is the group with the largest number of users, approximately 800 people, dominated by middle_aged_adults (36-55 years), who are predominantly married and have 1 child.
- In terms of income and expenses, this group has the smallest income and expenses each month, which are respectively IDR 33.4 million for total income a year, and IDR 53K for expenses per year
However, this group is ranked first as the group that visits the web most frequently with a median total of 7 visits a month, however, they still rarely make transactions and even use promos for their transactions.
- Apart from that, this group is the group that rarely or almost never receives campaigns.

2. **Low Spender** :
- This group is dominated by older_adults (>55 years) and middle_aged_adults (36-55 years), who are predominantly married and have 1 child.
- This group visits the website quite often, second most frequently after Cluster 0, with a median of 6 times a month, however, this group rarely receives campaigns.
- However, this group has the second smallest total income and expenses compared to other groups, which are respectively IDR 49 million for total annual income, and IDR 319K for annual expenses.

3. **Mid Spender** :
- This group is dominated by older_adults (>55 years) and middle_aged_adults (36-55 years), who are predominantly married and have 1 child.
- This group visits the website quite often, second most frequently after Cluster 0, with a median of 6 times a month, however, this group rarely receives campaigns.
- However, this group has the second smallest total income and expenses compared to other groups, which are respectively IDR 49 million for total annual income, and IDR 319K for annual expenses.

4. **High Spender** :
- This group is the group with the second largest number of users, 619 people, dominated by older_adults (>55 years) and middle_aged_adults (36-55 years), the dominant of whom are unmarried and do not have children.
- In terms of income and expenses, this group has the largest income and expenses each month, each amounting to IDR 70 million for total income a year, and IDR 1.1 million for expenses a year.
- This cluster is quite a lot of non-organic by responding to campaigns, but has the lowest number of promo uses compared to the others.
- This group is the group that has the largest conversion rate for purchasing our products, and we must not lose them.

### Recommendation and Potential Impact
**Recommendation**
1. Continue to monitor transactions and retention from the High Spender group. Focus on improving service so that this group does not churn
2. For the Mid Spender group, further analysis can be carried out on how to increase their transactions by providing more personalized recommendations, as well as deeper analysis on how to optimize promos in this segment and keep shopping on our platform.
3. For the Low Spender and Risk to Churn groups, further analysis can also be carried out on how to increase the visit to transaction conversion ratio. They have a fairly high number of visits but do not make transactions. This can be caused by unsuitable products or prices.

**Potential Impact**
1. If we focus on continuing to monitor the High Spender group, we will still get a potential GMV of **IDR 691 million**, while for the Mid Spender group it is **IDR 387 million**.
2. If we can optimize the promos spent on Mid Spenders (assuming a 50% reduction) we can reduce costs by around **IDR 50 million**.
