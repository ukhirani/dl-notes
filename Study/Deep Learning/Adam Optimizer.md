now we have RMSProp based on the frequency of features, and also momentum based approach based on the slope of the error surface.

so why not combine them both ?

![[Pasted image 20250409081619.png]]

the Mt part is the momentum part and the Vt part is the adagrad/RMSprop part.

	 (Adam = Adaptive Moments)

Mt is the exponentially weighted mean (first moment)
Vt is the exponentially weighted second moment (second moment)

we come up with the first moment and the second moment to come up with an adaptive learning rate.

![[Pasted image 20250409082238.png]]

![[Pasted image 20250409082548.png]]

![[Pasted image 20250409083113.png]]

this is later continued in  --> [[Deep Learning/Bias Correction in Adam]]


