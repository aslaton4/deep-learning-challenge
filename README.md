# Alphabet Soup Neural Network Model Report

## Overview
### The goal of this analysis is to build a deep learning model that will predict whether an Alphabet Soup funding applicant will be successful. Using historical funding data, a binary classification model to improve decision-making was created. By preprocessing the dataset, optimizing the neural network and then evaluating the performance, we should be able to determine if deep learning is an effective approach for this model. 

## Results
### Data Preprocessing
- Target Variable (y): IS_SUCCESSFUL (1 = successful, 0 = unsuccessful).
- Feature Variables (X): Categorical and numerical features, including APPLICATION_TYPE, CLASSIFICATION, ASK_AMT, etc.
- Removed Columns: EIN and NAME (irrelevant identifiers).

## Compiling, Training, Evaluating Model
- Input Layer: Matches number or preprocessed features
- Hidden Layers:
    - Layer 1: 128 neurons, ReLU activation
    - Layer 2: 64 neurons, ReLU activation
    - Layer 3: 32 neurons, ReLU activation
- Output Layer: 1 neuron, Sigmoid activation

### Performance
- Test Accuracy: 72.52% (Goal: 75%)

## Optimization Attempts
- Increased neurons and added third hidden layer
- Tried ReLu and LeakyReLU
- Adjusted hyperparameters: batch size = 32 and epochs = 100
- Adjusted learning rate Adam optimizer with 0.001
- Used dropout layers not included in final 

## Conclusion and Recommendations
- Deep learning did not achieve 75% accuracy.
- Increasing complexity didn't show significant improvement in results.
- Alternative models like Random Forest or XGBoost could perform better on this structured data.

## Resources
- Class/rewatch
- TA assistance
- google colab resources
- TensorFlow Playground
- Youtube
- Chatgpt