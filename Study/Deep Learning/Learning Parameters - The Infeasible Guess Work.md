![[Pasted image 20250401112023.png]]

W0 =  b (bias) --> just simple nomenclature from now on.

input = critic rating + weight
output = IMDB Rating

![[Pasted image 20250401112117.png]]

*the objective is to minimize the loss function.*

What do you expect at the end of the training stage and you get W* and B* which are the values learnt ?
	We want to find the output value close to the actual value.
	![[Pasted image 20250401112302.png]]

Let's start with the guess work:
![[Pasted image 20250401112412.png]]

we can see that the guess is pretty bad !
but can you tell how ***bad*** it is ?

We have the LOSS FUNCTION !
	![[Pasted image 20250401112529.png]]
	so now we have a *quantitative handle* on how bad it is.

Now let's try something else

![[Pasted image 20250401112645.png]]

We still are doing educated guess work :

![[Pasted image 20250401112748.png]]

Now let's find all the possible values of w and plot it 
![[Pasted image 20250401112908.png]]

blue -- less error (darker shade lesser error)
red --- more error (darker shade more error)

This is fine while we have these two parameters but it becomes intractable when you have more data and parameters.

![[Pasted image 20250401113034.png]]

So, we get it, it is a way of finding algorithms but not a feasible one for sure.

So now we will talk about a method which is neither brute force nor guess work.

Next --> [[Gradient Descent]]
Also Next --> [[Deep Learning/Other Type of Algorithms]]