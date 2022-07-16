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

![define model](https://user-images.githubusercontent.com/100816778/179341875-07189e00-f567-4d72-bde2-35098352aa4a.png)

#### Were you able to achieve the target model performance?
- The target model performance of 75% was not achieved. My model achieved an accuracy of 73%

![accuracy1](https://user-images.githubusercontent.com/100816778/179341879-d85dbad0-3b02-4bae-9a1d-51e2fda69d15.png)

#### What steps did you take to try and increase model performance?
- Optimization 1
  Added additional hidden layers and neurons:
  - Layer one (1) has 100 neurons and activation function 'relu'
  - Layer two (2) has 50 neurons and activation function 'relu'
  - Layer three (3) has 20 neurons and activation function 'relu'
  - Outer layer has activation function 'sigmoid'

![define model 2](https://user-images.githubusercontent.com/100816778/179341946-0b496990-1fd8-4d3d-b11f-b8a5398ff86e.png)
  
  The target model performance of 75% was not achieved. This model achieved a lower accuracy of 72%
  
![accuracy2](https://user-images.githubusercontent.com/100816778/179341968-a3a95f93-cb69-486d-ba13-58e66c01e443.png)
  
 - Optimization 2
   The hidden layers and neurons stayed the same, however layer 3 activation function was changed to 'tanh':
   - Layer one (1) has 100 neurons and activation function 'relu'
   - Layer two (2) has 50 neurons and activation function 'relu'
   - Layer three (3) has 20 neurons and activation function 'tanh'
   - Outer layer has activation function 'sigmoid'
   Additionally, 'AFFILIATION' column was removed.
   
![define model 3](https://user-images.githubusercontent.com/100816778/179342055-5c99ca85-565c-4601-b817-5412cc19935c.png)
   
![removecolumn](https://user-images.githubusercontent.com/100816778/179342057-f9a59af0-4941-4adf-8719-665de5b67e3d.png)
   
   The target model performance of 75% was not achieved. This model achieved an even lower accuracy of 66%
   
![accuracy3](https://user-images.githubusercontent.com/100816778/179342064-2c473a56-8964-469c-84c6-53356625e4c4.png)

## Summary
The initial model had the highest accuracy score of 73%. With two attempts at optimization, the accuracy score dropped to 72% and 66%. Random Forest could be used because it combines multiple smaller models into a more robust and accurate model. Random forest models use a number of weak learner algorithms (decision trees) and combine their output to make a final classification (or regression) decision.
