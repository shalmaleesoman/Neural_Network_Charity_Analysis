# Neural_Network_Charity_Analysis

## Overview Of Analysis

The purpose of this project was to use neaural networks with the Tensorflow platform in the MLNEV environment of Python to analyze whether applicants will be successful if funded by Alphabet Soup.

#### Methods:
* Preprocessing the data for teh neural network model.
* compile, train and evaluate the model
* optimize the model.

## Resources Used

* charity_data.csv
* Python, Anaconda Navigator, Conda, Jupyter Notebook 

## Results

### Data Processing:

* the target variable for this model was the "IS_SUCCESSFUL" data, because it contained binary data referring to whether the charity donation was used successfully or not
* "APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_ATM, SPECIAL_CONSIDERATIONS, ASK_AMT" are the features for the model
* "EIN' and "NAME" columns were dropped from the input data

### Compiling, Training, and Evaluating the Model

The neural network model is made of two hidden layers with 80 & 30 neurons respectively. Input data has 43 features and 25,723 samples.

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

## Summary

This deep learning neural netowrk did not reach the target of 75% accuracy, leading us to conclude that this model is not outperforming. Although we tried adding layers, applyding different features and using different activation functions, the model is still not good enough. Factors that would help this model be more precise would be more data to analyze, or a supervised machine learning model such as the Random Forest Classifier to combine a large quantities of decision tree to generate and evaluate against the deep learning model 

