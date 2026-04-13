# **Meaning of a word**

![[Pasted image 20250318185536.png]]

# **Need for word representation**

For effective representation of words we need to represent the words somehow in a way that it must encapsulate the word meaning.

We need to represent words as discrete symbols : such symbols for words can be represented by one-hot vectors: or *one-hot encoding*

![[Pasted image 20250318190115.png]]

Multiple problems here,
all these vectors are orthogonal. (if you take the dot product of these vectors it will always be 0)

***That's why it is not a good approach :***
- as vector size will be very large
- and no natural notion of similarity (due to orthogonal vectors)

# **Can we use existing ontologies like WordNet ?**

![[Pasted image 20250318190710.png]]![[Pasted image 20250318190731.png]]
*gloss* - description of the synset (strikes to me for the word "glossary" hehe)

notice the numbers on top of each synset

![[Pasted image 20250318191109.png]]

**But there are drawbacks in this too !**

![[Pasted image 20250318191346.png]]

# **Representing Words by Their Context**

![[Pasted image 20250318191534.png]]

From neighborhood you to try to guess the meaning of the word.

We approach it systematically using *count based approach*

![[Pasted image 20250318191718.png]]

row can be treated as a term vector.
column can be treated as a context vector.