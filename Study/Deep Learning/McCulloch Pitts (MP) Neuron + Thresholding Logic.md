![[Pasted image 20250311110905.png]]

These both scientists proposed Highly simplified computational model to simulate how we think the brain works.

This will take a lot of inputs (binary) -> artificial neuron -> function (decides whether to fire the neuron or not)

Ex.
Whether I should watch a movie or not ?

The inputs can be excitatory or inhibitory.

Ex. Am I Ill today ?

**Inhibitory** - if this input is on the output is always going to be off, the neuron is not going to fire
**Excitatory** - But it combined with all the other neurons can fire the neuron.

![[Pasted image 20250311111413.png]]

Theta is called the thresholding parameter, and this is called the thresholding logic.


# Implementing Boolean Functions using MP Neuron
 ![[Pasted image 20250311111636.png]]

**Using Inhibitory input**

![[Pasted image 20250311111704.png]]

![[Pasted image 20250311111744.png]]

The highlighted circle shows the inhibitory input in the diagram above
The threshold for the above is **1**

![[Pasted image 20250311112043.png]]
Threshold for the above is **0**.

![[Pasted image 20250311112111.png]]
Threshold for the above is **0**.

# Can any boolean function be represented using MP unit ?

**Let's take the geometrical representation of an MP unit :**
![[Pasted image 20250311112435.png]]

This represents an equation of a line.

![[Pasted image 20250311112550.png]]

A single MP neuron splits the input points into two halves using a linear decision boundary.

**Some more example/s**

![[Pasted image 20250311112718.png]]![[Pasted image 20250311112747.png]]

**What if we have more than 2 inputs :**

****Instead of a** ***line we will have a plane***, for further higher dimensions we will have a hyperplane dividing the space into positive and negative.

![[Pasted image 20250311112902.png]]

**Moral of the story :**
A single MP neuron can be used to represent boolean functions which are linearly seperable.

****


Next -> [[Perceptron]]