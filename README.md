# credit_card_churning
A detailed analysis about credit card data and attrition around same

# Requirements
Python 3.8+
Jupyter Notebook - Kaggle Notebook is preferrable

# Dataset
Credit Card Customers - https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers

# How to Run The Notebook.
1. Login to Kaggle.com
2. Visit https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers link
3. Click on "New Notebook" Option Available on the top of the screen.
4. Download the ".ipynb" File attached in the current repository, select the right version
5. Upload On the New Notebook place by clicking on Import Notebook option.
6. Run The Notebook program

# Key Data Insights

1. Figure 1 Depicts the Gender distribution, data is almost half split in terms of male and female, which is a good sign of having a balance data.
2. Figure 2 and 3 covers around age and dependent count distribution, data is normally distributed. Normally distributed data let machine learning models perform well in analysing the underline patterns.
3. Figure 4 depicts Marital Status, which is almost equally distributed among married and single, or even Divorced and unknown.
4. Customer age and total revolving balance data is analysed by comparing through credit limit, People aged between 35 to 55 has been allocated better credit limit in comparison to reverse age bracket. - Figure 5
5. Less than 20000 credit limit customers, maintaining 500 to 2500 of total revolvng balance, and most of the customers are concentrated in this reason only - Figure 6
6. Figure 7 depicts the credit limits relation with income category, people with less than 40K income are capped with credit limit of around 15000 and those whose income ranges between 40K to 60K are capped to have a credit limit of around 25000. Rest who is making more than 60K enjoying the max credit limit of 35000. However there are small credit limit for more than 60K income bracket.
7. Figure 8 and 9 covers around covers around transaction count and transaction amount, there has been a significant drop in people between 50 to 60. Rest data ahs been stable between 40 to 55 age group along with certain floor and shieling points.

# Business Insights

1. People whose age are between 30 to 60 and allocated a credit limit of 5000 are high risk customer and their attrition rate is very high. This Strata need to be monitored closely and understand other data patterns which can reduce risk in that segment.
2. People age between 40 to 50 and being assign with credit limit of 5000 to 10000 also show some major attrition rate and need a proper analysis around it. Both point 1 and 2 observed in Figure 11.
3. Customers whose transation is in between 0 to 4000 and assign with credit limit less than 10000 can be consider as high attrition zone and must be monitored properly.
4. People who spends more than 12000 can be cosidered as high worth premium customers and there are attrition almost near to 0. Getting customers in this segment by identifying other data metrics align with them covering salary, age i.e and onboarding them can improve business growth. Points 3 and 4 explained using Figure 12.
5. As per Figure 13, Customer with Transaction count more tha 80 are likely to be stable and has almost less than 1 percent attrition rate.
Using same figure, Customer with less than 80 Transactions and having a credit limit of less than 10000 are high rist cutomers, among them, in between 20 to 60 transacting customers with limit in less than 5000 must be closely monitored

# Model Performance

5 Models has been trained and there result has been published below.

1. Model1 - Accuracy 96.7 % - Random Forest
2. Model2 - Accuracy 93.6 % - Decision Tree
3. Model3 - Accuracy 89.1 % - Logistic Regression
4. Model4 - Accuracy 89.3 % - Naive Bayes
5. Model5 - Accuracy 97.4 % - XGBoost

Best Model as per below accuracy results can be considered as XGBoost and Random Forest as the second best model.

# Ethics Report
1. Model 5 i.e, XGBoost has less bais towards ethics necessity which includes Age, Marital Status, Education Level and Gender.
2. Females are to an extent more biased towards attrition, but considered Existing than male across all the models.
3. Marriage data is more understood by XGBoost and fitted properly compared to other models
4. In terms of Education, Post Graduated and High School customers are expected to be more biased. with even best model chances are more than 15 %.
5. People aged between 60 to 69 are having chances of wrongly predicted as existing compare to other age segment people.
6. Maximum concern Area is Age biasness and highest is being seen in between 60 to 69 with Logistic Regression Model usage which is around 62 %. 
