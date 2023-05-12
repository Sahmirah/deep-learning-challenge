# Deep Learning Challenge

## Overview 
The purpose of this analysis was to create a neural network and predict the best applicants for Alphabet Soup to provide funding for on the basis that the applicant will be successful. I received a CSV with more than 34,000 organiations that have received funding from Alphabet Soup over the years. The dataset columns included: 

* EIN and NAME—Identification columns
* APPLICATION_TYPE—Alphabet Soup application type
* AFFILIATION—Affiliated sector of industry
* CLASSIFICATION—Government organization classification
* USE_CASE—Use case for funding
* ORGANIZATION—Organization type
* STATUS—Active status
* INCOME_AMT—Income classification
* SPECIAL_CONSIDERATIONS—Special considerations for application
* ASK_AMT—Funding amount requested
* IS_SUCCESSFUL—Was the money used effectively

## Results

### Data Preprocessing

1. What variable(s) are the target(s) for your model?

* IS_SUCCESSFUL is the target for my model. When it is 1 that means the applicant was successful, and 0 mean unsuccessful. 

2. What variable(s) are the features for your model?

* APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and ASK_AMT are my features.  

3. What variable(s) should be removed from the input data because they are neither targets nor features?

* The variables I removed were EIN and Name. 

### Compiling, Training, and Evaluating the Model

1. How many neurons, layers, and activation functions did you select for your neural network model, and why?

* For my model, I used 4 hidden layers. My first hidden layer has 50 neurons and I used the relu activation. My second hidden layer has 50 neurons and I used the tanh activation. My third hidden layer has 30 neurons and I used the relu activation. My fourth hidden layer has 20 neurons and I used the tanh activation. I optimized my model several times and tried several different neurons and activations, but the highest accuracy I was able to attain was 73% I realized that the more I decreased the neurons the higher the accuracy, however, I was unable to achieve 75%

2. Were you able to achieve the target model performance?

* I was unable to achieve the target model performance of 75% I achieved 73% accuracy. 

3. What steps did you take in your attempts to increase model performance?

* I increased the number of epochs to 125 in order to increase the model performance. I also added 4 hidden layers. 

## Summary

Overall, this model is okay to use in order to predict the success of applicant being funded. However, I believe that decreasing the neurons and increasing the number of epochs may be able to garner a higher accuracy level. I also recommend adding another hidden layer to better create a higher accuracy prediction. 
