[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

First create a pmf that breaks down the distrobution into percentages
Then plot it and configure the labels

```
resp = nsfg.ReadFemResp()
pmf = thinkstats2.Pmf(resp.numkdhh, label='numkdhh')
thinkplot.Pmf(pmf)
thinkplot.Config(xlabel='Number of Children', ylabel='PMF')
```

Next create a biased observed PMF as if it has been sampled

```
biased_pmf = BiasPmf(pmf, label='observed')
```

Then plot both pmfs using preplot

```
thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased_pmf])
thinkplot.Config(xlabel='Number of Children', ylabel='PMF')
```

```
pmf.Mean()
biased_pmf.Mean()
```

the means are 1.024205155043831 and 2.403679100664282 respectively, showing how drastically different bias one is from the true result
