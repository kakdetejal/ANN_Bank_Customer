## Bank Customer Churn Prediction (ANN)

This project predicts whether a bank customer is likely to churn using an Artificial Neural Network (ANN).

# Overview
Dataset: Bank customer data (10,000 records)
Goal: Predict customer churn (Exited)
Type: Binary Classification

# Workflow
Data preprocessing:
Dropped irrelevant columns
Encoded Gender (Label Encoding)
One-Hot Encoded Geography
Feature scaling using StandardScaler
Train-test split (80-20)

# Model
ANN built using TensorFlow/Keras
Architecture:
Input layer
Hidden layers (ReLU)
Output layer (Sigmoid)
Early stopping used to prevent overfitting

# Hyperparameter Tuning
Used GridSearchCV with KerasClassifier
Tuned:
- Neurons
- Layers
- Epochs
Best model selected based on cross-validation score

# Model Saving
Saved:
Trained model (.h5)
Scaler (scaler.pkl)
Encoders (geo_encoded.pkl, gender_encoded.pkl)

# Prediction Pipeline
Load saved encoders & scaler
Transform new input data
Predict churn using trained ANN

# Output:
Class (0/1)
Probability of churn

# Result
Achieved ~85% accuracy after tuning



Layers
Epochs
Best model selected based on cross-validation score
