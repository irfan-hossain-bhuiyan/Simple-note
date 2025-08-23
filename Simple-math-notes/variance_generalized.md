In variance $V[x]=E[(x-E[x])^2]$
Even though amazing in look you can $V[x]=E[x^2]-E[x]^2$ so you can split the power to separate it,
Here is the relation,$I=I_G+Mh^2$ can be mapped to $E[x^2]=V[x]+E[x]^2$
There are some amazing features,like $E[(x+h)^2]=V[x]+E[x+h]^2$
,Is there a way for it to work in high dimension,So the 
$\sum{(x+h)^2} can also be split into summation?$

Another view for variance,a lot of things can be understand
if we know what that things is symmetric too,Maybe that is the only way to uniquely understand everything.

The thing is variance is symmetric to transformation,
Like X being the datapoint,If we shift the entire data to the right by a amount so X+a,then the variance remains constant,So we can do something like,
$$Variance=(\frac{sum{f_i*d_i^2}}{N}-\(frac{f_i*d_i}{N})^2)*h^2$$
,this is possible because $Var[x]=Var[x+a]$

