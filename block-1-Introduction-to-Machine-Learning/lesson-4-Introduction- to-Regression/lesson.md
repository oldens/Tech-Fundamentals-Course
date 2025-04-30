# Lesson 4: Introduction to Regression: Linear Regression

## Topics
- Problem formulation of regression
- Linear regression model
- Idea of least squares method and gradient descent (conceptually)

## Notes
Regression is a type of supervised learning task that involves predicting a continuous target variable based on one or more input features. Linear regression is one of the simplest and most widely used regression techniques.

### Problem Formulation of Regression
In regression, the goal is to find a function that maps input features to a continuous target variable. The problem can be formulated as:
\[ y = f(X) + \epsilon \]
Where:
- \( y \) is the target variable
- \( X \) is the input features
- \( f \) is the function that maps \( X \) to \( y \)
- \( \epsilon \) is the error term

### Linear Regression Model
Linear regression assumes a linear relationship between the input features and the target variable. The model can be represented as:
\[ y = \beta_0 + \beta_1 X_1 + \beta_2 X_2 + \ldots + \beta_p X_p + \epsilon \]
Where:
- \( \beta_0 \) is the intercept
- \( \beta_1, \beta_2, \ldots, \beta_p \) are the coefficients for the input features
- \( X_1, X_2, \ldots, X_p \) are the input features
- \( \epsilon \) is the error term

### Idea of Least Squares Method and Gradient Descent (Conceptually)
1. **Least Squares Method**: The least squares method aims to find the coefficients that minimize the sum of the squared differences between the predicted and actual values. The objective function is:
\[ \text{Minimize} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2 \]
Where:
- \( y_i \) is the actual value
- \( \hat{y}_i \) is the predicted value

2. **Gradient Descent**: Gradient descent is an optimization algorithm used to minimize the objective function by iteratively updating the coefficients. The update rule is:
\[ \beta_j = \beta_j - \alpha \frac{\partial J}{\partial \beta_j} \]
Where:
- \( \beta_j \) is the coefficient
- \( \alpha \) is the learning rate
- \( J \) is the objective function
- \( \frac{\partial J}{\partial \beta_j} \) is the partial derivative of the objective function with respect to \( \beta_j \)

By understanding the concepts of linear regression, least squares method, and gradient descent, we can build and train regression models to make accurate predictions.
