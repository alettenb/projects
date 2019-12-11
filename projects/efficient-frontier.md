---
layout: post
title: 'Efficient Frontier'
---
## About
In this, I create code to take an arbitrary number of stocks and craft an
efficient frontier for it. An efficient frontier is the optimal weight of
stocks used to maximize return. My code uses the expected return and 
standard deviation of the stocks from as far back as possible (the most recently
created company's first trade date). The code is still a work in progress,
and if you want to mess around with it, the repository can be found
[here](https://github.com/alettenb/efficientfrontier).

## Example
The graph below showcases some functionality of the generator. In this, 
I find the Efficient Frontier for Proctor and Gamble, Google, Apple, and
J.P. Morgan. You can hover over the orange dots to see which stock is which.
The red dot represents the stock weights maximizing the utility function,

<center><p>\(U = w \mu^T - \alpha w^T \Sigma w\),</p></center>

where *w* represents the weights of the stocks, *α* represents risk aversion, 
*μ* represents the vector of mean returns, and *Σ* represents the 
variance-covariance matrix for the stocks.

{% include efficient-frontier/efficient_frontier.html  %}

