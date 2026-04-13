
![[Pasted image 20250408125846.png]]

![[Pasted image 20250408130008.png]]

![[Pasted image 20250408130111.png]]

![[Pasted image 20250408130229.png]]

do you see these oscillations in vanilla gradient descent algo, this is because of the greedy nature where you are  looking for the individual point's update and profit rather than the dataset or the other points as a whole.

can we reduce these by improving our stochastic estimates of the gradient,(currently estimated from just 1 data point at the time.)

![[Pasted image 20250408130907.png]]

![[Pasted image 20250408131012.png]]

mini batch = smaller size of the whole dataset
batch gradient = the whole dataset.

![[Pasted image 20250408131209.png]]

![[Pasted image 20250408131737.png]]

![[Pasted image 20250408131754.png]]

 ![[Pasted image 20250408132036.png]]

the NAG is blue and the momentum is red (there is a printing mistake in the image down below) as NAG takes shorter u turns.

![[Pasted image 20250408132147.png]]

Next --> [[Deep Learning/Tips for adjusting the learning rate and momentum.]]