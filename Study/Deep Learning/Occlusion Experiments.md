![[Pasted image 20250521203737.png]]

how would we know which factor actually resulted in this decision.

![[Pasted image 20250521203847.png]]

now i make an occlusion of a patch in this image and do that for all the possible patches and see what is actually causing the answer to be affected the most.

![[Pasted image 20250521203935.png]]

and we create a heatmap which shows the the effect in the output prob. if you drop that patch
blue means more significant and red means less significant.

![[Pasted image 20250521204049.png]]

this is a weakness as if you cover some certain patch then the model is heavily relying on that feature to decide that class and so to make it more robust to noise and such occlusions, we need to learn in such a way that we are now prone to such cases.

![[Pasted image 20250521204309.png]]

