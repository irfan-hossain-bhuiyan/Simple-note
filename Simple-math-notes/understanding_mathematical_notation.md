# It is been very good time.
Any way I look it it now works: 
$$\forall x \forall \epsilon \exists \phi |(|x-y|<\phi \Rightarrow |f(x)-f(y)|<\epsilon)....(i)$$

There are several issue in the notation for one directional notation.
First for the upper case proposition,for $eq (i)$
$$(|x-y|<\phi \Rightarrow |f(x)-f(y)|<\epsilon)$$ 

the $P\Rightarrow Q$ output False for $P=False$

But for some thing like $\forall x ((x>1)\Rightarrow (x^2>x))$.Here $\Rightarrow$ output False for $P=False$


So my other hypothesis is $\Rightarrow$ and $\implies$ is not the same thing.$P \Rightarrow Q$ return false for $P=False$ where as $P \implies Q$ returns $True$ for $P=False$

