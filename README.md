# Multi-Variate-Regression-Case-Study-
## Multivariable regression pipeline to predict time taken for a package delivery business.
## Problem Statement

Regional Delivery Service, Inc. (RDS) is a small business focused on same-day delivery of letters, packages, and small items. To save time and reduce fuel costs, the company uses Google Maps to combine several deliveries into one trip. However, there’s a need to develop a reliable way to estimate delivery times based on 13 important factors that affect how long a delivery takes. Doing so will help RDS operate more efficiently and provide better service to customers.

## OBJECTIVES
- Develop a multivariable regression pipeline to predict time taken for a package delivery business.
- Develop three different models (on the basis of given set of hypotheses) and compare their performance.

## ABOUT DATA SET
- Data set has 100 rows and 14 columns
- There are 13 feature variables and 1 target variable "Time Taken"


## Hypothesis:
#### Hypothesis 1
- Including all available features in the linear regression model will provide the most accurate predictions.

#### Hypothesis 2
- A linear regression model built using only features that are significantly correlated with the target variable will outperform the model using all features, as it focuses on the most relevant predictors.

#### Hypothesis 3
- Excluding features that exhibit multicollinearity from the linear regression model will yield better performance compared to both the all-features model and the correlated features model.

## Model Evaluation

- All Features - MSE: 21.14979303890079 R-squared: 0.6471651689573914
- Correlated Features - MSE: 15.993902337563748 R-squared: 0.7331791465473565
- No Multicollinearity - MSE: 15.458541308382209 R-squared: 0.7421103931997768

## Model Comparison and Results

- Our hypothesis that we did set initially are yielding true predictions.
- For second model, when we select those features only with highest correlation with target variable,We got better R2_score: 0.73 and less MSE: 15.99 compared to model with all features,R2_score: 0.64 and MSE: 21.14
- For third model, when we excluded the features showing highest multicollinearity, we got more better results, R2_Score:0.74 and MSE:15.4 compared to second model,R2_score: 0.73 and MSE: 15.99.
