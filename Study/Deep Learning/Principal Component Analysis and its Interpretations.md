![[Pasted image 20250410102434.png]]

![[Pasted image 20250410102517.png]]

![[Pasted image 20250410102648.png]]

now we are reducing the dimensions from R2 to R1 by reducing the dimensions from 2 to 1 and removing a redundant dimension

![[Pasted image 20250410103329.png]]

 ![[Pasted image 20250410104307.png]]

is that all we want from PCA ? reducing dimensions

![[Pasted image 20250410104418.png]]

you see in the above example we can see that the y and z columns are highly related.

![[Pasted image 20250410104821.png]]

![[Pasted image 20250410105032.png]]

![[Pasted image 20250410105308.png]]

![[Pasted image 20250410105404.png]]

![[Pasted image 20250410105647.png]]

![[Pasted image 20250410110118.png]]

![[Pasted image 20250410110125.png]]

here the 1TX is going to be zero as similar to above relation each element will be the column sum and since the matrix given to us is mean zero we will have sum = 0 

![[Pasted image 20250410110238.png]]

![[Pasted image 20250410110411.png]]

![[Pasted image 20250410110552.png]]

![[Pasted image 20250410110610.png]]

 so in the second line it boils down to the dot product of the ith column and the jth column as we are finding the covariance between the column i and column j 
 
![[Pasted image 20250410110852.png]]

![[Pasted image 20250410110958.png]]

this is the ideal case as we we want for i = j the covariance !=0 and when i != j the covariance = 0 as we want no correlation between the now reduced dimensions.

variance should be high, the covariance should be 0 ideally.

essentially we want a diagonal matrix.

![[Pasted image 20250410111145.png]]

![[Pasted image 20250410111243.png]]

![[Pasted image 20250410111508.png]]

![[Pasted image 20250410111529.png]]

![[Pasted image 20250410111559.png]]

Next --> [[Deep Learning/Interpretation 2]]