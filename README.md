# MNIST Handwritten Digit Classification

This project uses the **MNIST dataset** to train a neural network that classifies handwritten digits (0–9) using **TensorFlow/Keras**.

## Dataset
The [MNIST dataset](http://yann.lecun.com/exdb/mnist/) contains:
- **60,000 training images**
- **10,000 test images**
- Grayscale images of size **28×28 pixels**

Each image represents a single digit (0–9).

## Project Workflow
1. **Load the dataset** using `keras.datasets.mnist`.
2. **Normalize** pixel values from `[0, 255]` to `[0, 1]`.
3. **Build a neural network** with:
   - Flatten layer
   - Dense (128, ReLU)
   - Dense (10, Softmax)
4. **Compile the model** with:
   - Optimizer: Adam
   - Loss: Sparse Categorical Crossentropy
   - Metric: Accuracy
5. **Train** for 5 epochs with validation split.
6. **Evaluate** on the test set.

## Installation
Make sure you have Python 3.8+ installed, then install dependencies:
```bash
pip install tensorflow
