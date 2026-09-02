# 🎮 Connect Four Move Prediction Using Machine Learning

A machine learning and deep learning project that predicts the optimal next move in a Connect Four game based on the current board state.

The project explores and compares multiple supervised learning models, from traditional machine learning algorithms to neural networks and convolutional neural networks.

## Overview

The goal of this project was to predict the optimal column for the next move in a Connect Four game.

The game board consists of a **6 × 7 grid**, represented by 42 board-position features. The dataset also includes the current player's turn and the optimal move as the target label.

Multiple models and feature engineering techniques were explored to determine which approach achieved the best prediction performance.

## Models Implemented

Eight machine learning and deep learning models were explored:

- Decision Tree
- Logistic Regression
- Random Forest
- Gradient Boosting
- XGBoost
- Neural Network
- LightGBM
- Convolutional Neural Network (CNN)

## Feature Engineering

Several preprocessing and feature engineering approaches were explored.

For the advanced models, the 42 board-position features were multiplied by the player's turn value to represent the board from the perspective of the current player.

For the CNN, the Connect Four board was reshaped into a **6 × 7 grid** and represented using three binary channels:

- Current player's tokens
- Opponent's tokens
- Empty cells

This created a **6 × 7 × 3 tensor**, allowing the CNN to learn spatial patterns from the game board.

## Model Performance

| Model | Validation Accuracy |
|---|---:|
| Decision Tree | 48.50% |
| Logistic Regression | 52.20% |
| Random Forest | 58.90% |
| Neural Network | 59.63% |
| Gradient Boosting | 62.80% |
| LightGBM | 64.09% |
| XGBoost | 64.45% |
| **Convolutional Neural Network** | **68.88%** |

The **CNN achieved the highest validation accuracy of 68.88%**, outperforming the traditional machine learning and other deep learning approaches.

## CNN Architecture

The final CNN architecture includes:

- Four convolutional layers
- Batch normalization
- ReLU activation
- Max pooling
- L2 regularization
- Dense layers
- Dropout
- Softmax output for 7-class classification
- Adam optimizer
- Early stopping
- Learning rate scheduling

L2 regularization was tested using multiple values, with **0.01 achieving the best validation accuracy**.

## Hyperparameter Tuning

Different tuning approaches were used across the models, including:

- Manual hyperparameter experimentation
- Randomized Search for XGBoost
- Regularization
- Early stopping
- Learning-rate adjustment
- Epoch and batch-size experimentation

## Evaluation

Model performance was evaluated using:

- Validation accuracy
- Confusion matrices
- Classification reports

The results were compared to determine how effectively each model predicted the next optimal Connect Four move.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow
- Keras
- XGBoost
- LightGBM
- Matplotlib
- Seaborn

## Key Concepts

- Machine Learning
- Deep Learning
- Multiclass Classification
- Convolutional Neural Networks
- Feature Engineering
- Hyperparameter Tuning
- Regularization
- Ensemble Learning
- Model Evaluation
- Game AI

## Project Purpose

This project was developed to explore how different machine learning and deep learning techniques can be applied to game move prediction.

By comparing traditional classifiers, ensemble methods, neural networks, and CNNs, the project demonstrates how representing the Connect Four board as a spatial grid can improve the model's ability to capture patterns and predict optimal moves.
