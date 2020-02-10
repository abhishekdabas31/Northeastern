# Linear Regression

Linear Regression is the Linear Model that assumes that there is a linear relationship between the independent variable ('x') and dependent variable('Y') such that 'y' can be calculated from a linear combination of imput variables 'x'.
For single imput variable it is called simple Linear Regression, whereas for multiple imput variables it is called multiple linear regression.

Incase of 1 imput 'x' and 1 output 'y', there is an output line
Incase of multiple imputs "x's" the line is replaced by a plane

>>These two variables are called the independent variable and the dependent variable, and they are given these names for fairly intuitive reasons. The independent variable is so named because the model assumes that it can behave however it likes, and doesn’t depend on the other variable for any reason. The dependent variable is the opposite; the model assumes that it is a direct result of the independent variable, it’s value is highly dependent on the independent variable.

## minimizing the error between the model predictions and the actual data means performing the following steps for each x value in your data set:
First, use the linear regression equation, with values for A and B, to calculate predictions for each value of x;
Second, calculate the error for each value of x by subtracting the prediction for that x from the actual, known data;
Third, sum the error of all of the points to identify the total error from a linear regression equation using those values for A and B.
Error = (Actual — Prediction)²

## Since the linear regression model minimizes the squared error the solution is referred to as the least squares solution. This is the name for the combination of A and B that return the minimum squared error over the data set.

## Regression analysis is the science and art of fitting a straight line of pattern into data.
In a linear regression model, the variable of interest (the so-called “dependent” variable) is predicted from k
other variables (the so-called “independent” variables) using a linear equation. If Y denotes the
dependent variable, and X1, …, Xk, are the independent variables, then the assumption is that the
value of Y at time t (or row t) in the data sample is determined by the linear equation
`Y = β + β X + β X + ... + β X + ε`

## The art of Regression Modelling :-
Collect the data that is relative and informative with respect to your decision or inference problem and then define your variables and contruct your model 

## Choosing a good regression model requires 
(a) gathering useful data and making sure you know where it came from and how it was measured, 
(b) performing descriptive analysis on it to understand its general patterns and to spot data-quality problems, 
(c) applying appropriate data transformations if you see strong evidence of relationships that are nonlinear or noise that is non-normal or time-dependent, 
(d) fitting and refining and comparing models, 
(e) checking to see whether a given model’s assumptions are reasonably well satisfied or whether an alternative model is suggested, 
(f) choosing among reasonable models based on the appropriate bottom-line accuracy measure, and
(g) deriving some useful insights from the whole process.

## There are four principal assumptions which justify the use of linear regression models for purposes of inference or prediction:
1. linearity and additivity of the relationship between dependent and independent variables:
(a) The expected value of dependent variable is a straight-line function of each independent variable, holding the others fixed.
(b) The slope of that line does not depend on the values of the other variables.
© The effects of different independent variables on the expected value of the dependent variable are additive.
2. statistical independence of the errors (in particular, no correlation between consecutive errors in the case of time series data)
3. homoscedasticity (constant variance) of the errors
(a) versus time (in the case of time series data)
(b) versus the predictions
© versus any independent variable
4. normality of the error distribution.


>> Example:-
>>> Linear Regression is a very powerful statistical technique and can be used to generate insights on consumer behaviour, understanding business and factors influencing profitability. Linear regressions can be used in business to evaluate trends and make estimates or forecasts. For example, if a company’s sales have increased steadily every month for the past few years, by conducting a linear analysis on the sales data with monthly sales, the company could forecast sales in future months.

## How to check if model works well??
linear regression model this is typically done by calculating the coefficient of determination, or r² value. 
The coefficient of determination captures how much of the trend in the data set can be correctly predicted by the linear regression model. It’s a value ranging from 0 to 1, with lower values indicating worse fit and higher values indicating better fit.

## Limitations of Linear Regression:
1. The Linear Regression model is only capable of return straight lines. This makes it wholly unsuited to match data sets with any sort of curve in them, such as exponential or logarithmic trends.
2. linear regression only works when there’s a single dependent variable and a single independent variable. If you want to include multiple of either of those in your data set, you’ll need to use multiple regression










Source:-
1. http://people.duke.edu/~rnau/regintro.htm
2. Notes_on_linear_regression_analysis by Robert_Nau :- 
http://people.duke.edu/~rnau/Notes_on_linear_regression_analysis--Robert_Nau.pdf
3. https://medium.com/@srishtisawla/linear-regression-data-science-algorithm-every-data-scientist-should-know-34d5fcb51c03
4. https://towardsdatascience.com/understanding-the-fundamentals-of-linear-regression-7e64afd614e1