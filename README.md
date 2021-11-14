# Neural_Network_Charity_Analysis

## Overview Of Analysis

The purpose of this project was to use neaural networks with the Tensorflow platform in the MLNEV environment of Python to analyze whether applicants will be successful if funded by Alphabet Soup.

## Resources Used

* charity_data.csv
* Python, Anaconda Navigator, Conda, Jupyter Notebook 

## Results

### Data Processing:

* the target variable for this model was the "IS_SUCCESSFUL" data, because it contained binary data referring to whether the charity donation was used successfully or not
* "APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_ATM, SPECIAL_CONSIDERATIONS, ASK_AMT" are the features for the model
* "EIN' and "NAME" columns were dropped from the input data

### Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?

![1](https://user-images.githubusercontent.com/86750935/141701813-7768c4a6-eebd-4b4a-8f0c-039ff060e5b8.PNG)

The neural network model is made of two hidden layers, with 80 and 30 neurons. Each layer has an activation function. The first and second hidden layers have an activation function "relu" & the output layer is "sigmoid".

* Were you able to achieve the target model performance?

No, the model is under 75%, hence it is not a satisfying performance to help predict the outcome of Charity donations by Alphabet Soup.

* What steps did you take to try and increase model performance?

![2](https://user-images.githubusercontent.com/86750935/141702059-b3f3fb60-f235-49af-ae20-b5506d7ebc37.PNG)

* applied the bucketing to the feature ASK_AMT, and organized the different values by intervals to increase the performance of the model
* added hidden layers to increase the number of neurons, using an optimized model with three hidden layers.
* tried a different activation function (tanh), however, none of these helped.



