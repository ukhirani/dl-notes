what if in the first place we blew up the eta (n) in the first place so for each iteration we would have large jumps, thus having a higher learning rate.

![[Pasted image 20250408214731.png]]

so now we see that the fixed value of eta isn't really helping us so now we see the need for an adaptive learning rate which increases in value for gentle curves and decreases in value for steeper curves.

![[Pasted image 20250408214944.png]]

![[Pasted image 20250408215145.png]]

the intuition behind this ?
	 when you are done after 5 epochs you are somewhat close to the minima so slow down and reduce the learning rate by half after every 5 epochs.

![[Pasted image 20250408215244.png]]

run epoch t and and also run epoch t+1
if the the loss function value increases from t -> t+1 then discard all the calculations and then again run epoch t 

![[Pasted image 20250408223402.png]]

this exponential decay means with more and more iterations we are decreasing eta exponentially
t = is another hyper parameter that we are introducing which means after every epoch or something like that we are halving or doing something to the eta value.

![[Pasted image 20250408223601.png]]

![[Pasted image 20250408224307.png]]

Next --> [[Deep Learning/Line Search]]