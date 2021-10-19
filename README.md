The relevant code for deliverables can be found under AlphabetSoupCharity.ipynb and AlphabetSoupCharity_Optimization.ipynb. The relevant .h5 files can be found under the same name.

Disregard the untitled files. 

I apoligize for the repository being so unorganized. 

# Neural_Network_Charity_Analysis


## Overview
In this assignment, I used my knowledge of machine learning and neural networks to create a binary classifer capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results

### Data Preprocessing
- The variable/column 'IS_SUCCESSFUL' is considered the target for our model

- The columns 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', and 'ASK_AMT' are the features for our model. 

When optimizing the model I decided to try the neural network with the 'SPECIAL_CONSIDERATIONS' column dropped. In these cases this would no longer be a feature.

- The variables 'EIN' and 'NAME' are neither targets nor features, and should be removed from the input data.

### Compiling, Training, and Evaluating the model
- The model consisted of 2 hidden layers with 80 and 30 neurons, respectively. And the input data had 43 features consisting of 25,724 samples. I used the 'relu' activation funciton for both hidden layers and the 'sigmoid' activation function for the output. 

- Using the above info, I was not able to reach 75% accuracy in the model. I was unable to reach 75% with any of the adjustments that I made.

- To try and increase the model performance I first dropped the 'SPECIAL_CONSIDERATIONS' column. In my next attempt I decide to add another hidden layer consisting of 10 neurons. After this I tried to increase the no. of neurons in each of the layers. And in my last attempt I changed all the activation functions of the hidden layers to be 'tanh', but kept the activation layer 'sigmoid'.  None of these attempts cause my models performance to substantially change, and I was unable to reach 75% accuracy.

## Summary
My deep learning neural network never reached 75% accuracy in any of my 5 attempts. I suppose I could have tried changing the number of epochs, dropping other columns, or using different activation functions to reach this threshold, but that seemed excessive for this particular exercise.
A different model may be able to succeed in reaching 75% accuracy. I might recommend trying a supervised machine learning model. The Random Forest model, for instance, might be successful in combining decision trees to generate a more accurate model. It would at least be worthwhile to compare its output against our deep learning model.
