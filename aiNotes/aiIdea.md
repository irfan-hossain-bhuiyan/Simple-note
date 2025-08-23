#### Bidierectional Gradient
1. As the bidirectional gradient ,when there is a low and high,the gradient of high and low cancel each other out,So The ball will roll down in down surface,And try to go in the surface where there is more down than up,I don't know If there is should be something like this?Have to graph this finding.

This function shouldn't work,But it works really graet.

2. Try to change the bidirectional gradient to if it is flat from 1 to sigmoid function for getting distance information.

3. Other than constantly checking for future derivative ,Just check the direction it have to go then add them up.(This is a bad idea,With no mathematical strcuture.)

4. Because in a flat plane it will try to go in the direction,that has
more down hill than uphill in infinite,In my guess,that type of value should be 0,but I have to see it later.

5. Always go through the tilted floor,When got stuck permanently,Use bidirectional gradient to fix your point on where to go?

### Some general ideas.
6. Make use of as much as non linear function as possible?
7. Non Linear function(acitvation function) that works on entire vector than,each of the element works better?That's why attention mechanism works amazing.
8. Check if I can add new neuron in the layer,If needed.
9. I want a sleeping setup,I wanna know if a neuron is more active than other?If true that neuron will g    row,and if some is not active,It will shrink

### Making a AGI
1. When training a neural network in agi,I can't just train like doing a cost 
function to predict a value.
2. What can I do is doing random thing and predicting what will happen in ai?
3. How do I train an ai,So It understand game by itself?other than giving it hints the small step it need to take.


### some test to generalize ai
1. I can make ai to train xor,As the training will be simple,
    What I wll do is remove a lot of xor from the test,Like all the test case will have certain bit only 0,and certian bit only 1,in all test cases,Then in testing phase I will check if the model generalize itself,if not,What wil be a better training?

### Sleep
1. Every animal sleep,having better brain,ai shouldsleep too?
2. We have dream,So there are some simulating process there?I think ai need that too.
3. Transformer model is some what like a specialized model?like In simplified mdeol each layer is a 
    function ,that got passed to another function,But in transformer where the output  should be passed is decided by key and query vector

### Partial Linear FUnction
1. Understanding nonlinear function,how it behaves with linear function,is needed.
I have made a mathematical object that <m0,m1> which is equivalent to f(x)=m0x if x<0,else m1x,
Now this mathematical object is associative like (<m0,m1>.<m2,m3>).<m4,m5>=<m0,m1>.(<m2,m3>.<m4,m5>),
I need to test how this math operation evolve in high dimension?Interect with matrix
I know the function don't work good with addition,like <m0,m1>(a+b),
it won't distribute like <m0,m1>a+<m0,m1>b,is there a way to split it ,Can I just make the addition operation a part of higher matrix multiplication.

### Generating data for classification neural network
1. My brain can easily detect if a english word is valid,
but when I try to write those words,my brain get confused,
on that scenerio,I try to generate a word,most likely not the valid words,
try to tweak the word in some way to find the valid word.
2. We can do it to neural network as well,like in mnist data recognition neural network,
in input we can take a random sample,then use packpropagation,and say the cost function is having the value being 2,which it is not as the input is randomized,So when backpropagation,we won't update the weight,we will update the input value,update in a way to minimize the cost function,to generate image,there is a high chance the image we will get is just noise,
with a high probability of it being 2 in the network.So we need to train the network to reduce 
training this garbage value.
One way to do is having extra classification neural network,that is trained to detect garbage value,
So we will also train the neural network inputting the garbage value(random varaible) and detecting it as garbage value
A way to do it is several neural network with different initialized weight,So they train differently,
one will think it is real,other will detect it as garbage,

But there is a lot of neural network,to train,A easy way is to just train several neural network,that 
detects garbage value versus the non garbage one.


