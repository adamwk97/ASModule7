Advanced Statistics Module 7 - Confidence Interval Estimation And introduction to Fundamental of hypothesis testing
================

Question 1
==========

-   x̄ = 85 and σ = 8, and n = 64, set up a 95% confidence interval estimate of the population mean μ.

``` r
z = round(qnorm(.95),4)
me = z*(8/sqrt(64))
me = round(me,4)


cipos = round((85+me),4)
cineg = round((85-me),4)
```

We are 95% confident that the population mean falls within 86.6449 and 83.3551.

Question 2
==========

-   If x̄ = 125, σ = 24 and n = 36, set up a 99% confidence interval estimate of the population mean μ.

``` r
me = qnorm(.99)*24/sqrt(36)
cipos = round((125+me),4)
cineg = round((125-me),4)
```

We are 99% confident that the population mean falls within 115.6946 and 134.3054.

Question 3
==========

-   The manager of a supply store wants to estimate the actual amount of paint contained in 1-gallon cans purchased from a nationally known manufacturer. It is known from the manufacturer's specification sheet that standard deviation of the amount of paint is equal to 0.02 gallon. A Random sample of 50 cans is selected and the sample mean amount of paint per 1 gallon is 0.99 gallon.

-   Set up a 99% confidence interval estimate of the true population mean amount of paint included in 1-gallon can?

``` r
me = qnorm(.99)*.02/sqrt(50)
cineg = round((.99 - me),4)
cipos = round((.99 + me),4)
```

We are 99% confident that the population mean falls within 0.9834 and 0.9966.

-   On the basis of your results, do you think that the manager has a right to complain to the manufacturer? why?

I believe that while the manager has the right to be upset, he should not be complaining to the company. The confidence interval lands between 0.9966 and 0.9834, meaning is is within the .02 gallons of deviation specified by the manufacturer. The manager may be upset that his paint cans is in the lower half of 1.00 and not above, however there is stilll 99% confidence that his paint cans are within the single standard deviation that was given meaning the information provided upon purchase was legitimate.

Questions \# 4, 4a and 4b
=========================

-   A stationery store wants to estimate the mean retail value of greeting cards that has in its inventory. A random sample of 20 greeting cards indicates an average value of $1.67 and standard deviation of $0.32

-   Assuming a normal distribution set up with 95% confidence interval estimate of the mean value of all greeting cards stored in the store's inventory.

``` r
me = qnorm(.95)*(.32/sqrt(20))
cineg = round((1.67-me),4)
cipos = round((1.67+me),4)
```

We are 95% confident that the mean value of all greeting cards stored in the store's inventory is between 1.5523 and 1.7877.

-   How might the result obtained in (a) be useful in assisting the store owner to estimate of the mean value of all greeting cards in the store's inventory.

The result obtained in (a) may be useful because it gives a rough estimate of the store's entire inventory, and this number can be more precise with a larger sample as well as a more precise confidence value. The owner could also estimate the total worth by multiplying the total number of cards by the average of the two confidence intervals.

Question \# 5
=============

-   If you want to be 95% confident of estimating the population mean to within a sampling error of ± 5 and standard deviation is assumed to be equal 15, what sample size is required?

``` r
n = ((qnorm(.95)*15)/5)^2
```

If we want to be 95% confident for estimating this population mean to be within a sampling error of ± 5 and a standard deviation assumed to be equal to 15, we need a minimum sample size of 24.

Question \# 6
=============

-   Generate your own null and alternative hypothesis statements and provide rationale for your selection.

Null Hypothesis example: Age has no effect on competency levels with technology. Alternative Hypothesis Example: Age does have effect on competency levels with technology.

I chose these two as my hypotheses because I believe they are easy and straightforward. The null hypothesis infers that age does not have an effect on technological competence because the null hypothesis is meant to find no correlation. While the alternative hypothesis infers there is a correlation, and we have to decide whether or not to reject the null hypothesis and conclude correlation or a lack of.
