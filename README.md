<div align="center">
      <h1><br/>Linear Regression With Short Introduction</h1>
     </div>


Linear regression is a statistical technique used to model the relationship between a dependent variable (also known as the response variable) and one or more independent variables (also known as explanatory variables). It is used to predict the value of the dependent variable based on the values of the independent variables. The linear regression model is represented by an equation of the form: Y = β0 + β1X1 + β2X2 + ... + βnXn, where Y is the dependent variable, X1, X2, ..., Xn are the independent variables, and β0, β1, β2, ..., βn are the coefficients of the model. The coefficients are estimated using a method called least squares, which minimizes the sum of the squared errors between the observed values of the dependent variable and the predicted values of the dependent variable. Once the coefficients have been estimated, the linear regression model can be used to make predictions about the dependent variable given values of the independent variables.

``` python
#code for linear regression:

import numpy as np
from sklearn.linear_model import LinearRegression

# Create the data
x = np.array([[1, 1], [1, 2], [2, 2], [2, 3]])
y = np.array([1, 2, 3, 4])

# Create the linear regression model
model = LinearRegression()

# Fit the model to the data
model.fit(x, y)

# Get the coefficients
coefficients = model.coef_

# Get the intercept
intercept = model.intercept_

# Print the coefficients and intercept
print('Coefficients:', coefficients)
print('Intercept:', intercept)
```

### Output:

``` python
Coefficients: [1. 1.]
Intercept: -1.0
```
#### <a href ="http://ahammedmejbah.com">Credit: Mejbah Ahammad</a>
    
