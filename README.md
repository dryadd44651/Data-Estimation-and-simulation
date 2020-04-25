# Data_Estimation_and_simulation
This Project will show you how to estimate a function and parameters in the probability function

# Monte Carlo

## Pi estimation
- Get the sample points in rectangle 2x2
- Get the circle in the rectangle with radius 1
- Pi = points in circle/points in rectangle
## Satellite lifetime probability estimation
- Get random generation for the exponential distribution to get the sample lifetime
- To make statistic and get the information we want

# Maximum Likelihood Estimator (Parameters Estimator)

## The normal way to find the parameter
- Get Sample
- Get objective function by multiply probability density function
- Get likelihood function
- Get equation by differentiating likelihood function and set to zero
- Put sample value into the equation and get the parameter

## Maximum Likelihood Estimator
- Get Sample
- Get objective function by multiply probability density function
- Get likelihood function and multiply by minus one
- Get the parameter by minimizing the negative function(maximizing likelihood function) by optim R function

when we don't know how to or can't differential equations.

We can easily use Maximum Likelihood Estimator to find out the parameters

# bootstrap estimator

- Set the estimator size we want(ex: 1000)
- Eestimate each sample by ramdon sampling(i from 1~1000)
>- EX: data = 1 2 3 4, estimate[i] = 3 4 2 2(take and put it back)
>- est_data[i] = Mean(estimate[i])
- Once we get est_data we can get what ever information we want
>- mean
>- var
>- CI

# Parameter VS Non-parameter Bootstrap
- key different: How to generate the bootstrap sample data
>- From Parameter(known before the test) or Input data

