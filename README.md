# Neural Network Charity Analysis

## Analysis Overview
The purpose of this project is to use deep-learning neural networks with the TensorFlow platform in Python, to analyze and classify the success of charitable donations.\
We use the following methods for the analysis:
- preprocessing the data for the neural network model,
- compile, train and evaluate the model,
- optimize the model.

## Resources
- Data Source: charity_data.csv
- Software: Python 3.7.7, Anaconda Navigator 1.9.12, Conda 4.8.4, Jupyter Notebook 6.0.3

## Results

### Data Preprocessing
- The columns EIN and NAME are removed as they are considered to be identification information and does not contribute to our model. 
- The column 'IS_SUCCESSFUL' is chosen as our target variable for deep learning as it determine whether or not a charity donation was effective. 
- Other columns such as 'APPLICATION_TYPE, AFFILIATION, STATUS, INCOME' etc. are used as other parameters in our model. 

### Compiling, Training, and Evaluating the Model
- Our deep-learning network model consisted of two hidden layers with 80 and 30 neurons and our input data had more than 40 features and around 27,000 samples. 
- We further used the activation function ReLu for our hidden layers and Sigmoid was used for the output layer. 
- In our compilation, the optimizer is **adam** and the loss function used was **binary_crossentropy**
- Our model accuracy fell below 75% which did not accurately predict the outcome of charity donations. To increase the accuracy of our model, we tried bucketing the feature ASK_AMT and further increased the number neurons in one of the hidden layers. We then applied one more hidden layer to see if our accuracy changed. Unfortunately none of these steps improved the accuracy of our model. 
- 
## Summary
Our deep learning model failed in accuracy as it never broke 75%. One way we could have improved our model was including supervised machine learning models such as Random Forest Classifiers and decision tress to create better outputs. 
