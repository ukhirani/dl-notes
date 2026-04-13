For this discussion,
	True = +1 
	False = -1

Also
	 Red edge indicates w = -1
	 Blue edge indicates w = +1

![[Pasted image 20250313210118.png]]

Here it in the base level it means that each perceptron (having bias -2) means that it will fire up if the weighted sum of all >=2.

This network contains 3 layers.
	 The input layer (x1,x2)
	 The hidden layer (containing the 4 perceptrons)
	 The output layer (a.k.a. the final layer)

*We claim that this network can be used to implement any Boolean function* (linearly separable or not) !!, *well not really if you understand what is going on*
Each perceptron in the middle layer fires only for a specific input (and no two perceptrons fire for the same input)

![[Pasted image 20250401095450.png]]

![[Pasted image 20250313210817.png]]

Look for the first line in the above photo, you can see that the weighted sum should be greater than or equal to W0 if we want to fire the neuron, so don't get all worried up seeing the last line in the photo above.
It's just putting the value of the weights attained on each step to satisfy the condition we just talked about.

![[Pasted image 20250313210853.png]]

We have made sure that every neuron in the middle layer caters to one specific input, that's why these weights don't interfere with each other.

## What if we have more than 3 inputs ?

![[Pasted image 20250401095855.png]]

## What if we have "n" inputs ?

2^n perceptrons in the hidden layer

![[Pasted image 20250401100230.png]]

Give me any input and i will give you one NN which will fit the data when it converges 
![[Pasted image 20250401100507.png]]

![[Pasted image 20250401100519.png]]

The last line is the core of this topic.

Next -> [[Sigmoid Neuron]]