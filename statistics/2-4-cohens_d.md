[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

>> firsts, others = first.MakeFrames() <br />
  xBar1 = firsts.totalwgt_lb.mean()<br />
  xBar2 = others.totalwgt_lb.mean()<br />
  n1 = firsts.count(numeric_only=True)<br />
  n2 = others.count(numeric_only=True)<br />
  s1 = firsts.totalwgt_lb.var()<br />
  s2 = others.totalwgt_lb.var()<br />
  diff = xBar1 - xBar2<br />
  pooled_var = (n1.totalwgt_lb * s1 + n2.totalwgt_lb * s2)/(n1.totalwgt_lb + n2.totalwgt_lb)<br />
  d = diff / pooled_var ** .5<br />
