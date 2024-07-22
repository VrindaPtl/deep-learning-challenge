# deep-learning-challenge
# Purpose:
In this project, we will employ a deep learning approach to develop a binary classification model. This model aims to predict the success of organizations funded by Alphabet Soup using features from a dataset. I will utilize machine learning techniques and neural networks to analyze a CSV file comprising metadata from over 34,000 funded organizations. The goal is to predict the likelihood of success for future applicants based on this historical data.

# Analysis:
After testing four models, the origional model, which employed auto-optimization, achieved the highest accuracy on the test data at 72.65%, not surpassing the 75% accuracy goal. It also exhibited a relatively high loss percentage of 0.55.

The Optimisation models achieved an accuracy of 72.48%, 53.24% and 72.50% respectively, with a higher loss percentage of 0.56, 0.69 and 0.55 respectively. 

In conclusion, the Origional emerged as the best performer despite its relatively high loss percentage.

# Data Processing:

## Which variable(s) are the target(s) for your model? 
The target variable for each model was the IS_SUCCESSFUL column. Our objective is to predict the success of applicants, utilizing all other features to make predictions.

## Which variable(s) are the features for your model? 
The features available for my model include: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.

## Which variable(s) should be removed from the input data because they are neither targets nor features? 
Initially, I excluded the EIN and NAME columns as instructed. However, during the first optimization attempt, I reintroduced the NAME column to account for potential biases towards specific organizations, given that many were listed multiple times.

# Compiling, Training, and Evaluating the Model

## How many neurons, layers, and activation functions did you select for your neural network model, and why?
In the initial model, I opted for 2 hidden layers, each consisting of 100 neurons using ReLU activation. The output layer was configured with Sigmoid activation. I selected ReLU because upon examining the data, I recognized its non-linear characteristics, making ReLU the suitable starting point for activation functions.

Training Steps:
268/268: This indicates that the model was trained over 268 batches of data.

Time per Step:
0s - 1ms/step: Each training step took approximately 1 millisecond, which is quite fast.

Accuracy:
0.7268: This means the model’s accuracy on the training data is about 72.68%.

Loss:
0.5527: The loss value indicates how well the model is performing. A lower loss generally means a better model. In this case, the loss is 0.5527.

Final Metrics:
Loss: 0.5527326464653015: This is the final loss value after training.
Accuracy: 0.7267638444900513: This is the final accuracy value after training.

In summary, The model has a training accuracy of approximately 72.68% and a loss of 0.5527. These metrics suggest that the model is performing reasonably well, but there might still be room for improvement depending on your specific goals and the complexity of the task.


## Were you able to achieve the target model performance?
I unsuccessfully achieved a target model performance of 75% or higher in all attempts, including my initial model and three different optimizations, during my third optimization.

## What steps did you take in your attempts to increase model performance?
In my all 3 optimization, I added a third hidden layer using the ReLU algorithm.

# Summary:
I think a random forest could be an effective solution for this problem. This machine learning technique excels at classification tasks and could be useful in predicting funding for organizations. Additionally, random forests combine multiple decision trees, which helps to prevent overfitting—a challenge I previously faced.
