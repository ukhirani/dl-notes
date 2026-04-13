there is something which is the true distribution (P) and there is something which is the predicted distribution (Q).

let's say we are transmitting a message of prob. distr. (total size = 4) and each prob. is denoted by 2 bits as shown down below :

![[Pasted image 20250404194433.png]]

now what is the information content for each prob.

![[Pasted image 20250404194453.png]]

answer = 2 
so the information content is acutally the no. of bits you are using to transmit the message.

this holds true even for other no. of prob. distr. lengths (say 8)

![[Pasted image 20250404194606.png]]

answer = 3
holds true...

told ya !

what if we want to transmit over a long distance and make this more efficient... ?

![[Pasted image 20250404194900.png]]

this is a more efficient approach

now let's consider the case where we are predicting these message values (prob. distr. q )

![[Pasted image 20250404195230.png]]

the entropy would be -log(Qi)

do you see a problem with this
	 this is my prediction but the actual distribution is P 

![[Pasted image 20250404195358.png]]

now if i wanted to compute the expectation how would i do it ???

i'll have to use P because that's the true distribution from which the data is coming.

![[Pasted image 20250404195454.png]]

so this what the actual distribution would look like.


this quantity is known as the **cross entropy.**

***why is this the difference between two distributions which we previously wanted ?***
	 what is the property you would want this distribution to have ?
	 - if p = q ------ then ?-------> it should take the lowest possible value 
	 ![[Pasted image 20250404200000.png]]
	

**why (min. value of loss function is at p = q)?** see the proof down below !

what do we do if we want to find the min. value of a function say (x square --> x^2), then we differentiate it wrt to x and put value = 0.

![[Pasted image 20250404200515.png]]

![[Pasted image 20250404200537.png]]

this is using the le-grangian multiplier

![[Pasted image 20250404200737.png]]

if this condition satisfies, then the value of this above listed part will be 0 thus will minimize the overall loss function equation, otherwise will add some non negative part to the loss function, keeping it away from the minimum value.

![[Pasted image 20250404201018.png]]

so this cross entropy term will be minimized when your predicted distribution is same as the true distribution which captures the difference between the two.
so no difference = min. cross entropy

![[Pasted image 20250404201259.png]]

so the loss function is the cross entropy.





