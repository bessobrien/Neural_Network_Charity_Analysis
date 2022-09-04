# Neural_Network_Charity_Analysis

## Overview

The purpose of this project is to create a binary classifier that is capable of predicting whether loan applications will be successful if funded by the organization Alphabet Soup. We preprocessed the data for a neural network model using Pandas, compiled, trained, and evaluated the model. After the initial results, we attempted to optimize the model to obtain a high accuracy score.

## Results

While going through the model, we had to ask ourselves some key questions:

**DATA PREPROCESSING**

*What variable IS considered the target for our model?
    *IS_SUCCESSFUL

*What variables are considered to be the features for your model?
    *APPLICATION_TYPE
    *AFFILIATION
    *CLASSIFICATION
    *USE_CASE
    *ORGANIZATION
    *STATUS
    *INCOME_AMT
    *SPECIAL_CONSIDERATIONS
    *ASK_AMT

*What variables are neither targets nor features, and should be removed from the input data?
    *EIN
    *NAME

**COMPILING, TRAINING, AND EVALUATING THE MODEL**

*How many neurons, layers, and activation functions did you select for your neural network model, and why?
    *Layers: 2 layers for ease of starting, and simplicity for extensive data.
    *Neurons: 80 and 30 - 80 is approximately twice the input (43), and 30 neurons shortens the calculation time
    *Activation functions: ReLU as it is simple to implmenent and effectitve at overcoming limitations that are present in other activation functions

*Were you able to achieve the target model performance?
    *No - as seen below, we were not able to acheive 0.75 accuracy.
    !LINK[]()

*What steps did you take to try and increase model performance?
    *Increase Bins
    !LINK

    *Decrease Epochs
    !LINK

    *Increase Neurons
    !LINK

## Summary

Overall, even after optimization attempts, we were unable to improve the effectiveness of the model and bring accuracy up to 0.75 or greater. Finally, I would recommend combining optimization attempts - increase amount in bins, increase neurons, to see if that would further optimize the model.

Another approach to take is the Random Forest Classification model - this model excels at classification and is effective. The Random Forest Classifier is a little easier to use and less prone to overfitting than neural networks. 

