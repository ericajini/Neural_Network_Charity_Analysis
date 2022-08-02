# Neural Network Charity Analysis 

## Overview

The overall goal of this project was to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. The data provided was prepped to be used in the Neural Network by converting to numerical values and scaling the data. The target goal was to achieve 75% accuracy with the model and there were a number of things done in the Optimization phase in attempt to reach the desired succes rate; some of this includes adjusting the values in the input data/ binning, adjusting the neurons and hidden layers, adjusting the epochs, etc. I also set it up to export the models so they could be pulled up in the future/ on other machines if needed. 

## Results

### Data Preprocessing
1. What variable(s) are considered the target(s) for your model? 

The IS_SUCCESSFUL column is considered the target for the model. 

2. What variable(s) are considered to be the features for your model? 

The APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECIAL_CONSIDERATION, and the ASK_AMT columns are considered the features for the model. 

3. What variable(s) are neither targets nor features, and should be removed from the input data? 

The EIN, NAME, and STATUS columns are neither targets nor features and were removed from the input data. 

![Features,Target,Dropped]()

### Compiling, Traning, and Evaluating the Model 
1. How Many neurons, layers, and activation functions did you select for your neural network model, and why? 

In my final attempt, I used 100 neurons in each of the 3 hidden layers in attempt to achieve the desired model performance. During the optimization phase I used 1 hidden layer with 100 neurons and a hidden layer with 50 neurons and increased this as I went along since the max model performance reached was about 73%. 

2. Were you able to achieve the target model performance? 

No, I was not able to achieve the target model performance of 75% accuracy. 

3. What steps did you take to try and increase model performance? 

During the optimization phase, outside of trying to increase the neurons and hidden layers, I also tried using other activation types such as Tanh. I also removed the Status column since this seemed to be providing no value to the model and tried to change around the epochs to increase performance. 

![Final Model]()
![Best Success]()

## Summary 

As mentioned above, I was not able to achieve the desired accuracy of 75 %. I think after going through the process, the next step would be to look back at the input data and determine what I can do so that the model receives the data needed to be more accurate. 