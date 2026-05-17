# Part 1 — Neural Network Fundamentals and Training Behaviour Analysis

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)
![Task](https://img.shields.io/badge/Task-Customer%20Churn%20Prediction-purple)
![License](https://img.shields.io/badge/License-MIT-brightgreen)

---

# 📌 Project Overview

This project focuses on understanding how neural networks work by building a customer churn prediction system using a Feed-Forward Neural Network.

The main objective was not just to train a model, but also to study the complete learning process of neural networks, including:
- Forward propagation
- Loss calculation
- Backpropagation
- Weight updates
- Hyperparameter tuning

The model predicts whether a customer is likely to leave a service based on customer-related features from a structured dataset.

---

# 📂 Project Structure

```text
part-1-neural-network-fundamentals/
│
├── README.md
├── notebook.ipynb
├── requirements.txt
├── customer_churn_nn.csv
│
└── results/
    ├── dataset_analysis.png
    ├── preprocessing_pipeline.png
    ├── training_curves.png
    ├── confusion_matrix.png
    ├── hyperparameter_comparison.png
    └── final_predictions.png
```

---

# 📊 Dataset Information

### Dataset File
`customer_churn_nn.csv`

### Prediction Target

| Value | Meaning |
|---|---|
| 0 | Customer stayed |
| 1 | Customer churned |

### Dataset Characteristics
- Structured tabular dataset
- Contains both numerical and categorical features
- Binary classification problem

The dataset represents customer information that can help predict whether a user may discontinue the service.

---

# 🔍 Task 1 — Dataset Understanding

The first step involved exploring and understanding the dataset.

### Analysis Performed
- Dataset loading
- Shape and feature inspection
- Missing value checking
- Statistical summary generation
- Target distribution analysis

This helped identify potential preprocessing requirements before training the neural network.

---

# 🧹 Task 2 — Data Preprocessing

Data preprocessing was an important step because neural networks perform best when the input data is clean and properly formatted.

### Preprocessing Steps
- Handling missing values
- Encoding categorical variables using `OneHotEncoder`
- Feature scaling using `StandardScaler`
- Splitting the dataset into training and testing sets

### Why Scaling Matters
Neural networks are sensitive to feature magnitude. Standardization ensures that all features contribute more evenly during training.

---

# 🧠 Task 3 — Neural Network Model

A Feed-Forward Neural Network was implemented for customer churn prediction.

## Model Components
- Input layer
- Hidden layers with ReLU activation
- Output layer with sigmoid activation
- Adam optimizer

---

## Libraries Used

| Library | Purpose |
|---|---|
| Pandas | Data handling |
| NumPy | Numerical operations |
| Scikit-learn | Preprocessing and evaluation |
| TensorFlow / Keras | Neural network implementation |
| Matplotlib & Seaborn | Visualization |

---

# ⚙️ Task 4 — Model Training and Evaluation

The neural network was trained using the processed dataset and evaluated on unseen test data.

## Evaluation Metrics

| Metric | Value |
|---|---|
| Training Accuracy | 100% |
| Testing Accuracy | 98.25% |

### Additional Evaluation Methods
- Confusion Matrix
- Classification Report
- Accuracy Curves

---

## Observations
- The model achieved very high prediction accuracy.
- Some imbalance in the dataset affected minority-class predictions.
- Slight overfitting was observed because training accuracy was higher than testing accuracy.

---

# 🔬 Task 5 — Hyperparameter Experimentation

Several experiments were performed to understand how different hyperparameters affect model performance.

## Parameters Tested
- Number of hidden layers
- Number of neurons
- Activation functions
- Learning rate
- Batch size
- Epoch count

A comparison table was created to analyze how each configuration influenced accuracy and training stability.

---

# 📘 Task 6 — Understanding Neural Network Learning

This section focused on the theoretical understanding of how neural networks learn from data.

---

## Forward Propagation
During the forward pass, input features move through the network layer by layer until the final prediction is generated.

---

## Loss Function
The loss function measures how far the predicted output is from the actual target value.

The optimizer tries to minimize this loss during training.

---

## Backpropagation
Backpropagation calculates how much each weight contributed to the prediction error and updates the weights accordingly.

---

## Gradient Descent
Gradient descent is used to update the network parameters step by step in the direction that reduces the loss.

---

# 💡 Important Concepts Learned

## Role of Weights and Biases
Weights determine the importance of input features, while biases help shift activation values and improve learning flexibility.

---

## Importance of Activation Functions
Activation functions introduce non-linearity, allowing the neural network to learn complex patterns from the data.

---

## Learning Rate
The learning rate controls how quickly the model updates its parameters during training.

- Very high learning rate → unstable training
- Very low learning rate → slow convergence

---

## Underfitting vs Overfitting

| Problem | Meaning |
|---|---|
| Underfitting | Model fails to learn patterns properly |
| Overfitting | Model memorizes training data and generalizes poorly |

Regularization and hyperparameter tuning help reduce overfitting.

---

# 📈 Final Results

| Metric | Performance |
|---|---|
| Training Accuracy | 100% |
| Testing Accuracy | 98.25% |
| Task Type | Binary Classification |
| Model Type | Feed-Forward Neural Network |

---

# 🚀 How to Run the Project

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Launch Jupyter Notebook

```bash
jupyter notebook notebook.ipynb
```

---

## Google Colab Option

1. Upload:
   - `notebook.ipynb`
   - `customer_churn_nn.csv`

2. Then select:

```text
Runtime → Run All
```

---

# 📚 References

1. Goodfellow et al. — *Deep Learning*
2. TensorFlow Keras Documentation
3. Scikit-learn Documentation
4. Nielsen, Michael — *Neural Networks and Deep Learning*
