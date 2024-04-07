seieve algorithm which is used to filter out the prime number,It is not optimized,

I want to optimize it,to the point of O(N),like 
first I have to cut out everything that is divisible by 2,then 3,now when cutting out 6,I have to cut it both 
for 3 and 2.I want to optimize it.
Like when start cutting always start from P**2,the code will be like
```python
l=[True]*inf
l[0]=False
l[1]=False
index=0
while True:
    if(l[index]){
        for x in range(index,inf):
            l[x*index]=False
    }
    index+=1
```
This is because say,the code is now iterating 5,I just have to 
start from 5*5=25,as all the previous one have been cut out by other 
prime factor

Is there a reason that the optimization techinique like 
```python 
prime=[]
for x in range(2,inf): #If I would include 1 in the prime number.No other number number will 
                       #included in the prime number.I wonder what if I exclude 2,the number that got 
                       #generated,is there any properties between them.
    for y in prime.take(y*y<=x):
        if(x%y==0):
            break;
        else:
            prime.append(y);
```
Is this algorithm better than the other one.Like in this algorithm,I  don't have to I don't have to exclude 6 more than once,when 6 got divisible by 0,I pass it out.Same goes for 12,
I can do better in the first algorithm.Like after:
1. Cleaning divisor of 2,when faced with 3,I other than subtracting with three,I should substarct with 9 space.When it comes to 5,start substracting with 25.But shouldn't forgot 7 in there.
