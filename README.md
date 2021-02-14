# Overview of the analysis:
The purpose of this analysis is to determine if applicants will be successful if funded by Alphabet Soup. 

Results: Using bulleted lists and images to support your answers, address the following questions.

## Data Preprocessing
- "IS_SUCCESSFUL" is considered the target variable for this model. 

- "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "INCOME_AMT", AND "SPECIAL_CONSIDERATIONS" are all features of this model.


- "EIN" and "NAME" were removed from the input data because they are neither targets not features. 

## Compiling, Training, and Evaluating the Model

Layers Used = 2

Neurons Used in Layer 1 = 80

number_hidden_nodes = number_input_features * 3

Was able to achieve accuracy of 48% in one optimization after removing "CLASSIFICATION" feature.

Removed "CLASSIFICATION" from feature list and decreased number of layers.

Used "relu" activation function in first layer for non-linear input and "sigmoid" function in output layer to achieve binary classification.


## Summary:
Following are the accuracies achieved in each optimization:

Original Code: 268/268 - 0s - loss: 1.7335 - accuracy: 0.4806
Loss: 1.7334908246994019, Accuracy: 0.4805831015110016

First Optimization: 268/268 - 0s - loss: 6.1670 - accuracy: 0.4608 Loss: 6.167031288146973, Accuracy: 04607580304145813

Second Optimization: 268/268 - 0s - loss: 7.1581 - accuracy: 0.4627 Loss: 7.158142566680908, Accuracy: 0.4627405107021332

Third Optimization: 268/268 - 0s - loss: 5.2691 - accuracy: 0.4493 Loss: 5.269056797027588, Accuracy: 0.4493294358253479

Further data cleaning is required and one recommendation is to remove applications that have in-active status.