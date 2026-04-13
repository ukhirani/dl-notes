![[Pasted image 20250501203534.png]]

if you want to understand the two equations down below 

the first line simply means that with probability q we are setting random bits of input to 0

the second line says that with prob. 1-q we are setting the bits as they are without any change.

![[Pasted image 20250501203814.png]]

![[Pasted image 20250501203847.png]]

this means that the network will not get away by just copying directly the input to the output

![[Pasted image 20250501203957.png]]

it will no longer getaway by memorizing the data

![[Pasted image 20250501204031.png]]

![[Pasted image 20250501204051.png]]

![[Pasted image 20250501204327.png]]

![[Pasted image 20250501204500.png]]

![[Pasted image 20250501204600.png]]

we throw away the last layer and use it as a output layer

![[Pasted image 20250501204755.png]]

![[Pasted image 20250501204813.png]]

![[Pasted image 20250501204930.png]]

![[Pasted image 20250501204945.png]]

![[Pasted image 20250501205102.png]]
![[Pasted image 20250501205204.png]]

each of these boxes are the inputs that causes the k-th neuron to fire

![[Pasted image 20250501205318.png]]

thus more noise will force the nn to find relations from the neighboring inputs also

![[Pasted image 20250501205607.png]]
![[Pasted image 20250501205619.png]]

![[Pasted image 20250501205646.png]]
![[Pasted image 20250501205705.png]]
thus and AE with gaussian noise performs better than weight decay (L2 regularn.) filters


Next --> [[Sparse Autoencoders]]