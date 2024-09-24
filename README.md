**INTRODUCTION**

In the realm of modern banking, the effective utilization of data-driven strategies is of paramount importance when optimizing marketing campaigns. With the advent of machine learning techniques, financial institutions are empowered to enhance the precision and efficiency of their marketing endeavors. This report delves into the application of machine learning methodologies in the context of a bank's direct marketing campaigns aimed at predicting customer responses to offers for long-term deposit accounts. This study seeks to provide valuable insights for strategic decision-making in banking operations by leveraging predictive analytics.

**DATA UNDERSTANDING**

The dataset was related to direct marketing campaigns of a Portuguese Bank and is available at originally in the UCI Machine Learning Repository (Moro et al. 2014).  The dataset contains 45,000 customers who received an offer to open long-term deposit account with rates attractive interest. All necessary information acquired is accessible and legitimate, including age, job, marital status, educational level, balance, and current loan status (Table 1).  

![image](https://github.com/user-attachments/assets/08f3b8b5-cfda-4c45-873b-f016987895e6)

**DATA PREPARATION**

**DATA VISUALIZATION**

*Distribution of Term Subscriptions.* The pie chart in Fig 1 depicts the distribution of term subscriptions. 53% are categorized as "Did not Open Term Subscriptions”, indicates that most of the dataset comprises individuals who did not opt for term subscriptions
![image](https://github.com/user-attachments/assets/38341b6c-7337-483e-bbf6-c4d0668a2f62)

*Age, balance, day, duration, campaign, pdays analysis.* Fig 2 presents insightful analyses of age, balance, day, duration, campaign, and pdays within the dataset. Notably, the mean age of the individuals is approximately 41 years old, with ages ranging from 18 to 95 years. Regarding balance, the dataset exhibits a mean balance of 1,528 units. However, the high standard deviation indicates significant dispersion of balance values. 
Furthermore, dropping the duration column from the analysis is advisable due to its high correlation with the likelihood of a potential client subscribing to a term deposit. Duration, obtained after contacting the potential client, becomes less relevant for clients who have not received calls. This high correlation stems from the observation that longer durations of interaction with the bank tend to correlate with higher probabilities of term deposit subscription, indicating increased interest and commitment from potential clients.
![image](https://github.com/user-attachments/assets/59b5e381-dd3f-4b19-9489-f7b38bfb00f6)

*Analysis by Occupation.* Fig 3 presents that management is the occupation that is more prevalent in this dataset and the retired are the ones who have the highest median age, while students are the lowest
![image](https://github.com/user-attachments/assets/e66ccfb7-eddf-4359-b202-313f3ea872f9)

*Analysis by Marital Status.* Fig 4 shows divorced individuals often exhibit lower financial balances (orange dots), which can be attributed to asset division during divorce proceedings.
![image](https://github.com/user-attachments/assets/b82e4ac9-596e-48bd-a501-1273a26fbef6)

*Correlation matrix analysis of the dataset.* It appears from Fig. 5 that no pair of variables are strongly correlated, thus helping to satisfy the fundamental assumption (absence of multicollinearity) of modelling. The only notable correlation observed was between pdays and previous, reflect a strategy where previously contacted clients may require additional follow-up before a new campaign; and campaign duration and term deposit uptake.
![image](https://github.com/user-attachments/assets/0b467ba5-62eb-47de-a4ae-ff60d895e2d8)

**MODELS SELECTION**

Upon executing the classification models, Table 2 depicts that the decision tree classifier exhibited signs of overfitting, as indicated by nearly perfect accuracy scores (100%). To mitigate overfitting, cross-validation emerged as the preferred approach, leveraging the overall data pattern to effectively discern whether a potential client would subscribe to a term deposit or not.
![image](https://github.com/user-attachments/assets/136f33b5-84ee-4f89-abd5-4115a6b3e6b2)

Following a comprehensive evaluation, the optimal model was selected based on a specific set of metrics, ensuring the implementation of a versatile model capable of accommodating the dynamic characteristics of data patterns. Furthermore, given the absence of personally identifiable information in the dataset, privacy considerations were upheld.

**RESULTS** 

![image](https://github.com/user-attachments/assets/36e12804-4449-49b0-a965-0acb87adc3f8)
