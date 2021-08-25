# Neural_Network_Charity_Analysis

## Overiew

Utilzing Machine Learning and Neural Networks, this project attempts to assist Alphabet Soup Charity Group in developing a model that will be able to predict which applicants should get funding for their projects. For this model, a dataset of 34,000 organizations will be used to train the model to make accurate predictions.

In order to build an accurate model, the data will need to be preprocessed for the neural network model. This will consist of determining the target output for the model (which is a succesfull funding of a project), which variables are considered features, which variables are neither features or targets and should be dropped. The next step would be to compile train and evalute the model. In order to increase accuracy, there will be a testing of different features and varaibles to determine which are best to train the model, attempting to optimize the model using differnt hidden layers, epochs etc. 

### Software Used

Jupyter Notebooks \
Python \
Machine Learning \
Tensorflow \
Keras


## Results

### Preprocessing Data

First step is determining which column is the target. Since this model is intended to help determine the funding of projects, the target would be the "IS_SUCCESSFUL" column.

Next, determine which columns to drop, as they aren't beneficial to model. Having variables that do not add value, can lead to overfitting. Columns "EIN" and "NAME" will be dropped.

![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/droppedColumns.png)

Last step would be to determine which columns are the features then the data will be split into features (X value) and targets (y value) using the "IS_Successful"

![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/features.png)
![image[(https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/successful.png)


### Compiling, Training, and Evaluating the Model

### Optimizing 

During the optimization phase, different models were utilized and evaluated in order to achieve an accuracy rate of 75%. This was done by:
- using varying hidden layers
- using different levels of epochs
- dropping and/or combining different variables to see which have a greater influence on the model

## Summary