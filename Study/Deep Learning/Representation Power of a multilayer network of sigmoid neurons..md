![[Pasted image 20250401190515.png]]

This proof is known as the universal approximation theorem.

![[Pasted image 20250401190826.png]]

![[Pasted image 20250401190834.png]]

![[Pasted image 20250401190841.png]]

we can make it arbitrarily close to the value.

![[Pasted image 20250401190951.png]]

the more the tower functions, the better the approximation.

![[Pasted image 20250401191203.png]]

Our job is now to figure out is inside the blackbox tower maker.

![[Pasted image 20250401191443.png]]

ok so another 2 observations, as we increase w it becomes and comes more and more closer to a step function. and you increase b more and more it offsets more from the y axis or you can say move in the x axis.

so the point where we get that half value is :

![[Pasted image 20250401191635.png]]

![[Pasted image 20250401191742.png]]

here's how we get a tower function.

## Can we come up with a neural network that can to represent this operation of subtracting one sigmoid function from another ??

![[Pasted image 20250401191955.png]]

this will get you one tower:

![[Pasted image 20250401192217.png]]

what about 2 data

![[Pasted image 20250401192444.png]]

**note that here w2 = 0 , that's why it is not changing in that axis.**

what if we increase w1 and b

![[Pasted image 20250401192601.png]]

to make towers, what do i need to do ?
![[Pasted image 20250401192637.png]]

but will you live in this tower ?? no because it is open from two sides but to close it from there too , what will we do ? 
*ans* . make w1 = 0

now what will happen if we add both those tower functions ?

![[Pasted image 20250401192813.png]]

how to threshold these red values ?

![[Pasted image 20250401193026.png]]

so any values less than 1 we do something and for more than 1 we do something, what is this something , lets learn...

![[Pasted image 20250401193145.png]]

we use a steep sigmoid neuron to pass it through as we cannot use a neuron.

## Can we come up with a neural network to represent this entire procedure of constructing a 3 dimensional tower ?

![[Pasted image 20250401193432.png]]

this is just one block , we will have an aggregator on top of these to add them.

![[Pasted image 20250401193853.png]]
![[Pasted image 20250401194037.png]]

![[Pasted image 20250401194153.png]]

