
for f(x)=c1
then -> df(x)=0 which I represent as g(x)dx->0
but when I use f(x,y)=c1
-> df(x,y)=0 which is g(x,y)dx+h(x,y)dy=0
Does that mean 
df(x,y)=g(x,y)dx+h(x,y)dy so on,
It makes sense as 
df(x,y)/dx=g(x,y)dx/dx+h(x,y).dy/dx=g(x,y) as dy/dx=0 as y and x are independent of each other.
But there are some problems too.
Lets say f(x,y)=x^2.y^3
here df(x,y)=2x.y^3dx+3y^2.x^2dy
df(x,y)=dx^2.y^3+dy^3.x^2=2.d(x^2.y^3)

There is one way to fix this issue.In multivariable calculus,you always need to use partial deriavative.
New symbol d(x) is partial deriavative with respect to x.So, d(x)x^4=4x^3d(x)x where d(x)x can be just written as dx for shorthand.
So, likewise d(x)y is 0 if x is independent of y.
Now,df(x)+dg(x)=d(f(x)+g(x)) is only allowed if both have the derivative in respect to same variable.

so only d(x)f(x)+d(x)g(x)=d(x)(f(x)+g(x))

There are some questions
> How df(g(x))/dx=df(g(x))/dg(x).dg(x)/dx works even though d^2f(g(x))/(dx)^2=d^2f(g(x))/(dg(x))^2.(dg(x))^2/(dx)^2 doesn't work???
