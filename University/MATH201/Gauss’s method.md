---
author: aboude
---
# Gauss’s method
___

Created on: 2021-12-12-10:36
Last modified: 2021-12-12-10:36

___

### <span style="color: #ff5545;text-transform: capitalize;">Theorem</span>
If a linear system is changed to another by one of these operations:

```ad-definition
title:operations

1. An equation is swapped with another

1. an equation has both sides multiplied by a nonzero constant
2. an equation is replaced by the sum of itself and a multiple of another
```

then the two systems have the same set of solutions.
\
\
Each of the three operations has a restriction. 

```ad-Dont
* Multiplying a row by 0 is not allowed because obviously that can change the solution set.

* Adding a multiple of a row to itself is not allowed because adding −1 times the row to itself has the effect of multiplying the row by 0.
* We disallow swapping a row with itself, to make some results in the fourth chapter easier. Besides, it’s pointless.
```

```ad-example
> $$
\begin{alignat*}{4}
x & {}+{} &  y & {}+{} & z & {}={} & 9 \\
 2x & {}+{} &  4y & {}-{} &  3z & {}={} &  1 \\
 3x & {}+{} & 6y & {}-{} & 5z & {}={} & 0
\end{alignat*}$$

$$\xrightarrow[-3r_1+r_3]{-2r_1+r_2}$$
> $$
\begin{alignat*}{4}
x & {}+{} & y & {} + {} & z & {} = {} & 9\\
& {}{} & 2y & {} - {} &  5z & {} = {} & -17\\
& {} {} & 3y  & {}-{} & 8z & {} = {} & -27
\end{alignat*}$$

$$\xrightarrow{-(3/2)r_2+r3}$$
> $$
\begin{alignat*}{4}
x & {}+{} & y & {} + {} & z & {} = {} & 9\\
& {}{} & 2y & {} - {} &  5z & {} = {} & -17\\
& {} {} &   & {}-{} & (1/2)z & {} = {} & -(3/2)
\end{alignat*}$$
```
In the example above we solved the linear system and showed that $z=3, y=-1, x=7$.

As illustrated above, the point of Gauss’s Method is to use the elementary reduction operations to set up back-substitution.