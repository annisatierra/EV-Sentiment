# Sentiment Analysis of Electric Vehicle Policy in Indonesia

## Executive Summary
Using the Python programming language, I conducted a sentiment analysis focused on finding out public opinion on the Electric Vehicle policy. The data came from Twitter which focused on certain keywords, such as electric cars, electric vehicles, and other related terms.

This analysis was conducted by labeling the opinion data obtained into three categories, namely negative, neutral, and positive. From this data, a classification model will be trained so that if there is new data, the model will be able to group public responses into the appropriate category.

## Business Problem
There needs to be an in-depth study of public reaction to policies issued by the government as a consideration for follow-up actions that need to be taken. This analysis can be used as additional information from the public's perspective on the rapidly developing electric vehicle ecosystem in society. Knowing what topics are being discussed on social media is also crucial. This is because we will get information about topics that are hotly discussed by the public, both those with negative and positive intentions. The existence of this information will provide an overview of public sentiment towards the issue of electric vehicles and can be used as further consideration for the government.

## Methodology
1. Perform text cleaning and pre-processing of raw text data.
2. Build a classification model that will group each tweet into three emotions (positive, negative, and neutral)
3. Visualize wordclouds for each emotion group.

## Skills
**Python:** Pandas, Matplotlib, Seaborn, Regular expression operations, building an optimal classification model, imbalance class handling, Text Processing.

## Results and Recommendation
The most optimal classification model is a model using the SVC algorithm. Indications of class imbalance are handled using resampling with the SMOTETomek technique. The model shows quite good performance in grouping tweets that have positive, neutral, or negative reactions. By choosing the F1 Weighted metric as a reference, this SVC model has a performance on the test set of **0.56** without any indication of excessive overfitting.

Wordcloud visualization helps in understanding the topics of discussion of each reaction group which are summarized into the following points:

- The majority of netizens have **neutral sentiment** (59.3%) towards the electric vehicle policy, with frequently appearing words such as battery, price, SPKLU, and Indonesia, indicating that many are still hesitant and questioning the sustainability of this policy.
- **Negative sentiment** (25.1%) is also quite prominent, with words such as subsidies, expensive, criticism, impact, pollution, and buy, indicating concerns about environmental impacts, high costs, and subsidy policies.
- Only a small proportion of netizens (15.6%) have **positive sentiment**, supporting aspects such as subsidies, warranties, appropriate prices, and tax policies, although this support is still limited.
