# Neural Networks Basics

Welcome to the **Neural Networks Basics** repository! This repository is part of my [30-Day Machine Learning Learning Path](https://link.medium.com/3QdCOGokdPb) and provides the code and resources for Day 15, where we explore the fundamentals of neural networks.

## Table of Contents

- [Introduction](#introduction)
- [Key Concepts](#key-concepts)
- [Getting Started](#getting-started)
  - [Requirements](#requirements)
  - [Installation](#installation)
- [Code Walkthrough](#code-walkthrough)
- [Resources](#resources)

## Introduction

Neural Networks are inspired by the human brain and form the backbone of modern machine learning and deep learning systems. This session covers:

- The structure of neural networks (input layer, hidden layers, and output layer).
- Activation functions such as ReLU, Sigmoid, and Softmax.
- Building and training a simple neural network using TensorFlow/Keras.
- Understanding the learning process through forward propagation, loss calculation, and backpropagation.

## Key Concepts

- **Input Layer**: Takes raw data (e.g., images, text).
- **Hidden Layers**: Process data with weights and activation functions.
- **Output Layer**: Produces final predictions or classifications.
- **Activation Functions**: Introduce non-linearity (e.g., ReLU, Sigmoid, Softmax).
- **Optimization**: Use algorithms like Adam to minimize the loss.

## Getting Started

### Requirements

Ensure you have the following installed:

- Python 3.8 or higher
- TensorFlow 2.x
- NumPy
- Matplotlib (optional, for visualization)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/neural-networks-basics.git
   cd neural-networks-basics
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the code:
   ```bash
   python neural_network_basics.py
   ```

## Code Walkthrough

### Model Definition

```python
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Flatten, Dense
from tensorflow.keras.optimizers import Adam

# Define the model
model = Sequential([
    Flatten(input_shape=(28, 28)),  # Flatten 2D input to 1D
    Dense(128, activation='relu'),  # Hidden layer
    Dense(10, activation='softmax')  # Output layer
])

# Compile the model
model.compile(optimizer=Adam(),
              loss='sparse_categorical_crossentropy',
              metrics=['accuracy'])

# Train the model
model.fit(X_train, y_train, epochs=5, batch_size=32)
```

### Evaluation

```python
# Evaluate the model
test_loss, test_acc = model.evaluate(X_test, y_test)
print("Test accuracy:", test_acc)
```

For full details, see the `neural_network_basics.py` file in this repository.

## Resources

- [Neural Networks and Deep Learning Book by Michael Nielsen](http://neuralnetworksanddeeplearning.com/)
- [Andrew Ng's Deep Learning Specialization](https://www.coursera.org/specializations/deep-learning)
- [ReLU Activation Function - GeeksforGeeks](https://www.geeksforgeeks.org/relu-activation-function-in-deep-learning/)
- [TensorFlow Keras Documentation](https://www.tensorflow.org/guide/keras)
- YouTube Videos:
  - [Neural Networks - Simplified](https://www.youtube.com/watch?v=aircAruvnKk)
  - [Building Neural Networks in TensorFlow](https://www.youtube.com/watch?v=tPYj3fFJGjk)


If you find this repository useful, feel free to give it a star ⭐ and share your feedback. For questions or collaborations, reach out to me on [LinkedIn]([https://www.linkedin.com/in/kartik-garg-99a754252/])!
