The choice of the loss function depends closely on the problem at hand (the special O function at the end)

Let's learn with Examples

![[Pasted image 20250402081138.png]]

![[Pasted image 20250402081409.png]]

Why not use the aggregation function with weights as a linear function ?

Why will the output function be bounded to a limit even though it isn't by definition ?
	 Because we are minimizing loss and will penalize those values greater than the bound.

If I took a guess then how wrong would I be ?

![[Pasted image 20250402082436.png]]

talking about entropy, before that , expectation = reward x prob for each event 

![[Pasted image 20250402082557.png]]
![[Pasted image 20250402082609.png]]

But more the probability, less the information content and vice versa 

![[Pasted image 20250402082712.png]]

And now the cross entropy would be something like this :

p = actual prob. distribution
q =  predicted prob. distribution

![[Pasted image 20250402083113.png]]

the cross entropy is the formula at the last
when would this be minimized --- when both are same 

so cross entropy will tell you how close a predicted distribution will be to the actual distribution.

![[Pasted image 20250402083412.png]]

here the prob. distribution means that it's sum should be bounded by 1.

can we use the sigmoid function ?
	 no because the sum would be greater than 1 in many case which is not valid for a prob. distribution as summation of all probabilities should be equal to 1.

Then what do we use ?

**SOFTMAX FUNCTION**

![[Pasted image 20250402083639.png]]

![[Pasted image 20250402083732.png]]

Here, if you observe that even for negative values say -10 the output will be e^-10
which will be a positive value. that's why we don't directly take -10/-10 + 20 + 30 , rather take the exponential of each value and then add it up.

This is why we need the softmax function.

What will we take as the objective function ??

**Cross entropy** again !

![[Pasted image 20250402084840.png]]

![[Pasted image 20250402085024.png]]


![[Pasted image 20250402085242.png]]

![[Pasted image 20250402085309.png]]


Next --> [[Backpropagation]]