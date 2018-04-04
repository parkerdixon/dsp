[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> import nsfg <br />
  import thinkstats2 <br />
  import thinkplot <br />
  def BiasPmf(pmf, label):<br />
      new_pmf = pmf.Copy(label=label)<br />
      for x, p in pmf.Items():<br />
          new_pmf.Mult(x, x)<br />
          new_pmf.Normalize()<br />
      return new_pmf<br />
  resp = nsfg.ReadFemResp()<br />
  numChildren = resp.numkdhh<br />
  pmf = thinkstats2.Pmf(numChildren)<br />
  biasedPmf = BiasPmf(pmf, label='Biased')<br />
  thinkplot.PrePlot(2)<br />
  thinkplot.Pmfs([pmf, biasedPmf])<br />
  thinkplot.Config(xlabel='Number of Children', ylabel='Probability')<br />
  unbiasedMean = pmf.Mean()<br />
  biasedMean = biasedPmf.Mean()<br />
