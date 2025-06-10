## Understanding catlan number

1. Understand catlan number,unferstand all formula for finding catlan number.
2. Relation between tree and catlan number.

Catlan number is used for all permutation of brackets,I can calculate recursively using,  
$C_a(n,r)=1 if a=n else C(n+1,r)+ C(n,r+1) if n>r else 0$
$C_n=C_n(0,0)$
#### else
$C(n,r)=1 if C(0,r) else C(n-1,r+1)+C(n,r-1)if 0<r else 0$
