# Neural_Network_Charity_Analysis
 
## Overview off Analysis
Using machine learning and neural networks, use the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results
### Data Preprocessing
#### What variable(s) are considered the target(s) for your model?
- IS_SUCCESSFUL—Was the money used effectively
 
#### What variable(s) are considered to be the features for your model?
- APPLICATION_TYPE—Alphabet Soup application type
  
- AFFILIATION—Affiliated sector of industry

- CLASSIFICATION—Government organization classification
  
- USE_CASE—Use case for funding
  
- ORGANIZATION—Organization type
  
- STATUS—Active status
  
- INCOME_AMT—Income classification
  
- SPECIAL_CONSIDERATIONS—Special consideration for application
  
- ASK_AMT—Funding amount requested
      
#### What variable(s) are neither targets nor features, and should be removed from the input data?
- EIN and NAME—Identification columns

### Compiling, Training, and Evaluating the Model
#### How many neurons, layers, and activation functions did you select for your neural network model, and why?
- Layer one (1) has 80 neurons and activation function 'relu'
- Layer two (2) has 30 neurons and activation function 'relu'
- Outer layer has activation function 'sigmoid'

#### Were you able to achieve the target model performance?
- The target model performance of 75% was not achieved. My model achieved an accuracy of 73%

#### What steps did you take to try and increase model performance?
- Optimization 1
  Added additional hidden layers and neurons:
  - Layer one (1) has 100 neurons and activation function 'relu'
  - Layer two (2) has 50 neurons and activation function 'relu'
  - Layer three (3) has 20 neurons and activation function 'relu'
  - Outer layer has activation function 'sigmoid'
 The target model performance of 75% was not achieved. This model achieved a lower accuracy of 72%
  
  

## Summary
