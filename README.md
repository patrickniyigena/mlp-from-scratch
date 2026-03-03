# Multilayer Perceptron (MLP) from Scratch

This repository contains a complete, from-scratch implementation of a Multilayer Perceptron (MLP) using only NumPy. It was developed for the 18-786 Introduction to Deep Learning course.

The goal of this project is to demystify the inner workings of modern deep learning frameworks by manually implementing forward propagation, backpropagation, and various optimization algorithms.

## Features

* **Dynamic Architecture:** Supports an arbitrary number of hidden layers and perceptrons per layer.
* **Activation Functions:** Custom implementations of ReLU, Sigmoid, Tanh, and Linear activations, along with their derivatives.
* **Weight Initialization:** Supports both Xavier (Glorot) and He initialization strategies.
* **Loss Functions:** Includes Mean Squared Error ($l_{2}^{2}$) and Cross-Entropy (CE) loss.
* **Custom Optimizers:** Includes implementations of:
  * Vanilla Stochastic Gradient Descent (SGD)
  * SGD with Momentum
  * Adam
* **Non-linear Embeddings:** Demonstrates how mapping inputs to higher-dimensional spaces (e.g., $x_{i}^{2}+y_{i}^{2}$) can simplify complex classification problems like the XOR and Swiss Roll datasets.

## Datasets

The network is tested and validated against five distinct 2D toy datasets:
1. Linear-separable
2. Circle
3. XOR
4. Sinusoid 
5. Swiss-roll 

## Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/patrickniyigena/mlp-from-scratch.git
   cd mlp-from-scratch# mlp-from-scratch
   ```
2. **Install dependencies:**
This project strictly relies on standard Python libraries to ensure the underlying math is implemented manually.
```Bash
pip install numpy matplotlib
```
3. **Run the experiments:**
Execute main.py to run the training sequences across all deliverables. The script will output loss curves and decision boundary visualizations for each dataset.
```Bash
python main.py
```
**Note:** Generated visualizations are automatically saved to the /images directory.

## Results
The model achieves >95% validation accuracy on complex non-linear datasets (such as XOR and Sinusoid) and >90% on the Swiss Roll dataset  by leveraging appropriate deep architectures, Adam optimization, and non-linear feature embeddings.

## Acknowledgments
Starter code for dataset generation (numpyNN.py) was provided as part of the course materials for 18-786.
