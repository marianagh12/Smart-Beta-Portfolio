# Proyecto-Final
## Smart Beta Portfolio Project

This smart beta portfolio construction seeks for the ultimate combination of low risk and high profits using traditional ways like diversification combined with the implementation of machine learning algorithms

### Process

The universe for this portfolio is created by stocks from the tech industry listed on NASDAQ and NYSE but also listed
on the international market of Mexico (SIC).
	 

## The construction of this portfolio has 3 steps:

1. Selection of top 5
2. Creation of the portfolio sample 
3. Optimization of the final 20 stocks.


## Selection of top 5

```markdown

Taking the 40 stocks that conform the universe, each of these has a combined Score of 3 metrics
weighted as below:

* Price Momentum = Shows the rate of change in price movement over a year.(.35)

* Volatility = The fluctuation of price in a year.(.35)

* Company Size = (# stocks that are public or able to trade * price of the stock)(.30)

The top 5 stocks with the better combined score are selected.

These measures were choosen due to the necessity to create a portfolio with great returns.

```

## Creating the Porfolio sample.

```markdown

* Once we selected the top 5 stocks, we take the original universe of 40 stocks, calculate a daily return 
for the prices over a year.

* This data is clustered using the KMeans algorithm in Python.
* Once the data is clustered we take the 15 stocks nearest to the top 5 in distance.

```

# Optimization of the portfolio

```markdown

* We have the ultimate collection of tech stocks for the porftolio, now we have to select the best combination to generate 
better returns, to do this we use the optimization model for portfolios called the efficient frontier that allows you to 
get the highest return for the lowest possible risk

