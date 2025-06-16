# Linear-Regression-Analysis_E-commerce-Store-Data-Analysis

# Background
This is an e-commerce analysis for a store which offers in-store style and clothing advice sessions. Customers come in to the store, have sessions/meetings with a personal stylist, then they can go home and order either on a mobile app or website for the clothes they want. The business is trying to decide whether to focus their efforts on their mobile app experience or their website.

# Objective
With the use of linear regression, the anaylsis aims to help the business determine which of the two channels are generating more revenue.

# About the dataset
The dataset was retrieved from [Kaggle](https://www.kaggle.com/datasets/kolawale/focusing-on-mobile-app-or-website/data). It contains the following information:
* Avg. Session Length: Average session of in-store style advice sessions.
* Time on App: Average time spent on App in minutes
* Time on Website: Average time spent on Website in minutes
* Length of Membership: Number of years the customer has been a member with the business.

# Approach
Performed EDA to understand the correlation between all variables. This can be used to validate results from the regression model.

Split the data into training and testing data at 70% and 30% respectively then fitting the data to the linear model and perform model training.

After model training, the unseen data (X_test) is fitted to the model to generate prediction values of the repsonse variable.

The model performance is evaluated using evaluation metrics such as MAE, MSE and RMSE which gives an overall assessment of how off the predictions are from the actual values. Residual analysis was also conducted as part of the model evaluation to verify whether the residuals (i.e., the differences between actual and predicted values) follow a normal distribution — which would indicate that the model errors are randomly distributed (spread around zero, both positive and negative without structure) and generally small across all data points.

