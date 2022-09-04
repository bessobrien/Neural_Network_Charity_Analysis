# Neural_Network_Charity_Analysis

## Overview

The purpose of this project is to create a binary classifier that is capable of predicting whether loan applications will be successful if funded by the organization Alphabet Soup. We preprocessed the data for a neural network model using Pandas, compiled, trained, and evaluated the model. After the initial results, we attempted to optimize the model to obtain a high accuracy score.

## Results

While going through the model, we had to ask ourselves some key questions:

**DATA PREPROCESSING**

1. What variable IS considered the target for our model?
    
    1. IS_SUCCESSFUL

2. What variables are considered to be the features for your model?
    
    1. APPLICATION_TYPE
    2. AFFILIATION
    3. CLASSIFICATION
    4. USE_CASE
    5. ORGANIZATION
    6. STATUS
    7. INCOME_AMT
    8. SPECIAL_CONSIDERATIONS
    9. ASK_AMT

3. What variables are neither targets nor features, and should be removed from the input data?
    
    1. EIN
    2. NAME

**COMPILING, TRAINING, AND EVALUATING THE MODEL**

1. How many neurons, layers, and activation functions did you select for your neural network model, and why?
    
    1. Layers: 2 layers for ease of starting, and simplicity for extensive data.
    
    2. Neurons: 80 and 30 - 80 is approximately twice the input (43), and 30 neurons shortens the calculation time
    
    3. Activation functions: ReLU as it is simple to implmenent and effectitve at overcoming limitations that are present in other activation functions

2. Were you able to achieve the target model performance?
    
    1. No - as seen below, we were not able to acheive 0.75 accuracy.
    
    ![original](https://github.com/bessobrien/Neural_Network_Charity_Analysis/blob/main/Resources/nn_original.png)

3. What steps did you take to try and increase model performance?
    
    1. Increase Bins
    
    ![bins](https://github.com/bessobrien/Neural_Network_Charity_Analysis/blob/main/Resources/increase_bin.png)

    2. Decrease Epochs
    
    ![epochs](https://github.com/bessobrien/Neural_Network_Charity_Analysis/blob/main/Resources/decrease_epoch.png)

    3. Increase Neurons
    
    ![neurons](https://github.com/bessobrien/Neural_Network_Charity_Analysis/blob/main/Resources/increase_neurons.png)

## Summary

Overall, even after optimization attempts, we were unable to improve the effectiveness of the model and bring accuracy up to 0.75 or greater. Finally, I would recommend combining optimization attempts - increase amount in bins, increase neurons, to see if that would further optimize the model.

Another approach to take is the Random Forest Classification model - this model excels at classification and is effective. The Random Forest Classifier is a little easier to use and less prone to overfitting than neural networks. 

