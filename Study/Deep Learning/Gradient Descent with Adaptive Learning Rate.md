![[Pasted image 20250409075420.png]]

let's say there is a feature that is sparse in nature (majority elements 0)
for ex. isAmirKhanMovie --> then most of the time it will be 0 as he has appeared on very less movies but the feature will be learnt very slowly as it is not that dense.
however we don't want to miss out on identifying all the good patterns, such as isAHitMovie, then yes it mostly will be yes as it's AmirKhan after all. but we don't want to miss out on this features that's the thing.

and we also want that the learning rate take care of itself based on the frequency of the features.

![[Pasted image 20250409075843.png]]

that means if the feature has been updated a fewer times give it a larger rate and if it is updated many times give it a smaller rate.

the learning rate inversely proportional to update history.

![[Pasted image 20250409080021.png]]

![[Pasted image 20250409080136.png]]

![[Pasted image 20250409080253.png]]

this is the plot
- the red is the momentum
- the blue is the NAG
- the black is the GD

can you observe something ? it's almost all 3 didn't know Pythagoras theorem. hehe

![[Pasted image 20250409080420.png]]

![[Pasted image 20250409080545.png]]

now this green is the adagrad one
- now we can observe that the history has accumulated so much and the eta is so small that the line is stuck in the b axis as it has a very small eta.

![[Pasted image 20250409080745.png]]

How can we solve this ?

![[Pasted image 20250409080856.png]]

![[Pasted image 20250409081010.png]]

ok so in this we are multiplying it by some B which is less than 1 prolly and we see that we are not keeping the history that aggressively, rather just a small fraction of that history.

![[Pasted image 20250409081115.png]]

![[Pasted image 20250409081140.png]]

rms prop doesn't increase or decrease the denominator that aggressively.

![[Pasted image 20250409081234.png]]

we know it should look something like this and shouldn't overlap with the data too much as we are not reducing/increasing the weights aggressively, but it's just the problem of the data and not the algorithm. in theory it should look like something above.

ADAM --> [[Adam Optimizer]]