![[Pasted image 20250502104715.png]]

Let us consider this example of sine wave (the true f(x))

![[Pasted image 20250312072249.png]]

For now we will behave that we don't know the true f(x), rather we will try to predict it and in the process we will learn the bias variance tradeoff.

![[Pasted image 20250312072743.png]]

y = f^ x (f hat of x)

We will consider two models.

![[Pasted image 20250312072453.png]]

![[Pasted image 20250312072609.png]]

Simple line that can be said as an output of linear regression which is trying to minimize the mean squared error simply.

![[Pasted image 20250312072647.png]]

![[Pasted image 20250312072658.png]]

![[Pasted image 20250502104857.png]]

Now what we do is that 

![[Pasted image 20250312072917.png]]

Now we plot all the sample lines and curves

![[Pasted image 20250312073002.png]]

However they are very far from the true sinusoidal curve.

![[Pasted image 20250312073318.png]]

And more complex models tend to overfit.

Now let's understand what **Bias** and **Variance** are :

![[Pasted image 20250312073448.png]]

# **BIAS**

![[Pasted image 20250312073510.png]]

It tells you how much does this expected value (the average of all possible lines (the green one in the figure below.) and plots taken from the random samples) differ from the true function.

![[Pasted image 20250312073630.png]]

![[Pasted image 20250502105154.png]]

The green line here shows the average value of all possible lines of the simple lines that we drew earlier.

![[Pasted image 20250502105214.png]]

This is show that the bias is **very high**.

However for the blue curve that is the average of all the complex plots, the bias is **very low**.

That mathematically implies that,

> *A simple model has high bias whereas a more complex model would have a low bias.*


# **VARIANCE**

![[Pasted image 20250312074034.png]]

*Variance tells me the spread.*

![[Pasted image 20250312074043.png]]

function - average of that functions

It tells me how each line are different from the average f(x).

![[Pasted image 20250502105305.png]]

> *Simple models have a low variance whereas complex models have a high variance.*

![[Pasted image 20250502105331.png]]

# Mathematical Reasoning behind it 

[[Train Error VS Test Error]]



