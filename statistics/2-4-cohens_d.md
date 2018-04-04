[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

>> firsts, others = first.MakeFrames()

xBar1 = firsts.totalwgt_lb.mean()
xBar2 = others.totalwgt_lb.mean()
n1 = firsts.count(numeric_only=True)
n2 = others.count(numeric_only=True)
s1 = firsts.totalwgt_lb.var()
s2 = others.totalwgt_lb.var()
diff = xBar1 - xBar2
pooled_var = (n1.totalwgt_lb * s1 + n2.totalwgt_lb * s2)/(n1.totalwgt_lb + n2.totalwgt_lb)
d = diff / pooled_var ** .5
