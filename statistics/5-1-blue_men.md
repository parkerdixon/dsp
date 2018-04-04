[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> import scipy.stats <br />
  mu = 178<br />
  sigma = 7.7<br />
  heightDist = scipy.stats.norm(loc=mu, scale=sigma)<br />
  lowEnd = heightDist.cdf(177.8)<br />
  highEnd = heightDist.cdf(185.4)<br />
  bmgRange = highEnd - lowEnd<br />
