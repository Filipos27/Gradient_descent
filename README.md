# Gradient_descent
In this repository will be projects with gradient descent.
The goal of the gradient descent is to minimise a given function which, in our case, is the loss function of the neural network. To achieve this goal, it performs two steps iteratively:
1. Compute the slope (gradient) that is the first-order derivative of the function at the current point
2. Move-in the opposite direction of the slope increase from the current point by the computed amount

### Batch gradient descent
In Batch Gradient Descent, all the training data is taken into consideration to take a single step. We take the average of the gradients of all the training examples and then use that mean gradient to update our parameters. So that’s just one step of gradient descent in one epoch.

![batch](https://user-images.githubusercontent.com/77289083/109833753-d13bae80-7c41-11eb-98c1-3fb973d99810.png)



### Stohastic gradient descent
Stohastic gradient descent is an iterative method for optimizing an objective function with suitable smoothness properties (e.g. differentiable or subdifferentiable). It can be regarded as a stochastic approximation of gradient descent optimization, since it replaces the actual gradient (calculated from the entire data set) by an estimate thereof (calculated from a randomly selected subset of the data). Especially in high-dimensional optimization problems this reduces the computational burden, achieving faster iterations in trade for a lower convergence rate.
In Stochastic Gradient Descent (SGD), we consider just one example at a time to take a single step. We do the following steps in one epoch for SGD:
- Take an example
- Feed it to Neural Network
- Calculate it’s gradient
- Use the gradient we calculated in step 3 to update the weights
- Repeat steps 1–4 for all the examples in training dataset

![stoh](https://user-images.githubusercontent.com/77289083/109833855-e7496f00-7c41-11eb-99a8-5f850ea430ed.png)

## Project structure

1. Exploring data set (pandas)
2. Cleaning data set (pandas)
3. Data visualization (matplotlib,seaborn)
4. Preparing data,scaling (MinMaxScaler)
5. Predicting prices (batch gradient descent,stohastic gradient descent)
