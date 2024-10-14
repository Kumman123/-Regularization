# Ridge and Lasso Regularization Comparison

This project demonstrates the application and comparison of **Ridge** and **Lasso** regression techniques using Python. It implements both methods from scratch using their mathematical formulas and compares the models based on error metrics and visual plots.

## Project Overview

In this project, we explore two regularization techniques used in regression:
1. **Ridge Regression** - Adds a penalty proportional to the square of the magnitude of the coefficients.
2. **Lasso Regression** - Adds a penalty proportional to the absolute value of the coefficients, potentially driving some coefficients to zero.

We use a sample dataset:
- X = [1, 2, 3, 4]
- y = [2, 4, 6, 9]

### Key Features:
- Compute Ridge and Lasso regression coefficients using their mathematical formulas.
- Compare both models based on Mean Squared Error (MSE) and R-squared values.
- Visualize the resulting regression lines.
- Use the sklearn library to compute and validate the results.
  
## Dataset

The dataset used in this project is as follows:
We use a sample dataset:
- X = [1, 2, 3, 4]
- y = [2, 4, 6, 9]



## Code Structure

The code is implemented in the following steps:

. **Data Preparation**: 
   - Load and normalize the data.
   
### Ridge Regression Formula:

The formula for Ridge regression is:

$$
w_1 = \frac{\sum (X - \text{mean}(X))(y - \text{mean}(y))}{\sum (X - \text{mean}(X))^2 + \lambda}
$$

Where:
- \(X\) is the feature matrix.
- \(y\) is the target/output.
- \(\lambda\) is the regularization parameter.


### Lasso Regression Formula:

For Lasso regression, the coefficient \( w_1 \) is computed as:

$$
w_1 = \frac{\text{sign}(numerator) \cdot \max(0, |numerator| - \lambda)}{denominator}
$$

Where:
- \( \lambda \) is the Lasso regularization parameter.

. **Comparison**:
   - Calculate MSE and \( R^2 \) score for both Ridge and Lasso models.
   - Plot the regression lines for both models to visualize the difference.

## Requirements

To run the code, you will need the following Python libraries:

- `numpy`
- `matplotlib`
- `sklearn`

You can install the required libraries using pip:

```bash
pip install numpy matplotlib scikit-learn
