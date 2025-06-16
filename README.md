# Linear Regression Analysis - E-commerce Data

# Background
This is an e-commerce analysis for a store which offers in-store style and clothing advice sessions. Customers come in to the store, have sessions/meetings with a personal stylist, then they can go home and order either on a mobile app or website for the clothes they want. 

# Objective
The business is trying to decide whether to focus efforts on their mobile app experience or their online website. With the use of linear regression, the anaylsis aims to help the business determine which of the two channels is yielding higher customer yearly expenditure.

# About the dataset
The dataset was retrieved from [Kaggle](https://www.kaggle.com/datasets/kolawale/focusing-on-mobile-app-or-website/data). It contains the following information:
* Avg. Session Length: Average session of in-store style advice sessions.
* Time on App: Average time spent on App in minutes
* Time on Website: Average time spent on Website in minutes
* Length of Membership: Number of years the customer has been a member with the business.

# Libraries used
* sklearn
* pandas
* matplotlib
* seaborn
* scipy
  
# Approach
1. EDA <br>
Performed EDA to understand the correlation between all variables. This can be used to validate results derived from the regression model.

2. Train Test Split <br>
Split the data into training (70%) and testing (30%) data and fit the training data (X_train, y_train) to the linear model for model training.

3. Model Training <br>
Training the model using the training data (X_train, y_train).

4. Generating Predictions <br>
After model training, the model is used to generate predictions of the response variable using the testing data (X_test).

5. Model Evaluation <br>
The model performance is evaluated using evaluation metrics such as MAE, MSE and RMSE which gives an overall assessment of how off the predictions are from the actual values. Residual analysis was also conducted as part of the model evaluation to verify whether the residuals (i.e., the differences between actual and predicted values) follow a normal distribution — which would indicate that the model errors are randomly distributed (spread around zero, both positive and negative without structure) and generally small across all data points.

# Key Findings
The length of membership appears to be the most significant factor on the yearly amount spent by customers. However, comparing between the amount of time spent on the mobile app vs time spent on website, the time spent on website almost has no correlation to the yearly amount spent. On the other hand, time spent on mobile apps have a relatively large influence.

# Future Works
Additional data about the products that customers purchased through the mobile app can be collected and included in the dataset. Clustering can be performed to cluster customers in terms of the product categories they spend on and their spending habits such as purchased amounts and frequency. With such insights, the business can create personalized advertisements targeted towards each cluster of customers. By providing a personalized shopping experience, customers could feel more valued and this can benefit the business by ensuring customer retention.
