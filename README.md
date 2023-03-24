# Neural_Network_Charity_Analysis

## Overview of the loan prediction risk analysis:

### The purpose of this project is the use the features in the AlphbetSoupCharity dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.  This data set contains 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

#### A. Identification columns

#### B. Alphabet Soup application type

#### C. Affiliated sector of industry

#### D. Government organization classification

#### E. Use case for funding

#### F. Organization type

#### G. Active status

#### H. Income classification

#### I. Special consideration for application

#### J. Funding amount requested

#### K. Was the money used effectively

## Results:

### Data Preprocessing

#### 1. The variable that was considered the target was whether the money was used effectively and the organization was successful.

#### 2. All other variables were considered features except the application name and EIN number.

#### 3. The two variables that were removed were the EIN and Name of the organization.

### Compiling, Training, and Evaluating the Model

#### 1. The number of neurons in the first and second layers were 80 and 30 respectively.  The number of input dimensions was the length of the features in the table.  As relu is less prone to vanishing gradient problems it was chosen.  

#### 2. The target performance of 75% was not achieved.

#### 3.  The optimization was done through the Keras_tuner library which allowed for the model to determine the number of neurons (1-30) and option of activation function (relu, tanh, and sigmoid) in the first and hidden layers.  The output layer's activation function was sigmoid, as that is the standard choice.  The Keras_tuner was unable to find a model that did better than 75%
![Top_3_hyperparameters](https://user-images.githubusercontent.com/115171651/227627884-7cba5f0c-f0cf-444c-816f-dcb6a7bf6e31.png)
![Top_model_dataset](https://user-images.githubusercontent.com/115171651/227627897-a36bc144-dd4c-4895-b372-91304e83927c.png)


## Summary:

There is a summary of the results (2 pt)
There is a recommendation on using a different model to solve the classification problem, and justification (3 pt)
