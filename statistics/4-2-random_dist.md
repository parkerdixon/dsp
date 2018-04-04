[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>> import numpy as np <br />
  import thinkstats2<br />
  import thinkplot<br />
  rand = np.random.random(1000)<br />
  pmf = thinkstats2.Pmf(rand)<br />
  thinkplot.Pmf(pmf, linewidth=.15)<br />
  thinkplot.Config(xlabel='Random Series', ylabel='PMF')<br />
  """<br />
  Based on the plot produced from the distribution, it seems that the random generation does indeed produce a uniform distribution<br />
  """<br />
