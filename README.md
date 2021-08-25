# Neural_Network_Charity_Analysis

## Overview

Utilizing Machine Learning and Neural Networks, this project attempts to assist Alphabet Soup Charity Group in developing a model that will be able to predict which applicants should get funding for their projects. For this model, a dataset of 34,000 organizations will be used to train the model to make accurate predictions.

In order to build an accurate model, the data will need to be preprocessed for the neural network model. This will consist of determining the target output for the model (which is a successful funding of a project), which variables are considered features, which variables are neither features or targets and should be dropped. The next step would be to compile train and evaluate the model. In order to increase accuracy, there will be a testing of different features and variables to determine which are best to train the model, attempting to optimize the model using different hidden layers, epochs etc. 

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
![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/successful.png)


### Compiling, Training, and Evaluating the Model
This phase consisted of customizing the neural network to calculate data inputs and extract and output. The model was defined with 2 hidden layers utilizing the Rectified Linear Unit (ReLU) function, with 80 and 30 neurons respectively and the output layer utilized the Sigmoid function. This lead to an accuracy rate of 72%.

- Defined Model

![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/DefineModel.png)

- Compiled, Trained and Evaluated Model

![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/compileTrainEvaluate.png)

- Model Accuracy

![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/InitialAccuracy.png)

### Optimizing 

During the optimization phase, different models were utilized and evaluated in order to achieve an accuracy rate of 75%. This was done by:
- using varying hidden layers
- varying numbers of neurons on the hidden layers
- using different levels of epochs
- dropping and/or combining different variables to see which have a greater influence on the model

#### First Attempt at Optimization

![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/Optimization1.png)
![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/OptimizationModel1.png)
![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/OptimizationAccuracy1.png)

#### Second Attempt at Optimization

![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/Optimization2.png)
![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/OptimizationModel2.png)
![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/OptimizationAccuracy2.png)

#### Third Attempt at Optimization

![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/Optimization3.png)
![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/OptimizationModel3.png)
![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/OptimizationAccuracy3.png)

#### Fourth Attempt at Optimization

![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/Optimization4.png)
![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/OptimizationModel4.png)
![image](https://github.com/roderickspells/Neural_Network_Charity_Analysis/blob/main/Challenge/Images/OptimizationAccuracy4.png)

## Summary

The initial model was able to predict successful funding at 72% accuracy. After optimizing the model different ways, the optimal accuracy rate achieved was 73%. Although desired 75% accuracy rate was not achieved, the methodology used here - testing and improving - different modeling techniques can help build a stronger neural network through trial and error. Although there is a substantial amount of data in this dataset, other types of data might be useful in the training of the model. Since the model is taking into consideration metadata such as income classification, funding amount requested and the effective use of the funding, data point such as past loan behavior (default rate, timely payments etc.) could also be used to improve prediction rates of the model.

Different models utilizing activation functions such as the Leaky ReLU function or tanh function could give different and more accurate results. The Random Forest model could also be an alternative to as it tends to hand classification issues easier because it can interpret and handle outliers better. Another reason Random Forest might be a better model is due to the fact that the data used here is tabular.
