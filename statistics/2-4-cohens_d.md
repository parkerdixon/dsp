[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

>> firsts, others = first.MakeFrames()/n
  xBar1 = firsts.totalwgt_lb.mean()/n
  xBar2 = others.totalwgt_lb.mean()/n
  n1 = firsts.count(numeric_only=True)/n
  n2 = others.count(numeric_only=True)/n
  s1 = firsts.totalwgt_lb.var()/n
  s2 = others.totalwgt_lb.var()/n
  diff = xBar1 - xBar2/n
  pooled_var = (n1.totalwgt_lb * s1 + n2.totalwgt_lb * s2)/(n1.totalwgt_lb + n2.totalwgt_lb)/n
  d = diff / pooled_var ** .5/n
