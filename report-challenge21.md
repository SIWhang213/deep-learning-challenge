# Report on the Neural Network Model: Alphabet Soup Charity 

## Overview of the Analysis
* The purpose of this analysis is to develop a deep learning model to predict whether applicants to Alphabet Soup Charity will be successful if funded. 
* It focuses on optimizing the model's performance in terms of accuracy and loss while handling the specific characteristics of the dataset.

## Results

### Data Preprocessing:
* The target variable for the model is the "IS_SUCCESSFUL" column, representing the success of funding (1 for successful, 0 for unsuccessful).
* Features for the model are "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION",	"STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS" and 	"ASK_AMT".
* Variables like "EIN" and "NAME" are removed during preprocessing as they do not contribute to the predictive power of the model.


### Compiling, Training, and Evaluating the Model:
* First hidden layer: 80 neurons, 'relu' activation function.
* Second hidden layer: 30 neurons, 'relu' activation function.
* Output layer: 1 neuron, 'sigmoid' activation function (binary classification).


### Achievement of Target Model Performance
* I tried to achieve a target predictive accuracy higher than 75% by following the steps mentioned. However, the efforts did not yield significant improvements.

### Steps to Increase Model Performance

* Decrease the number of values for each bin.
* Drop unimportant columns based on the feature importance resulting from the Random Forest Model.
* Add one more hidden layer.
* Use different activation functions for the hidden layers.
* Early stop epochs until overfitting using EarlyStopping.

* Extra: Try ajusting the number of neurons, layers and activation functions using KerasTuner.

## Summary
* Despite the rigorous efforts to optimize the model, the target accuracy was not met. 
* Further exploration of data characteristics, feature engineering, or alternative model architectures may be necessary to achieve the desired predictive performance for Alphabet Soup Charity's funding success prediction. 
* Regular reassessment and refinement of the model based on new insights or data modifications are recommended for future improvements.
