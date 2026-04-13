We want to find a more efficient and principled way of navigating through this weight and parameter finding process

Goal
	![[Pasted image 20250401180926.png]]

let's initialize a vector of parameters:

![[Pasted image 20250401181114.png]]

let's be conservative and move only by a small amount 'n'

![[Pasted image 20250401181152.png]]

![[Pasted image 20250401181209.png]]

![[Pasted image 20250401181538.png]]

The vector in the right most part written in red pen is known as "Gradient" which is essentially a vector consisting the partial derivatives of the two parameters.
 two parameters  = R2 ,three---- R3 ....................n parameters ===> Rn.

similarly, the triangle (delta) highlighted box in red would be of size 2 x 2 as justified below as it is gradient of gradient.

![[Pasted image 20250401184938.png]]

we ignore n now as it is small in value 

![[Pasted image 20250401182253.png]]

now when will u say that the new loss function is better than the old loss function,
when ---vvvvv---

new loss < old loss 
new loss - old loss < 0

thus,

![[Pasted image 20250401182335.png]]

thus, the stuff in the above above equation (n*ut delta L theta) and stuff * should be negative, thus implying..........

![[Pasted image 20250401182513.png]]

that means we are moving in the right direction.

![[Pasted image 20250401182953.png]]

![[Pasted image 20250401183034.png]]

now we have a more principled approach. 

![[Pasted image 20250401183408.png]]

but in this formula what is delta-w t and delta-b t.

![[Pasted image 20250401183604.png]]

![[Pasted image 20250401183900.png]]

now for two points we will get a sum of derivatives.
![[Pasted image 20250401183945.png]]

similarly for b,
![[Pasted image 20250401184027.png]]

algorithm implemented in code:

![[Pasted image 20250401184518.png]]

notice that in the last function do_gradient_descent() the for x,y in zip(x,y) is doing the summation of gradients, nothing else

![[Pasted image 20250401184643.png]]

the plot after running this code. Notice that how it follows the path of the gradient almost like a ball falling through the slope hehe

![[Pasted image 20250401184831.png]]

Next --> [[Feedforward Neural Networks (a.k.a. multilayered network of neurons)]]