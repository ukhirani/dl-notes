![[Pasted image 20250401104958.png]]

What do we mean by "cannot deal with " ?
look in the slide above

Now to the most important slide in the course
![[Pasted image 20250401105259.png]]

We agree that there exists *some relation between the input and the output*. We all know that there is a function that represents it which is y = f(x).

But we don't know that function, if we knew it we wouldn't be finding it in the first place,
so we take an assumption 

y = f^(x,w)  ---> assumption

now we want to predict the values of these parameters.

![[Pasted image 20250401105714.png]]

*now what is wrong with the logistic equation ?(that equation which is written in red)*
**ANS.** is that *we have nothing to learn,* we can plug in any values irrespective of the data and we will get an answer which is very much prone to errors as we haven't adjusted the formula according to the data.


Once we have these *W* in all the three formulas written in black, we have these parametric form of the equation in which we can learn these parameters.

![[Pasted image 20250401110016.png]]

![[Pasted image 20250401110037.png]]

Learning is driven by ???

![[Pasted image 20250401110225.png]]

For example,
![[Pasted image 20250401110428.png]]

Why do we use squared difference?
	 1. Differentiable ✔️ 
	 2.  Positive errors and negative errors should not cancel out each other.

The learning error should aim to find a *w* which minimizes the above function.

Next --> [[Learning Parameters - The Infeasible Guess Work]]