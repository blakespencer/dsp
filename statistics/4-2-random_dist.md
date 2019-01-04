[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

Fist generate the random numbers

```
sample = np.random.random(1000)
```

Then create and plot the pmf

```
pmf = thinkstats2.Pmf(sample)
thinkplot.Pmf(pmf)
thinkplot.Config(xlabel='Random numbers', ylabel='PMF')
```

Here we can see that every number has nearly equal probability which is what we expect

So now we create the CMF which is easier to see

```
cdf = thinkstats2.Cdf(sample)
thinkplot.Cdf(cdf)
thinkplot.Config(xlabel='Random variate', ylabel='CDF')
```

And again we can see that the line is straight, thus confirming that it is truely random
