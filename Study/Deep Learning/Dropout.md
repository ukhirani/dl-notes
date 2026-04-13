![[Pasted image 20250502161210.png]]

![[Pasted image 20250502161248.png]]

![[Pasted image 20250502161332.png]]

![[Pasted image 20250502161837.png]]

see both the tricks above - very imp

![[Pasted image 20250502161917.png]]
![[Pasted image 20250502162227.png]]

Here's what happens during test time :

![[Pasted image 20250502162407.png]]

you can say that if there was a meeting of all these nodes then each node was sleeping sometime and was awake with probability p --> then each node was present with prob. P

now we scale each weight with prob p. because we have p probability confidence in those weights w.

for example if you say your weight is 200 but if your p = 0.2 then i will take ur wait 40 as i trust you 20% (since ur p = 0.2)

![[Pasted image 20250502163002.png]]

this dropout basically does not allow the neurons to co-adapt, that means it will not be lazy and reliable on the other nodes that haan he will take care of it and update it's weight as randomly any of those neighbors will be dropped off and thus it needs to be active.

for example.

![[Pasted image 20250502163113.png]]

say for example hi is detecting nose, so now the other 4 neighbors can not rely on the hi to detect the nose and will have to do some sort of job to either detect nose or lips or hair or something.