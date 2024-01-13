# Alphabet Soup Charity Funding Predictor

## Overview of the Analysis

The purpose of this analysis is to create a deep learning model that can predict whether applicants for funding from Alphabet Soup will be successful. Alphabet Soup, a philanthropic foundation, requires a tool to help them discern which organizations are likely to use the funding effectively. The model is built using a dataset of over 34,000 past applications with various metrics about each organization.

## Results

Data Preprocessing
Target Variable(s):
The target for the model is the IS_SUCCESSFUL column, which indicates whether the money was used effectively.
Feature Variable(s):
The features for the model include:
APPLICATION_TYPE: Type of application.
AFFILIATION: Affiliated sector of industry.
CLASSIFICATION: Government organization classification.
USE_CASE: Use case for funding.
ORGANIZATION: Organization type.
STATUS: Active status.
INCOME_AMT: Income classification.
SPECIAL_CONSIDERATIONS: Special considerations for application.
ASK_AMT: Funding amount requested.
Non-Feature/Target Variables:
Variables that were removed from the input data include:
EIN and NAME: These are identification columns and not predictive of the outcome.
Compiling, Training, and Evaluating the Model
Model Architecture:
The final model consists of:
First Hidden Layer: 80 neurons, ReLU activation function.
Second Hidden Layer: 30 neurons, ReLU activation function.
Output Layer: 1 neuron, Sigmoid activation function.
This architecture was chosen to provide enough complexity to learn from the dataset while avoiding overfitting.
Model Performance:
The target model performance was not fully achieved. The final model had an accuracy of approximately 72.68%, slightly below the target of 75%.
Optimization Attempts:
To improve model performance, the following steps were taken:
Increasing the number of neurons in the hidden layers.
Adding additional hidden layers.
Experimenting with different activation functions.
Adjusting the number of epochs and batch sizes during training.
## Summary

The deep learning model developed for Alphabet Soup's funding application evaluation performed moderately well, with an accuracy of about 72.68% after 4 attempts. While it provides a good starting point, there is room for improvement to reach the desired accuracy threshold.

### Recommendation for a Different Model
Alternative Approach:
A Random Forest Classifier could be considered as an alternative to the neural network model. Random Forests are effective for classification problems and can handle a mix of numerical and categorical data well. They also provide good performance with less need for tuning compared to deep learning models.
