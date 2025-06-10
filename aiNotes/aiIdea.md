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
