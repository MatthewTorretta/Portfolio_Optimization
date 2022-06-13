# Portfolio_Optimization
Calculating expected annual returns and optimal portfolios using python. 

In the estimation of the parameters of an optimal portfolio, the historical inputs will make a big difference in the results. Given that
druing Feb-March 2020 there has been an ongoing financial crisis related to the
COVID-19 disease, I am going to analyse two models for the input of historical data:

Dow Jones Industrial, S&P500, FTSE100, EZU, and Gold prices.

From [ 27-Jan-2020 to 23-March-2020 ] and from the 5 years between [ January 2015 until December 2019 ].

Calculations included:

- Expected Annual Returns
- Expected Annual Covariance Matrix
- Annualized portfolio return
- Annualized portfolio variance
- Annualized portfolio volatility
- Monte Carlo simulation of portfolio weights (The optimal portfolio weights)
- Optimal Portfolio (Volatility of the optimal portfolio, The optimal portfolio return)
- Maximum Sharpe Ratio
- Minimum Variance Portfolio
- Efficient Frontier

Given that the amount of observations for the Model 1 case is small, a eigenvector bias is produced in the estimation of the Covariance.

The main advantage of the shrinkage method is that it attempts to improve the
accuracy of covariance matrix estimation. For portfolio optimisation, it is required that the
estimated covariance matrix is non singular (invertible) and positive definite (eigenvalues are
positive).
In the case of Model 1, the estimated annual covariance matrix technically is stable
since the number of observations is more than the number of securities that comprise the
portfolio. Yet with such a small number of observations, the shrinkage method is the best bet
to optimise the portfolio. Until T (number of observations) is significantly larger than N
(number of assets), problems with our optimisation will arise.

Using the estimated shrinkage I found the new Expected Annual Covariance Matrix.

