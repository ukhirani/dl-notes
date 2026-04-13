what it does is that one each step (irrespective of vanilla/momentum gradient descent) we use a bunch of learning rates (say 5 of them)

## Algorithm

then on each iteration you will get 5 values of w,b and plugin each value in the error function and the one which is minimum is kept.
retain that w,b value and repeat

![[Pasted image 20250409073804.png]]

you see in the array, for steeper curves it will take value around 0.1 and for more gentle curves it will take around 10.0 or some value close to it which is in the array.

![[Pasted image 20250409073852.png]]

What's the flipside ?

![[Pasted image 20250409073955.png]]

![[Pasted image 20250409074215.png]]

we hardly see any oscillations in this case, but that all depends on the set (array) of the learning rates that you have taken.
for example. if on a steep curve the rate required is 0.01 but in your set every value is larger than 0.01 then the curve will overshoot and lead to oscillations.
thus choosing a good set of learning rates need to be essential.

Now let's move to some standard and more use approaches in the recent times in every research paper that you could see...........

Next --> [[Deep Learning/Gradient Descent with Adaptive Learning Rate]]