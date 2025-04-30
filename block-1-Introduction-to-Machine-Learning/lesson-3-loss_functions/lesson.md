# Lesson 3: Model Evaluation: Loss Functions

## Topics
- Importance of model quality evaluation
- Metrics
- Loss functions for regression (MSE, MAE) and classification (Cross-Entropy)

## Notes
Evaluating the quality of a machine learning model is crucial to ensure its effectiveness and reliability. Different metrics and loss functions are used to measure the performance of models in various tasks.

### Importance of Model Quality Evaluation
Model evaluation helps in understanding how well a model generalizes to new, unseen data. It also aids in comparing different models and selecting the best one for a given task.

### Metrics
Metrics are quantitative measures used to assess the performance of a model. Common metrics include accuracy, precision, recall, F1-score, and ROC-AUC.

### Loss Functions for Regression
1. **Mean Squared Error (MSE)**: Measures the average squared difference between the predicted and actual values. It is calculated as:
\[ \text{MSE} = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2 \]
2. **Mean Absolute Error (MAE)**: Measures the average absolute difference between the predicted and actual values. It is calculated as:
\[ \text{MAE} = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i| \]

### Loss Functions for Classification
1. **Cross-Entropy Loss**: Measures the difference between the true labels and the predicted probabilities. It is commonly used in classification tasks. For binary classification, it is calculated as:
\[ \text{Cross-Entropy} = -\frac{1}{n} \sum_{i=1}^{n} [y_i \log(\hat{y}_i) + (1 - y_i) \log(1 - \hat{y}_i)] \]

By using appropriate metrics and loss functions, we can effectively evaluate and improve the performance of machine learning models.
