![[Pasted image 20250403115820.png]]

the red part is what we are interested in this module.

![[Pasted image 20250403120026.png]]

if you have multiple paths, you can add up the chain rule across all paths.
it's that simple.

see in how lovely way he has shown z as a function of x.

let's formalize this :

![[Pasted image 20250403120308.png]]


how do you read this ?

![[Pasted image 20250403120527.png]]

the partial derivative of the loss function w.r.t. to the j-th element in the i-th hidden layer.

![[Pasted image 20250403120623.png]]

notice how for the above highlighted h-22 , it means it's the second neuron in the second hidden layer.


![[Pasted image 20250403120947.png]]

the k here means k paths which is 2 in the case below,
here the formula is nothing but the summation of the derivatives for each paths individually.

![[Pasted image 20250403121140.png]]

![[Pasted image 20250403121330.png]]

here luckily for this case of h22, the A(i+1)=L which means the last layer, the output layer and we know the derivative of the loss function w.r.t the output layer through the previous module.

however this will not be true for the other generic cases.

but generally it will be something like this :

![[Pasted image 20250403121551.png]]

this can be understood using the example below.

![[Pasted image 20250403121830.png]]

ignore the b33 in the bias addition term that's a mistake 

![[Pasted image 20250403122451.png]]

here in the above calculation, we are calculating the below part of that whole huge formula

![[Pasted image 20250403122525.png]]

because the first part, the loss function wrt to output layer is already something what we know.

this is the derivative of a(i + 1) by h(ij)

![[Pasted image 20250403123008.png]]


![[Pasted image 20250403123143.png]]

here do u see above the underline ?

the . (dot) , j (dot comma j) what does it mean ?
that means all the i that belong to j 
![[Pasted image 20250403123231.png]]
which can be seen through the above example.

![[Pasted image 20250403123406.png]]

now see something amazing, the dot product above mentioned (in the image above circled with red) results in nothing but the formula which we wanted to derive (see down below, the forumula we wanted to derive which is circled in red and the dot product is shown below)

	 just try to visualize the dot product illustrated below in your mind
	 i'm pretty sure you will end up with the formula above !!!!!!
	 isn't this amazing ?

![[Pasted image 20250403123510.png]]

![[Pasted image 20250403123634.png]]

![[Pasted image 20250404101447.png]]

Till now we were assuming for the special case a i+1 = L, but now we need to generalize a bit 

![[Pasted image 20250404101648.png]]

here you can see what the derivative of the activation function (g') looks like
	[[Derivation of the activation function -- g']]

g = sigmoid
as we can say g (a ij) = sigmoid of a-ij

![[Pasted image 20250404101842.png]]

Note --> [[Computing Gradients w.r.t. Parameters (weights)]]