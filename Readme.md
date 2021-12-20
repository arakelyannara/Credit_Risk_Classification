
## Overview of the Analysis

The purpose of the Credit Risk Classification project is to find a better model to predict high-risk loans using the dataset with outnumbering healthy loans. We build the prediction based on the data from the lending_data.csv file in the Resources folder. First, we will build the Logistic Regression model on the initial data, then on oversampled data to check the metrics defining the performance of the chosen method. 

The given feaures are 'loan_size', 'interest_rate', 'borrower_income', 'debt_to_income', 'num_of_accounts', 'derogatory_marks', 'total_debt', 'loan_status'. With the help of Machine Learning tools we will try to build a model to predict the loan_status, wheater it's a healthy loan (0) or high-risk loan(1). 
The initial data contains:

* 0    75036
* 1     2500

The data will be split into training and testing sets. The Logistic Regression will use the training data to learn the pattern the data has and predict the possible outcome for future incoming data. Since the dataset is imbalanced the second method we'll be using the RandomOverSampler to resample the data and build the model on an oversampled dataset. To check the accuracy and other metrics we'll be using the previously split testing data.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:

The accuracy score of the model 1 is 0.95.

                   pre       rec    

          0       1.00      0.99    
          1       0.85      0.91  

avg / total       0.99      0.99    


* Machine Learning Model 2:

The accuracy score of the model 2 with ovesampled dataset is 0.99.

                   pre       rec      

          0       1.00      0.99    
          1       0.84      0.99     

avg / total       0.99      0.99   


## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

Based on the metrics we see above we can tell that the Model 2 sems to perform the best. From the first sight it seems that we have the same performance based on average/total figures, but once we look at how our models perform on predicting 1s(i.e the high risk loans) we will see the increase in recall (99%). Also the accuracy score increased from 95% to 99%.

## Technologies

JupyterLab web application

This project leverages python 3.7 with the following packages:

* pathlib
* pandas
* hvplot
* and sklearn machine learning library

---

## Usage


To use the Credit Risk Classification clone the repository, open it with Jupyterlab and run the 

    * credit_risk_resampling.ipynb

---
    
## Contributor

Nara Arakelyan

---

## Licence 

UC Berkley
    

