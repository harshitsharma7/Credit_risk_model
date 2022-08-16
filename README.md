# Credit_risk_model
This is the credit risk model development processflow and how it was created

1. We need all the features in categorical format so that we can make sense of it more easily and calculate and adjust the scores easily.
2. Data Collection - Bureau Data and non-Bureau data
3. Feature Engineering and all the existing features - 600 total features
4. We do feature elimination based on the covariance of features with each other and with dependent variable.
5. Do other small checks like missing value rate.
7. Then we apply RFE using random forest as the base estimator to eliminate the remaining features to come down to 20 features
8. We come down to 20 features and then used Business intelligence and iv values to narrow them down to 15 variables
9. Weight of Evidence is used to treat the missing values and to encode the Categorical variables because it allows the linear relationship with the target variable, it has a linear relationship with log of odds.
10. We also create categories for the continous variables and check the bins with woe and feature importance using the iv values
11. Again did some feature selsection using Information value and then eliminated too high a scores and too low a scores
12. 
13. Logistic regression was used since the coefficient values are important to us for score card development
14. AUC ROC
Stratified K folding

Used woe for bucketing the data and converting the numerical data to categorical data as it is essential in Credit Risk Scorecard creation and easy human interpretation of the score card
