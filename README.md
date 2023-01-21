# Neural Network Charity Analysis

## Purpose

The purpose of this analysis was to use a deep-learning model to analyze and then classify charitable donations. 

In this analysis I used:
* Data preprocessing
* Compiling, training, and evaluation of the model
* Different methods of optimization for the model

## Results
### Data Preprocessing:
* The column present in the data, ```IS_SUCCESSFUL```, contains binary data. As such, it was used as our target in the model. 
* Columns ```APPLICATION_TYPE, AFFILIATION	CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT``` were considered features of our data and were used in training and testing data. 
* Both the ```NAME``` and ```EIN``` columns were removed from input data.

### Compiling, Training, and Evaluating the Model:
* For the initial modeling I used 8 neurons and 5 neurons for both the first and second hidden layers. I settled on 8 neurons and 5 neurons for my two hidden layers because they gave me best performance with the initial model while remaining lightweight enough to stay away from over training the data. Activation functions for the hidden layers were set to ReLU and my output layer used Sigmoid.
* Unfortunately, I was not able to reach the target model performance of 75% using the initial model.
* To try and increase the performance of my initial model, I tried increasing the number of neurons, the number of hidden layers, the number of epochs, and changing both activation and output functions.

## Summary

Though many optimizations were researched and used the model was not able to perform at the 75% or better level. Tne initial model saw only 72.3% efficiency while our optimized model saw only ~72% in three separate tries. Perhaps the issue with the performance level is the method used and instead using something like a Supervised Learning algorithm such as RandomForestClassifier would result in better performance levels.
