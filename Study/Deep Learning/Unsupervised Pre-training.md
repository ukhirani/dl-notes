![[Pasted image 20250502164035.png]]

![[Pasted image 20250502170207.png]]

![[Pasted image 20250502170347.png]]

we try to reconstruct x from h1 (similar to what we did in [[Autoencoders]])

now for each layer we are obtaining an abstract representation of the previous layer and thus increasing the abstraction layer by layer.

and we repeat the same thing trying to reconstruct h1 using h2 

![[Pasted image 20250502170935.png]]

![[Pasted image 20250502171320.png]]

and now we add the output layer and now we fine tune the weights of the whole model 
AND THIS WORKS .... WAIT ??
we told that training deep neural networks using only [[Backpropagation]] didn't work so how will this work ??

![[Pasted image 20250502171331.png]]

![[Pasted image 20250502171441.png]]

## Is it because of better optimization ??

![[Pasted image 20250502171546.png]]

![[Pasted image 20250502171616.png]]

if the last layer has a very high capacity, then it will drive the training loss to zero even if you don't do unsupervised pre training.

![[Pasted image 20250502171731.png]]


## Is it because of better regularization ??

![[Pasted image 20250502171846.png]]

so we can see that with pre training the same constraining nature is observed.

and this means we are doing the same thing as backpropagation but we are initializing from a better space and hence just fine tuning

![[Pasted image 20250502173645.png]]

and in-fact it's a better approach

![[Pasted image 20250502173741.png]]

![[Pasted image 20250502173915.png]]

this led to all the methods and advancement that we now know such as [[Dropout]] and [[Adam Optimizer]] and all such methods.

sadly [[Unsupervised Pre-training]] is not used anymore 

![[Pasted image 20250502174048.png]]

