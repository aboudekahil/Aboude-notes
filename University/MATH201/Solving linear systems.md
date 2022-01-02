---
author: aboude
---
# Linear system of equations
___

Created on: 2021-12-12-09:31
Last modified: 2021-12-12-09:31

___

Systems of linear equations are common in science and mathematics.
\
\
The example below is from Chemistry. We can mix, under controlled conditions, toluene C7H8 and nitric acid HNO3 to produce trinitrotoluene C7H5O6N3 along with the byproduct water (conditions have to be very well controlled — trinitrotoluene is better known as TNT). In what proportion should we mix them? The number of atoms of each element present before the reaction must equal the number present afterward.

> $$xC_{7}H_{8} +yHNO_{3} \rightarrow zC_{7}H_{5}O_{6}N_{3} + wH_{2}O$$

Applying that in turn to the elements C, H, N, and O gives this system.

>  $$7x = 7z$$
>  $$8x +1y = 5z + 2w$$
>  $$1y = 3z$$
>  $$3y=6z+1w$$
### <span style="color: #ff5545;text-transform: capitalize;">Linear combination</span>
A linear combination of $x_{1},...,x_{n}$ has the form:
> $$a_{1}x_{1}+a_{2}x_{2}+a_{3}x_{3}+\cdots+a_{n}x_{n}$$

where $a_{1},...,a_{n}\in\mathbb{R}$ are the combination coefficients.

### <span style="color: #ff5545;text-transform: capitalize;">linear equation</span>
A linear equation in the variables $x_{1},...,x_{n}$ has the form:
>$$a_{1}x_{1}+a_{2}x_{2}+a_{3}x_{3}+\cdots+a_{n}x_{n} = d$$

where $d \in \mathbb{R}$ is the constant
\
An n-tuple $(s_{1},s_{2},...,s_{n}) \in \mathbb{R}^{n}$ is a solution of the equation if substituting the numbers $s_1,s_2,...,s_n$ for the variables gives a true statement.

### <span style="color: #ff5545;text-transform: capitalize;">System of linear equations</span>
A System of linear equations
>$$a_{1,1}x_{1}+a_{1,2}x_{2}+\cdots+a_{1,n}x_{n}=d_1$$
> $$a_{2,1}x_{1}+a_{2,2}x_{2}+\cdots+a_{2,n}x_{n}=d_2$$
> $$\qquad\quad\quad\quad\qquad\qquad\qquad\,\,\,\,\vdots$$
> $$a_{m,1}x_{1}+a_{m,2}x_{2}+\cdots+a_{m,n}x_{n}=d_m$$

has the solution $(s_1,s_2,…,s_3)$ if that n-tuple is a solution of all the equations

## Relevant 
[[Matrices]] | [[Gauss’s method]]