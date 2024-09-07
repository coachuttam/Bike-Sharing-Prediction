
# <b style='color:red;'>Build a multiple linear regression model for the prediction of demand for shared bikes</b>
![image](https://github.com/user-attachments/assets/8d1d68ab-48da-4cef-83eb-29c49d2a3016)



## Problem Statement : 
Due to the ongoing corona pandemic in the US, the revenues of bike-sharing company BoomBikes have taken a hit. The company is now struggling to maintain its operations due to the current market conditions. It has therefore decided to create a business plan to boost its sales once the situation improves.
To understand the demand for its services, BoomBikes is currently working on developing a demand model that can analyze the various factors that affect its business. The company is planning on responding to the needs of its customers once the COVID-19 pandemic ends.
To gain a deeper understanding of the demand for its services, the company has contracted a consulting firm to analyze the factors that affect its business.

- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands

Through the collected data, the company has been able to identify the daily bike demands in the US.

## Goal: 
The demand model must be created with the help of independent variables. It can be used by the business to determine the exact demands that the company encounters, as well as the ways in which it can meet those demands. In addition, it can help management understand the dynamics of the new market.

## Data Preparation: 
In the data dictionary, you can see that certain variables, such as "weathersit" and "season," have numerical values ranging from 1, 2, and 3 to 4, which correspond to labels. These values might indicate that there's an order to them, but it's not the case.
- Before starting the model development process, it's important that the feature values are converted into a set of categorical string values. This will help the business understand the various independent variables.

## Model Bulding:
The data dictionary shows three main variable types: "casual," "registered," and "cnt." The former indicates the number of casual users who made a reservation, while the latter shows the total number who booked a bike on a given day, both registered and casual. The model should then build a representation of this variable in the form of "cnt," which indicates the overall bike rental count.

## Model Evaluation: 
After you've finished building the model and made predictions on its test set, you can refer to the following code to calculate the R squared score.

from sklearn.metrics import r2_score

r2_score(y_test, y_pred)

The y_test and y_pred variables represent the test data sets for the target variable and the predicted values, respectively.
You must perform this step to ensure that the R-Squared score is consistent with the test set's results. The variable names in the function r2_score can also be customized based on the ones you've selected.
