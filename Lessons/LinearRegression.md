# Linear Regression

## What is linear regression and what is its application? (5 min)

## Visualize the simple linear regression when have single-input single-output data (5 min)

## Mathematical formulation of linear regression and what the objective function is to be minimized (5 min)

## Activity: write a Python code to obtain the coefficient and intercept of a simple linear regression (15 min)
- The X and Y as the single-input single-output data are given
- Use numpy np.polyfit and np.poly1d to obtain the linear regression model coefficients
- Use sklearn from sklearn.linear_model import LinearRegression to obtain the linear regression model coefficients

## Multiple Linear Regression is introduced and advertising dataset is given and explored (5 min)

## Activity: Obtain linear regression model parameters for advertising dataset (20 min)

- Load Advertising.csv
- Use from sklearn.linear_model import LinearRegression and import statsmodels.formula.api as smf
- Compare the result and sklearn with ordinary least square (OLS) from statsmodels
- Good resource for OLS: https://www.statsmodels.org/stable/regression.html

## Break (10 min)

## How to evaluate linear regression model? (5 min)
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R-Squared

## Activity: Obtain the R-squared for linear model fitted for advertising data (15 min)

## Optional reading for closed-form solution of linear regression model (10 min)

## Introduce the challenges and stretch challenges for linear regression (10 min)
