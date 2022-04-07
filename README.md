# Credit_risk_model
This is the credit risk model development processflow and how it was created

1. Data Collection - Bureau Data and non-Bureau data
2. Feature Engineering and all the existing features - 600 total features
3. Weight of Evidence is used to treat the missing values and to encode the Categorical variables because it allows the linear relationship with the target variable, it has a linear relationship with log of odds.
4. Now we need to reduce the dimentions so we use Information Value and apply a cut off of 10% and above.
5. We now have 200 features and then we do some clustering and correlation analysis and then pick the ones with more IV
6. We come down to 60 features and then used Business intelligence to narrow them down to 30 variables
7. Then applying VIF to check for multicolinearity and further reduce the variables to around 10 and then applying the logistic regression model.
8. We tried bagging (random forest) and boosting (xgboost) but the trade off for simplicity to predictive power was not a lot.
9. The evaluation metric was KS Metric (To be studied).

