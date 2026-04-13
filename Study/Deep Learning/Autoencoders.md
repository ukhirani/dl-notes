![[Pasted image 20250429130556.png]]
![[Pasted image 20250429130618.png]]
# Similarity between autoencoder and PCA

![[Pasted image 20250429130603.png]]

![[Pasted image 20250429130642.png]]

below is the equation for decoder.

![[Pasted image 20250429130659.png]]

Why are we trying to do this ?

![[Pasted image 20250429130751.png]]

we are able to represent the input layer in smaller dimensions and are able to reconstruct the original inputs at the output layer with minimal loss.

similar to PCA.

![[Pasted image 20250429130907.png]]

do you see any analogy with the PCA ???????????????????????????

![[Pasted image 20250429130927.png]]

![[Pasted image 20250429131027.png]]

![[Pasted image 20250429131045.png]]

copy input in first n out of d bits and then leave remaining empty

![[Pasted image 20250429131106.png]]

![[Pasted image 20250429131111.png]]

let's see a case where this might be actually useful as an autoencoder.

![[Pasted image 20250429131226.png]]

BMI is a function of (height and weight) and let's say in any case of casualty, we want to find out whether it was due to the height or the weight, then this might provide a way but it's still useless as we can directly copy the BMI in the first n bits out of d bits. 

![[Pasted image 20250429131448.png]]

let's start with the choice of f(x) and g(x)

# Choice of F(x) and G(x)

## for binary inputs

first let's consider the case where the inputs are binary.

![[Pasted image 20250429131524.png]]

this means the output also means binary

![[Pasted image 20250429131552.png]]

![[Pasted image 20250429131559.png]]

![[Pasted image 20250429131618.png]]

## for real inputs 

![[Pasted image 20250429131726.png]]

linear function is better

![[Pasted image 20250429131740.png]]

g is typically seen as the sigmoid function



# Choice of Loss Function

## for real inputs

squared error is the best

![[Pasted image 20250429131936.png]]

![[Pasted image 20250429132006.png]]

which would look like this when opened up in matrix form 

![[Pasted image 20250429132040.png]]

![[Pasted image 20250429132058.png]]

# Backpropagation in Autoencoders

![[Pasted image 20250429132246.png]]

but previously we had entropy as a loss function due to the probability distribution but now we have squared error loss function. so all that we study went in vain ?????

no.

![[Pasted image 20250429132359.png]]
![[Pasted image 20250429132520.png]]

the part where arrow is pointing is the only part that we need to recompute, else will remain the same.

![[Pasted image 20250429145246.png]]
![[Pasted image 20250429145327.png]]

## binary inputs

![[Pasted image 20250429145549.png]]

we look at the cross entropy loss because it works better in our case,

![[Pasted image 20250429145649.png]]

![[Pasted image 20250429145806.png]]

![[Pasted image 20250429145926.png]]

instead of writing p and q let's write p and 1 - p and in that format you can see the formula was written such as Xij log q + (1-Xij)log(1-q).

![[Pasted image 20250429150421.png]]

![[Pasted image 20250429150624.png]]

when will the above value be minimized
when xij = x^ ij (x-hat ij) =1 or =0

it's value will be minimum = 0 

 ![[Pasted image 20250429150753.png]]

![[Pasted image 20250429151132.png]]

![[Pasted image 20250429150906.png]]

![[Pasted image 20250429151051.png]]


[[Link Between PCA and Autoencoders]]