# GRADIENT DESCENT

Gradient descent is an optimization algorithm used to find the local minimum of a differentiable function. It's a core concept in many machine learning algorithms, including linear regression and neural networks, where it's used to optimize coefficients to minimize a cost function.

### A Hiking Analogy
Imagine you're hiking in a mountainous region, and you want to find the fastest way down to the valley's lowest point. The valley represents your cost function, and you're looking for the quickest route down. At each point in the journey, you have multiple options for which direction to go, but you want the steepest path. This is where the concept of the gradient comes in. The gradient indicates the steepest slope, guiding you to the quickest descent.

![Hiking Analogy](https://miro.medium.com/v2/resize:fit:1400/1*DDjCOEPSHLsU7tff7LmYUQ.png)

### Understanding Gradient Descent
Gradient descent works by initializing at a starting point, then iteratively taking steps in the direction of steepest descent, guided by the gradient. The size of these steps is known as the learning rate. Too large a learning rate might cause you to overshoot and miss the local minimum, while too small a rate could mean it takes too long to reach the bottom. 

Mathematically, gradient descent can be expressed as:
![Gradient Algo](https://miro.medium.com/v2/resize:fit:1400/1*OHLLc-i6QOCT3cQddwCL2A.jpeg)

### Types of Gradient Descent
There are two main types of gradient descent:

1. **Batch Gradient Descent (Vanilla Gradient Descent)**
   - Computes the gradient for the entire dataset before updating the model parameters.
   - The process where all data points are used to compute the gradient is called an "epoch."
   - **Advantages**: Produces a stable gradient, resulting in smoother convergence. Efficient for large datasets.
   - **Disadvantages**: Can be computationally intensive. Requires the entire dataset to be in memory.

2. **Stochastic Gradient Descent (SGD)**
   - Computes the gradient and updates the model parameters for each training example one-by-one.
   - **Advantages**: Faster updates, especially with large datasets, and can escape local minima due to its inherent noise.
   - **Disadvantages**: The updates can be noisy, resulting in oscillations or slow convergence.

### Practical Applications
Gradient descent is widely used in machine learning to train models such as linear regression, logistic regression, and neural networks. By iteratively adjusting the model's parameters, it aims to minimize the cost function, leading to better predictions or classifications.

### Common Cost Function: Mean Squared Error (MSE)
In linear regression, one common cost function used is the Mean Squared Error (MSE). It measures the average squared difference between predicted and actual values. Mathematically, it is represented as:

![MSE](https://miro.medium.com/v2/resize:fit:1400/1*WDGwqWArsoIcj1x8CY_fNw.png)
### Conclusion
Gradient descent is a powerful tool in machine learning and optimization, guiding us toward minimizing a cost function. Understanding the different types of gradient descent and their applications is crucial for effectively using machine learning algorithms.

