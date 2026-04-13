What about non-boolean (say,real) inputs ?????
Do we always need to hand code the threshold ?????
Are all inputs equal ? What if we want to assign more weight (importance) to some inputs ?????
What about functions which are not linearly seperable ?????

# Perceptron

![[Pasted image 20250311113518.png]]

- Frank Rosenblatt - proposed the **classical perceptron** model.
- Introduction of numerical weights for inputs and a *mechanism for learning these weights.*
- Inputs are no longer limited to boolean values.


# How it works ?

![[Pasted image 20250311113840.png]]

**Now one more change !!! 

*Notice the change in the value of the range of i in the photo above and below. 

![[Pasted image 20250311113941.png]]

Instead of 1 to n it is 0 to n and also the theta has disappeared, indicating that **the theta is considered a weight a.k.a W0 and X0 is 1.**

![[Pasted image 20250311114103.png]]

Updated perceptron model :

![[Pasted image 20250311114121.png]]

# Why do we need weights ???

![[Pasted image 20250311114436.png]]

![[Pasted image 20250311114759.png]]

*Notice here that more the theta the more it will increase the threshold here to fire up the neuron*
If you are an avid movie watcher, then you will have less opposition to watch any move in this case (indicating ideal theta = 0 or close to that), but if you are very selective movie watcher then the value of theta will be higher indicating a higher threshold which means that you have somewhat of a higher opposition to watch the movie irrespective of the movie being offered.

# **What kind of functions can be implemented using perceptrons ?** *Any difference from MP neurons* ?

![[Pasted image 20250311114942.png]]

![[Pasted image 20250311115316.png]]

We get a set of linear equalities, thus opening a door for many other possibilities.

![[Pasted image 20250311115426.png]]

You can come up with the same thing with MP neuron by deciding the value of theta...
# Error and Error Surfaces

![[Pasted image 20250311122037.png]]

We want values of "W" such that we minimize errors or in best case 0.

**Error Surfaces 

![[Pasted image 20250311122251.png]]
Just a 3D plot of w1 w2 with the error

See Next -> [[Perceptron Learning Algorithm]]
But what about [[What about the Functions that are not linearly separable...]]
