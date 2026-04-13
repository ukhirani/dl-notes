Enough about Boolean functions !!

we now want to represent arbitrary functions of the form y  = f(x)

![[Pasted image 20250401103259.png]]

can we have a network which can approximately represent such functions ?

before that we have to graduate from *perceptrons to sigmoidal neurons*....

Recalling - a perceptron will fire if the weighted sum of it's input is greater than the threshold (-W0)

0.5

## Sigmoidal Neuron

*The thresholding logic used by a perceptron is very harsh !!!*

you will learn that from the example below,
notice how a slight change in the value of criticsRating changes the overall decision with a small change in the value.

![[Pasted image 20250401103809.png]]

**Characteristic of a Perceptron**

![[Pasted image 20250401104000.png]]

Introducing Sigmoid neuron which is much smoother than the step function.

![[Pasted image 20250401104122.png]]

The logistic function: 
![[Pasted image 20250401104144.png]]

![[Pasted image 20250401104202.png]]

thus when wTx -- infinity ==> 1
		 wTx -- -infinity ==>0

Thus now we no longer see a sharp threshold

![[Pasted image 20250401104431.png]]

![[Pasted image 20250401104445.png]]

Now we need to learn these weights !!

![[Pasted image 20250401104718.png]]

Next --> [[A typical supervised Machine Learning setup]]
Also --> [[Representation Power of a multilayer network of sigmoid neurons.]]