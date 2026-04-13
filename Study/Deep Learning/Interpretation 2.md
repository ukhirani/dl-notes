![[Pasted image 20250411161719.png]]

remember in interpretation 1 we talked about how we needed only the top-k dimensions to represent the data such that there is a high variance along each axis.

so now if we use those k axes and represent the data among those axes we can't fully reconstruct the data, meaning summation of RHS terms != LHS term as we need to get rid of noisy and redundant dimensions.

![[Pasted image 20250411161945.png]]

![[Pasted image 20250411162017.png]]

 ![[Pasted image 20250411162220.png]]

this is the error that we are trying to find.
so the part that will actually be the result will be the noise that we were trying to initially filter out. 

![[Pasted image 20250411162622.png]]

some further calculations ahead we find out that in this dot product there will be mainly two types of products that will be happening , the one with same i and with not the same i 

for example. p1 * p1 (same i)
for example. p1 * p2 (not the same i)

![[Pasted image 20250411162757.png]]

so this will how it will look like if we divide the sum into those two parts
however for the p with same i the pT X P will be 1 and 0 otherwise so the 2nd term will cancel out to 0 in the above formula.

![[Pasted image 20250411162916.png]]

![[Pasted image 20250411162946.png]]

![[Pasted image 20250411162958.png]]

![[Pasted image 20250411163158.png]]

and we can write the stuff in the red box as the text written in red

![[Pasted image 20250411163221.png]]

![[Pasted image 20250411163327.png]]

![[Pasted image 20250411163420.png]]

and what does all these mean , this red box highlights the covariance between column 1 and column 2.

thus equal to m XTX.

all that boils down to this

![[Pasted image 20250411163528.png]]

![[Pasted image 20250411163648.png]]

![[Pasted image 20250411163744.png]]

thus we need to select the P with the smallest eigen vectors and then remove that so that our error is minimized while removing those axes from these basis.

Let's learn the same with this example.

![[Pasted image 20250411163918.png]]

we now both the basis vectors are orthogonal and u1T u2 = 0 (u1 transpose u2 = 0)

now orthonormal vectors require the magnitude of the vectors to be 0, thus doing the below operation dividing the vectors with their magnitudes.

![[Pasted image 20250411164058.png]]

![[Pasted image 20250411164156.png]]

so to represent x in the newer dimensions , we can reconstruct it using this :

![[Pasted image 20250411164235.png]]

now what would happen if we throw away the second dimension.

![[Pasted image 20250411164308.png]]

thus in doing this i m not losing much information whilst removing the low variance dimension. 

![[Pasted image 20250411164620.png]]

Next ---> [[Deep Learning/Interpretation 3]]