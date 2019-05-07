# Linear-regression-from-scratch
Linear Regression from Scratch in Python without using Scikit-learn

In this exercise, I will look at two different approaches to implemet linear regression or more precisely estimate linear regression co-efficients (also called weights or theta in ML jargon, I have reffered to it as theta in following code). The puprose of this exercise is to understand how these two approaches works and simulate it using python based on a toy dataset.

### Linear Regression

Statistically speaking, Linear regression is used to model relationship between a dependent variable (target vector) and a given set of independent variables (input variables). It assumes that there is a linear(i.e. staright line) relationship between dependent variable (target vector) and independent variables (input variables)

In simple terms, target variable(y) can be calculated as a linear combination of the input variables (X). If there is just a  single input variable, it is called simple linear regression. If there are more than one input variables , it is called multiple linear regression.

The equation for linear regression line is:

y = theta_0 + theta \* x

Here, theta_0 and theta are the coefficients that are estimated from the input variables and target vector. Once they are calculated these values can used to predict target values for new data that comes in.

The two approaches are:
* Linear regression with Normal equation
* Linear regression with Gradient Descent

The key differences between the two approaches are:
* Normal equation involves calculation of input variable's matrix inverse and matrix multiplication, hence gives a one shot answer for theta values.Suited for small datatsets only as matrix inverse and matrix multiplication are computaionally expensive operations.
* Gradient Descent invovles mimizing a cost function over multiple iterartions. This technique is computationally less expensive and well suited for large datasets. Does not always give the optimal values of theta.


In the following exercise we will estimate the values of theta using both approaches and see how the values for theta differ. 
