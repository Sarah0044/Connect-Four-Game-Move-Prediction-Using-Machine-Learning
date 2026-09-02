# 🎮 Connect Four Move Prediction Using Machine Learning

🏆 **3rd Place – King Saud University Machine Learning Course Competition**

A machine learning and deep learning project that predicts the optimal next move in a Connect Four game based on the current board state.

The project explores and compares multiple supervised learning models, from traditional machine learning algorithms to neural networks and convolutional neural networks.

## 🏆 Achievement

This project achieved **3rd place** in the Machine Learning course competition at **King Saud University**.

The final Convolutional Neural Network (CNN) achieved the best performance among the models developed in the project, reaching **68.88% validation accuracy**.

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

For the advanced models, the 42 board-position features were transformed based on the player's turn to represent the board from the perspective of the current player.

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

The **CNN achieved the highest validation accuracy of 68.88%**.

## CNN Architecture

The final CNN architecture includes:

- Four convolutional layers
- Batch normalization
- ReLU activation
- Max pooling
- L2 regularization
- Dense layers
- Dropout
- Softmax output
- Adam optimizer
- Early stopping
- Learning rate scheduling

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

This project was developed as part of the **Machine Learning course at King Saud University** to explore how different machine learning and deep learning techniques can be applied to game move prediction.

The project ultimately achieved **3rd place in the course competition**.
