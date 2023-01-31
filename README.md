# Neural_Network_Charity_Analysis

## Overview of the analysis: 

Based on our knowledge of machine learning and neural networks, in this project we were tasked with predicting whether charity applicants will be successful if funded by Alphabet Soup. Neural networks are a set of algorithms that are modeled to reflect how the human brain works. Currently, neural networks are a form of machine learning designed to recognize patterns and features from input data to provide clear quantitative outputs. This is achieved by creating layers of neurons, which perform individual computations based on the amount of neurons per player and their activation functions. Finally, after the computations are weighed against each other, the final layer will return a categorical result. To test our knowledge of this type of modeling, Alphabet Soup’s business team sent data containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. This project is made up of the deliverables that are listed below:

- Deliverable 1: Preprocessing Data for a Neural Network Model
- Deliverable 2: Compile, Train, and Evaluate the Model
- Deliverable 3: Optimize the Model

## Results:

### Data Preprocessing

- In the preprocessing deliverable the “name” and “ein” columns were removed because they were deemed as non-beneficial for the model. It was also discovered that ask amount, classification, and application type had enough unique variables to be catergorized and binned. 

-When shooting to optimize the data, the status column was sorted and filtered by active, and then removed. This was done so the model was only taking into account active charities. 

### What variable(s) are considered the target(s) for your model?

- The target for this model was to accurately predict if a charity would be successful if it was funded by Alphabet Soup.

### What variable(s) are considered to be the features for your model?

- The column “is_successful” was the primary feature for this model.

### What variable(s) are neither targets nor features, and should be removed from the input data?

-The “ein” number and the “name” of the charity were removed from the input data because they are features that would not increase the accuracy of the model. 

### After Compiling, Training, and Evaluating the Model, how many neurons, layers, and activation functions did you select for your neural network model, and why?

- Without optimizing the model, the model had 100 neurons in the first hidden layer and 50 neurons in the second. The activation functions that were selected were relu for the hidden layers and sigmoid for the outer layer. Relu was chosen initially in the hidden layers because it is simpler computationally; whereas, sigmoid requires an exponent therefore it is computationally more demanding.

### Were you able to achieve the target model performance?

- Even after trying to optimize the model, we were not able to achieve an accuracy score greater than 75%.

### What steps did you take to try and increase model performance?

The steps that were taken in order to optimize the model include the following:

- Dropping more columns.

- Creating more bins for rare occurrences in columns.

- Increasing the number of values for each bin.

- Adding more neurons to each hidden layer.

- Adding more hidden layers.

- Using different activation functions for both the hidden and output layers.

- Adding the number of epochs to the training regimen.

## Summary:

The original model without any optimizations that utilized the relu activation functions in the hidden layers and sigmoid function in the outer layer yielded the highest result at about 73% accuracy. After optimizing the model it failed to achieve an accuracy score greater than 75% it is recommended that a Random Forest Model could solve the classification problems by randomly sampling the preprocessed data and developing easier to execute decision trees. 
