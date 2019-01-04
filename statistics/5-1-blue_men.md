[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

To find the percentage of the population between heights 5'10 and 6'1 we can use the CDF and minus them
µ = 178 cm and σ = 7.7 cm

```
import scipy.stats
mu = 178
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)
```

now we can compute the percentages with CMF, which will give us the percentage of people upto a given height

```
low = dist.cdf(177.8)    # 5'10"
high = dist.cdf(185.4)
high - low
```

0.34209468294595308 so 34% of people are in that range
