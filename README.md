# README – Part 1: Neural Network Fundamentals and Training Behavior Analysis

## Project Title

Customer Churn Prediction using Neural Networks

---

# Project Overview

This project demonstrates the implementation and analysis of a Feed-Forward Neural Network for a supervised learning problem using a structured dataset.

The objective of this assignment is not only to build a predictive model but also to understand how neural networks learn through:

* Forward propagation
* Loss calculation
* Backpropagation
* Weight and bias updates
* Hyperparameter tuning

The project uses customer churn data to predict whether a customer is likely to leave the service.

---

# Dataset Information

Dataset File:

`customer_churn_nn.csv`

Target Variable:

`churn`

* 0 → Customer did not churn
* 1 → Customer churned

Dataset Characteristics:

* Structured tabular dataset
* Contains numerical and categorical features
* Binary classification problem

---

# Tasks Covered

## Task 1 – Dataset Understanding

Performed:

* Dataset loading
* Shape analysis
* Feature identification
* Missing value checking
* Statistical summary
* Target variable distribution analysis

---

## Task 2 – Data Preprocessing

Performed:

* Missing value handling
* Categorical encoding using OneHotEncoder
* Feature scaling using StandardScaler
* Train-test splitting

---

## Task 3 – Neural Network Model Building

Implemented:

* Feed-forward neural network
* Hidden layers with ReLU activation
* Adam optimizer
* Binary classification output layer

Libraries Used:

* Scikit-learn
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

## Task 4 – Training and Evaluation

Evaluated using:

* Training accuracy
* Testing accuracy
* Confusion matrix
* Classification report

---

## Task 5 – Hyperparameter Experimentation

Experiments were conducted by changing:

* Hidden layers
* Number of neurons
* Activation functions
* Learning rate
* Batch size
* Number of epochs

A comparison table was created to analyze performance differences.

---

## Task 6 – Final Reflection

Included explanations about:

* Role of weights and biases
* Importance of activation functions
* Effect of learning rate
* Underfitting and overfitting

---

# Neural Network Learning Process

The report also explains:

1. Forward Pass
2. Loss Function
3. Backpropagation
4. Gradient Descent Parameter Updates

This helps understand how neural networks optimize themselves during training.

---

# Model Performance Summary

| Metric            | Value  |
| ----------------- | ------ |
| Training Accuracy | 100%   |
| Testing Accuracy  | 98.25% |

Observation:

* The model achieved high accuracy.
* Dataset imbalance affected prediction of minority class.
* Mild overfitting was observed.

---

# How to Run the Project

## Step 1: Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## Step 2: Place Dataset File

Keep the dataset file in the same folder as the Python notebook/script.

Example:

```text
project_folder/
│
├── customer_churn_nn.csv
├── part1_solution.ipynb
└── README.md
```

---

## Step 3: Run the Notebook or Python Script

Execute all cells sequentially.

---

# Folder Structure

```text
Part1_Project/
│
├── customer_churn_nn.csv
├── README.md
├── neural_network_solution.ipynb
└── report.pdf
```

---

# Conclusion

This project successfully demonstrates:

* Neural network implementation
* Data preprocessing
* Model training and evaluation
* Hyperparameter tuning
* Understanding of neural network learning behavior

The assignment provides both practical implementation and theoretical understanding of neural network fundamentals.
