## Perceptron: Understanding the Basics

A perceptron is a basic unit of a neural network, often considered the simplest type of neural network model. It serves as the foundation for more complex neural networks and is used for binary classification tasks. The perceptron operates by applying a linear transformation to input data and then using an activation function to generate a binary output.

![Perceptron Structure](https://miro.medium.com/v2/resize:fit:916/1*_xbbcmL06_nXADsGK1TAug.png)

### How a Perceptron Works

Imagine you have a set of features (inputs) and you want to predict a binary outcome (like whether an email is spam or not). A perceptron learns to find a linear boundary that separates these two classes.

A perceptron has:
- **Weights:** A set of parameters, one for each input feature.
- **Bias:** A scalar added to the weighted sum of inputs to allow flexibility in shifting the decision boundary.
- **Activation Function:** Determines whether the perceptron outputs a 0 or 1 based on the linear combination of the weights and bias.

The output is determined by:

![Formula for Perceptron Output](https://pabloinsente.github.io/assets/post-5/perceptron-math.png)

where \( x_i \) are the input features, \( w_i \) are the weights, and \( b \) is the bias. The activation function outputs 1 if the weighted sum is greater than or equal to 0, and 0 otherwise.

### Training a Perceptron

Training a perceptron involves adjusting the weights and bias based on the error between the predicted and actual outputs. This adjustment is done using a learning rate to control how much the weights and bias change at each step.

Here's the general training process:
1. **Initialize weights and bias to zero.**
2. **Loop through each training sample:**
   - Calculate the linear output and apply the activation function to get the prediction.
   - Compare the prediction with the actual output.
   - If the prediction is incorrect, adjust the weights and bias accordingly using the error.

### Limitations of Perceptrons

Perceptrons have their limitations:
- **Linearity:** They can only learn linear boundaries, which makes them less effective for complex, non-linear problems.
- **Binary Classification:** Perceptrons are designed for binary outcomes. Multiclass classification requires additional methods.

### Example Perceptron Implementation

In this example, we implemented a perceptron from scratch to classify a binary outcome using a dataset. The example covered:
- Building the perceptron class.
- Training the perceptron with a dataset.
- Evaluating the accuracy of the perceptron on a test set.
- Visualizing the decision boundary.

The code snippet demonstrates a simple perceptron with adjustable learning rate and epochs, allowing for easy experimentation and learning.

