suppose i have an ern of balls with colors red blue and white and for example this is the true probability distribution given 
![[Pasted image 20250404190421.png]]

and suppose one of my friend is just allowed to take a peep in the ern and just guess the prob. distribution of the ern. let's say he predicted this distribution (q)

![[Pasted image 20250404190555.png]]

how to find the loss or the mistake 

you can take the squared error........

![[Pasted image 20250404190643.png]]


here we are ignoring the fact that this is not a normal vector distribution, rather it's a probabilistic distribution.
now we want a more principled and a better way of computing the error of the predicted distribution vs the actual distribution.

let's say some teams of cricket entered a tournament finals and stuff and the final happened and team B won : here is what would the prob. distr. would look like :

![[Pasted image 20250404191025.png]]

here all the mass is focused on the event of prob. B occurring.

but if i watched till the semi finals and i had to predict which team would have won, then this is what i would have guessed in the first place 

![[Pasted image 20250404191248.png]]

these are the numbers/prob. which i assigned

a simple way to calculate how wrong i was would be to calculate the squared errors:

and the loss function is some notion of difference between p and q

![[Pasted image 20250404192110.png]]

now let's again revisit the topic of expectations.

there is a prob. and gain/profit for each random variable.
here's how you will calculate the expectation value.

![[Pasted image 20250404192449.png]]

***what is information content ?***

for ex. if you tell me my name is umang, then information gain is too low but if you tell me that today i'm going to get struck by lightning (strike me down zeus, you don't have the ba..............), the information gain is really high.

so low probability means high information gain. (inversely proportional)

![[Pasted image 20250404192752.png]]

here we are just vaguely describing the relation, now we want a function that gives us the same relation with the input and the output.

let's consider X and Y (2 independent events) 
![[Pasted image 20250404193015.png]]

and i come and tell you something about x and y (what is the information content gained from this) = IC-X + IC-Y

![[Pasted image 20250404193200.png]]

so this is what the function should satisfy basically,

since the two events X and Y are independent, we can write the joint prob. as P(x) X P(y).

![[Pasted image 20250404193230.png]]

and what family of functions do we know that can satisfy this ?
log .......... right ???
yeah but we want it to be inversely proportional

so log(1/P(A)) = - (log(P(A)))

![[Pasted image 20250404193431.png]]

P(A) means P(X=A) ............ hehe

![[Pasted image 20250404193719.png]]

how do i now calculate the entropy of the whole distr.

![[Pasted image 20250404193746.png]]

this is basically the mathematical expectation of the prob. and the information content that we just calculated.

and the total entropy is going to be 0.

so this was entropy, now we want to know something known as cross entropy 
NEXT ---> [[Deep Learning/Cross Entropy]]