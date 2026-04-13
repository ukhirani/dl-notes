Presenting the **XOR*** Function...............
![[Pasted image 20250313135453.png]]

![[Pasted image 20250313135543.png]]

This is a simple boolean function a perceptron cannot handle as it is not linearly separable.

![[Pasted image 20250313135634.png]]

Most real world data is not linearly separable and will always contain some outliers,

![[Pasted image 20250313140024.png]]

and even if there are no outliers, still the data may not be linearly separable (take for example the figure down below), and we need computational units (models) which can deal with such data.

![[Pasted image 20250313140004.png]]

While a single perceptron cannot deal with such data, a network of perceptrons can indeed deal with such data.

Before proceeding towards that, we will see all different types of non-linearly separable functions.

How many boolean functions can you design from 2 inputs. ----> 2^4 = 16
                                        3 inputs. ---> 2^8 = 256
                                         n inputs ----> 2^2^n functions possible.

**Of these (2 input functions), how many are linearly separable ?**
***Ans*.** *All of them except XOR and !XOR .*

**For n inputs ? How many are not linearly separable functions ?** -> We don't know, but there exists some which are not linearly separable.

To see next --> [[Network of Perceptrons And It's Representation Power]]

