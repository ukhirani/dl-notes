
it takes a lot of time to navigate regions having a gentle slope in gradient descent.
this is because the gradient in these regions is very small.

yes 

![[Pasted image 20250408122751.png]]

![[Pasted image 20250408122946.png]]

![[Pasted image 20250408123115.png]]

its an exponential weighted average
my maximum fate lies on the current guy who told me the direction , lesser in previous and even lesser in previous to previous.

![[Pasted image 20250408123217.png]]

![[Pasted image 20250408123343.png]]

pseudo code of gradient descent

![[Pasted image 20250408123458.png]]
 the output after 15-20 steps
but is moving fast always really good ?

![[Pasted image 20250408123550.png]]

can momentum be detrimental in this below case ?

![[Pasted image 20250408123653.png]]

![[Pasted image 20250408123849.png]]

as you can see there are a lot of oscillations around the minima of the valley both in the image above and below.

![[Pasted image 20250408124229.png]]

visualization of the algorithm actually learning the function we desire.

can we do something to reduce these oscillations ??

next--> [[Deep Learning/Nesterov Accelerated Gradient Descent]]