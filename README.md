## Bike Sharing Demand Prediction (Supervised ML- Regression)


### Problem Statement:
Bike rentals have became a popular service in recent years and it seems people are using it more often. With relatively cheaper rates and ease of pick up and drop at own convenience is what making this business thrive. 

Mostly used by people having no personal vehicles and also to avoid congested public transport which that’s why they prefer rental bikes. Therefore, the business to strive and profit more.

Our project goal is a pre planned set of bike count values that can be a handy solution to meet all demands.

![Bike-Sharing-Demand-1194x501](https://user-images.githubusercontent.com/105766113/225235557-0df410d0-7774-4327-8318-4d4309b49fe0.jpg)


### Dataset Information
Number Of Records - 8761

Number Of Attiributes - 14

### Attribute Information:

* Date : Year-Month-Day 
* Rented Bike Count - Count of bikes rented at each hour 
* Hour - Hour of the day 
* Temperature - Temperature in Celsius  
* Humidity - % 
* Wind Speed - m/s 
* Visibility - 10m 
* Dew point temperature -Celsius 
* Solar radiation -MJ/m2 
* Rainfall -mm 
* Snowfall -cm 
* Seasons -Winter, Spring, Summer, Autumn 
* Holiday -Holiday/No Holiday 
* Functional Day – NoFunc  (Non Functional Hrs), Fun (Functional Hrs)

### Target Variable:
Our target variable is "Rented Bike Count"

### Challenges:


   1. Data Cleaning
   2. Data Analysis
   3. Predict the count of rented bike 
	 
### Work Flow :

1. Importing required Libraries
 
2. Loading the dataset

3. EDA on features

4. Feature Engineering

5. Data Cleaning

6. Feature Selection

7. HyperParameter Tuning and Modeling

8. Evaluation and comparision of models

9. Selecting the best model

10. Conclusion





### Conclusion :

Started with loading the data so far we have done EDA ,feature engineering , data cleaning, target encoding and one hot encoding of categorical columns, feature selection and then model building. So far we have modelled on

1. Linear Regression
2. Lasso Regressor
3. Ridge Regressor
4. Elastic Net
5. Decision Tree Regressor
6. Random Forest Regressor
7. Gradient Boost Regressor

As we have calculated MAE,MSE,RMSE and R2 score for each model. Based on r2 score will decide our model performance.
Our assumption: if the differnece of R2 score between Train data and Test is than 5 % we will consider it as overfitting

On Gradient Boost regressor model, without hyperparameter tuning we got r2 score as 98% on training data and 90% on test data. Thus our model memorised the data.So it was a overfitted model, as per our assumption
After hyperparameter tuning we got r2 score as 90% on training data and 87% on test data which is very good for us. # Gradient Boosting Regression(Gradient Boosting Machine):
On Random Forest regressor model, without hyperparameter tuning we got r2 score as 86% on training data and 85% on test data.Our model performed well without hyperparameter tuning.
After hyperparameter tuning we got r2 score as 96% on training data and 91% on test data,thus we improved the model performance by hyperparameter tuning.

### Thus Gradient Boosting Regression(GridSearchCV) and Random forest(gridSearchCv) gives good r2 scores. We can deploy this models.


![regression](https://user-images.githubusercontent.com/105766113/225238367-30adb000-7603-41cd-9d2a-b91571c81629.png)


### Certificate-

![Bike sharing demand prediction project](https://user-images.githubusercontent.com/105766113/225239417-64ae7c99-7807-4ca4-a155-4d2c21b04848.png)

