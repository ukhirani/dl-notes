Why regularization --> to prevent overfitting and improve generalization.

This happens as when we are training, we are just trying to solve one optimization problem that is to minimize the training error and this may lead to overfitting due to large number parameters.

this means that it can happen in over-complete autoencoders (can happens in under-complete autoencoders)

![[Pasted image 20250501202550.png]]
![[Pasted image 20250501202612.png]]

we are not allowing our weights to grow by this means.
this simply means we are not allowing the error in loss function to reach 0, thus preventing overfitting to the training data.

![[Pasted image 20250501203023.png]]

![[Pasted image 20250501202926.png]]

also it's very easy to update the update rule in gradient descent

![[Pasted image 20250501203107.png]]

now we are telling that for decoding i wont give u another pair of w(w*) instead you have to learn w in such a way that wT (w-transpose) becomes the decoder weights

thus reducing the number of parameters used (by half)

 
