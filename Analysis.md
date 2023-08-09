# Overview

In this analysis we have developed several different methodologies of model training for classification. The goal is to showcase the effectiveness of various techniques in improving model performance. The intent is to use this model to inform selection decisions for applicants for the organization Alphabet Soup.

# Example of a model trained using Batch Normalization

Below shows python code for an example of a model using batch normalization and the results below. The accuracy is high overall but did not achieve as high of an accuracy as the original model.

![Fig2_Batch_Analysis](https://github.com/eacromwell/deep-learning-challenge/assets/123791177/d848f623-bd30-4d08-bf6a-7240279422ee)

# Results

## Data Preprocessing
- Target Variable(s):

The target variable for our model is a binary classification label indicating the presence or absence of a specific outcome.

- Feature Variable(s):

The feature variables are the attributes or characteristics that we use as inputs to the model for making predictions. These features contribute to the model's decision-making process.

- Variables to Remove:
  
Any variables that are not directly related to the target variable or do not provide meaningful information for the classification task should be removed. Irrelevant or redundant features can negatively impact the model's performance and increase its complexity.

## Compiling, Training and Evaluating the Model

- Neurons, Layers, and Activation Functions:
In our neural network model, we selected the following configuration:

Input Layer: 38 units (corresponding to the number of features), no activation function specified.
Hidden Layer 1: 10 units with the tanh activation function. Tanh provides a good balance between linearity and non-linearity, which is beneficial for capturing complex relationships in the data.
Hidden Layer 2: 8 units with the tanh activation function. Adding a second hidden layer allows the model to learn more intricate features from the data.
Output Layer: 1 unit with the sigmoid activation function. Sigmoid is suitable for binary classification as it maps the output to a probability between 0 and 1.

- Target Model Performance:

The target model performance is typically determined based on the problem's context and requirements. It could be a specific accuracy threshold, precision, recall, or other relevant metrics. Achieving the target performance indicates that the model is effectively capturing patterns and making accurate predictions.

- Steps Taken to Increase Model Performance:
  
To enhance model performance, we undertook several optimization methods:

Learning Rate Scheduling: Adjusting the learning rate during training can aid convergence and improve the model's ability to find optimal solutions.
Batch Normalization: Normalizing activations between layers helps stabilize training and accelerate convergence.
L2 Regularization: Adding L2 regularization reduces overfitting by penalizing large weights, promoting simpler and more generalizable representations.

## Summary

In conclusion, the chosen neural network model architecture and optimization techniques were designed to achieve better training convergence and improved generalization. The model's performance was evaluated based on accuracy and loss metrics, and optimization techniques were applied to enhance its effectiveness. The target model performance was achieved, suggesting that the selected techniques successfully contributed to better classification outcomes.
