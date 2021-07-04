# Neural_Network_Charity_Analysis

## Overview of the Analysis
The purpose of this analysis is to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup by using the provided dataset.

## Results

### Data Preprocessing

#### What variable(s) are considered the target(s) for your model?
The target for my model is the column named "IS_SUCCESSFUL" as shown in the image below.

![Target_Column](https://github.com/WTAN241/Neural_Network_Charity_Analysis/blob/main/Resources/Target_Column.PNG)

#### What variable(s) are considered to be the features for your model?
The features of my model include the following columns:
1. STATUS
2. ASK_AMT
3. IS_SUCCESSFUL
4. APPLICATION_TYPE
5. INCOME_AMT
6. SPECIAL_CONSIDERATIONS

#### What variable(s) are neither targets nor features, and should be removed from the input data?
The variables that are neither targets nor feaures and have been removed from the input data are the columns "EIN" and "NAME"

### Compiling, Training, and Evaluating the Model

#### How many neurons, layers, and activation functions did you select for your neural network model, and why?
For this model, I have selected 3 layers, 80 neurons for the first layer, 30 neurons for the second and 1 neuron for the third layer and the relu and sigmoid activation functions have been used. The reason why this combination of neurons, layers, and activation functions was chosen is because they attained the highest prediction accuracy rate among all the other combinations I have tried.

#### Were you able to achieve the target model performance?
No, I was not able to successfully achieve the target model performance of 75% of accuracy.

![Model_Optimization_Results](https://github.com/WTAN241/Neural_Network_Charity_Analysis/blob/main/Resources/Model_Optimization_Results.PNG)

#### What steps did you take to try and increase model performance?
I have tried the three steps below to increase model performance:
1. I have dropped a few more columns such as "AFFILIATION" and "ORGANIZATION"
2. I have added an additional layer with 30 neurons and using the relu activation function
3. I have increased the number of neurons in the first and second layer to 100 and 50 respectively

## Summary
The overall results of this model shows that it can potentially achieve an accuracy rate of 68.9% and a loss of 69.2%. The reason why the accuracy rate could not achieve the targeted rate of 75% might be an indication that a deep learning model is not the best model for this dataset. A random forest model could be a better predictor for this dataset.