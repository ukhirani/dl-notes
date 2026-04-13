#deeplearning 
A more principled approach of learning the weights.....

![[Pasted image 20250311132133.png]]

**Algorithm**

P -> inputs with label 1
N -> inputs with label 0

Initialize w = {w1,w2.....wn} randomly

Algo Starts !!  --->

while ! [[Convergence]] do
![[Pasted image 20250311132742.png]]

Now instead of writing the summation we represent it in vector form and which essentially means we are taking the dot product and that determines the decision boundary

![[Pasted image 20250311133142.png]]

The vector will be perpendicular to the line of the decision boundary (W^T X = 0) as the dot product is zero

![[Pasted image 20250311133550.png]]

points in w^t x >=0 will make less than 90. with w and inverse for the other case.

![[Pasted image 20250311133855.png]]

Now revisiting the perceptron learning algorithm.

![[Pasted image 20250311134217.png]]

This is for P (where angle should be less than 90* but it is greater than 90* which should not be happening)

thus alpha-new < alpha-old
thus what we are essentially doing is that we are slowly moving the angle from greater than 90degrees to less than 90degrees.
this will keep doing this till it reaches convergence.

**Now let's see the algorithm in action**

![[Pasted image 20250311135004.png]]

after picking *p1* as the random point here's the correction in the w that happens after one iteration

w = w + x (also notice that the angle became smaller than before implying we are trying to make it less than 90* when we reach convergence)

![[Pasted image 20250311135042.png]]

now after picking up p2 (w = w + x  and also the angle becomes somewhat smaller again)

![[Pasted image 20250311135211.png]]

Now we pick the point n1 (w = w-x  angle becomes greater )

![[Pasted image 20250311135345.png]]

now we pick p3 (w = w+x)

![[Pasted image 20250311135409.png]]

now by definition my algorithm has converged.

**Now are there any problems ????**
**Will it always converge ????**

To know more [[Proof of Convergence]]
