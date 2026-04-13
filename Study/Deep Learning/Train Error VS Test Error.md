Consider a new point (x,y) which was not seen during training

![[Pasted image 20250312083417.png]]![[Pasted image 20250312083543.png]]
We want a sweet spot where bias is not very high and also variance is not very high, you want something in between.

![[Pasted image 20250312083809.png]]

These both errors typically exhibit a trend shown in the figure down below :

![[Pasted image 20250312083948.png]]

**How do we achieve this sweet spot (the ideal spot) ?????**
**Ans.** Regularization

![[Pasted image 20250312084109.png]]

Relation b/w train error and model complexity

![[Pasted image 20250312084207.png]]

We always tend to minimize and target train error while we should focus on the validation error to see that you are not overfitting on the training.

![[Pasted image 20250312084341.png]]

![[Pasted image 20250312084412.png]]

![[Pasted image 20250312084500.png]]

On average the noise is going to be 0.

![[Pasted image 20250312084907.png]]
 
 but we cannot estimate directly because we don't know the relation f .
 ![[Pasted image 20250312085016.png]]

But here is something you can estimate. (not really)
Empirical Estimate................

![[Pasted image 20250312085330.png]]

Quantity of interest (LHS) = RHS (which can now be computed)

*E* -> means true expectations

**Empirical Estimations**

![[Pasted image 20250312090128.png]]

Taking the same analogy :

![[Pasted image 20250312090140.png]]

Now we will replace all the *E*'s with the summation formula we have going on above

![[Pasted image 20250312095243.png]]
![[Pasted image 20250312095345.png]]

That's why the training error seems to be very optimistic as we have ignored the third term  which is the  + 2*E*..... term.
# **But how is all this even related to Model Complexity ?**

![[Pasted image 20250312204250.png]]

![[Pasted image 20250312204455.png]]

Answer :

![[Pasted image 20250312204524.png]]

Notice the change in the line in simple and complex model in the diagram down below :

![[Pasted image 20250312204627.png]]

![[Pasted image 20250312204726.png]]

The base of all regularization methods :

![[Pasted image 20250312204833.png]]

# Why do we care about the [[Bias and Variance Tradeoff]] in terms of Deep Learning ?

![[Pasted image 20250312205053.png]]

Let's start with [[L2 Regularization]]
