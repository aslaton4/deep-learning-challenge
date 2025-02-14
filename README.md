# Alphabet Soup Neural Network Model Report

## Overview
### The goal of this analysis is to build a deep learning model that will predict whether an Alphabet Soup funding applicant will be successful. Using historical funding data, a binary classification model to improve decision-making was created. 

## Results
### Data Preprocessing
- Target Variable (y): IS_SUCCESSFUL (1 = successful, 0 = unsuccessful).
- Feature Variables (X): Categorical and numerical features, including APPLICATION_TYPE, CLASSIFICATION, ASK_AMT, etc.
- Removed Columns: EIN and NAME (irrelevant identifiers).

## Model Summary
### Architecture
- Input Layer: Based on the number of features.
- Hidden Layers:
    - Layer 1: 64 neurons, ReLU
    - Layer 2: 32 neurons, ReLU
- Output Layer: 1 neuron, Sigmoid activation

### Compilation
- Optimizer: Adam
- Loss Function: Binary Crossentropy
- Epochs: 50, Batch Size: 32

### Performance
- Test Accuracy: 72.52% (Goal: 75%)
- Loss: 0.5583

## Optimization Attempts
- Increased neurons and layers → No significant improvement.
- Adjusted activation functions and learning rate → Overfitting issues.
- Trained for more epochs → No major accuracy gain.

## Conclusion and Recommendations
- Deep learning did not achieve 75% accuracy.
- Alternative models like Random Forest or XGBoost could perform better on this structured data.
- Further feature selection and tuning might improve results.

## Resources
- Class/rewatch
- google colab resources
- TensorFlow Playground
- Youtube
- Chatgpt