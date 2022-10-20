# Neural_Network_Charity_Analysis
## Overview

### Goal

Use machine learning and neural networks on the dataset to create a binary classifier capable of predicting if applications will be successful post funding.

Project Deliverables

1.	 Preprocessing Data for a Neural Network Model
2.	 Compile, Train, and Evaluate the Model
3.	 Optimize the Model
4.	 A Written Report on the Neural Network Model 

## Results

### Data Preprocessing

- **What variable(s) are considered the target(s) for your model?**

    The target is the binary feature “IS_SUCCESSFUL”, which indicates whether the money was used effectively. 

- **What variable(s) are considered to be the features for your model?**

    "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", "ASK_AMT", "STATUS", these columns are features for the model.

- **What variable(s) are neither targets nor features, and should be removed from the input data?**

    “EIN” and “NAME” are identification columns, have been removed from the input data.

### Compiling, Training, and Evaluating the Model

- **How many neurons, layers, and activation functions did you select for your neural network model, and why?**

     The neural network model has 2 hidden layers with 80 and 30 neurons for each layer. Generally, it is common to choose 2 layers, 80 is close to twice of input features (43) and 30 is close to 2/3 of the input features. The ```ReLU``` activation function was used for hidden layers to speed up the training process and ```Sigmoid``` was used for the binary output layer.


- **Were you able to achieve the target model performance?**

     The performance is around 73%, which is below target model performance of 75%.

- **What steps did you take to try and increase model performance?**
    1.	Applied bucketing to ASK_AMT feature.
    2.	Added additional neurons on hidden layers.
    3.	Added additional hidden layers.
    4.	Used different activation function, tanh.

## Summary

Overall, the  results of the deep learning model are near 73%. Even though several methods were attempted to optimize the performance, the result is still under 75%. As recommendation, try Random Forest Classifier, which is a classification algorithm consisting of many decisions to further evaluate the performance.
