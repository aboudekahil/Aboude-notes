---
author: aboude
---
# Matrices
___

Created on: 2021-12-12-15:04
Last modified: 2021-12-16-21:56

___

### <span style="color: #ff5545;text-transform: capitalize;">What’s a matrix?</span>
In mathematics, a matrix (plural matrices) is a rectangular array or table of numbers, symbols, or expressions, arranged in rows and columns, which is used to represent a mathematical object or a property of such an object.
```ad-example
The matrix below is a two by three matrix (“$2\times3$-matrix”).
> $$ A=
\begin{bmatrix}
2&5&7\\\color{red}5 & -11 & 0 
\end{bmatrix}$$

```
```ad-note
5 is an entry inside the matrix A, we denote an entry by writing the name of the matrix then the row and column number seperated by a comma as a subscript.

for example 5 is $A_{1,2}$.
```
### <span style="color: #ff5545;text-transform: capitalize;">Square matrices</span>
Square matrices are matrices with the same number of rows and columns. Square matrices play a big role in many fields including [[Solving linear systems|linear systems]] 

```ad-example
The matrix below is a square matrix with 3 rows and 3 columns.
> $$
A=\begin{bmatrix}
2 & 7 & 23 \\
6 & 66 & 666 \\
47 & 48 & 49
\end{bmatrix}$$
```

### <span style="color: #ff5545;text-transform: capitalize;">matrix addition</span>
When adding two matrices, we add each corresponding entries with each-others then return the resulting matrix

```ad-example
An example of matrix addition:
> $$\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
+\begin{bmatrix}
4 & 3 \\
3 & 1
\end{bmatrix}=\begin{bmatrix}1+4 & 2+3\\3+3 & 4+1\end{bmatrix}=\begin{bmatrix}5 & 5\\6 & 5\end{bmatrix}$$
```
```ad-warning
Matrices should be the same size when adding them together.
```
### <span style="color: #ff5545;text-transform: capitalize;">scalar multiplication</span>
Scalar multiplication is multiplying every entry of the matrix by a number, so basically **scaling every entry in the matrix by a value**
```ad-example
An example of scalar multiplication
> $$5\cdot\begin{bmatrix}2 & 3 \\ 2 & 0\end{bmatrix}=\begin{bmatrix}5\cdot2 & 5\cdot3 \\ 5\cdot2 & 5\cdot0\end{bmatrix}=\begin{bmatrix}10 & 15\\10 & 0\end{bmatrix}$$
```

### <span style="color: #ff5545;text-transform: capitalize;">Transposition</span>
The transpose of an m-by-n matrix $A$ is the n-by-m matrix $A^T$
```ad-example
An example of Transposition
> $$A=\begin{bmatrix}1 & 2 & 3 \\ 4 & 3 & 1\end{bmatrix}\xrightarrow{\text{Transposition}}A^T=\begin{bmatrix}1 & 4 \\2 & 3\\3 & 1\end{bmatrix}$$
```

### <span style="color: #ff5545;text-transform: capitalize;">matrix multiplication</span>
Best way to learn matrix multiplication is http://matrixmultiplication.xyz/
<iframe src="http://matrixmultiplication.xyz/" width=700 height=500/>

```ad-warning
* the number of columns in the first matrix must be equal to the number of rows in the second matrix.

* $A\cdot B \neq B \cdot A$

```

### <span style="color: #ff5545;text-transform: capitalize;">identity matrices</span>
 **Identity matrix** of size _n_ is the _n_ × _n_ square matrix with ones on the main diagonal and zeros elsewhere. It is denoted by $I_n$, or simply by _I_ if the size is immaterial or can be trivially determined by the context.
 
 ```ad-example
 > $$I_1=\begin{bmatrix}1\end{bmatrix},\:\:I_2=\begin{bmatrix}1&0\\0&1\end{bmatrix}, I_n=\begin{bmatrix}1&0&0&\cdots&0\\0&1&0&\cdots&0\\0&0&1&\cdots&0\\\vdots&\vdots&\vdots&\ddots&\vdots\\0&0&0&0&1\end{bmatrix}$$
 ```
 
 ### <span style="color: #ff5545;text-transform: capitalize;">Determinants</span>
 In mathematics, the determinant is a scalar value that is a function of the entries of a square matrix. It allows characterizing some properties of the matrix and the linear map represented by the matrix. In particular, the determinant is nonzero if and only if the matrix is invertible.
 
 To calculate a $2\times 2$ matrix determinant you do the following
 
 > $$|A|=\det(A)=\det\begin{pmatrix}a&b\\c&d\end{pmatrix}=\begin{vmatrix}a&b\\c&d\end{vmatrix}=ad-bc$$

And to calculate a $3\times 3$ matrix determinant you do the following
> $$\det\begin{pmatrix}a&b&c\\d&e&f\\g&h&i\end{pmatrix}=a\begin{vmatrix}e&f\\h&i\end{vmatrix}-b\begin{vmatrix}d&f\\g&i\end{vmatrix}+c\begin{vmatrix}d&e\\g&h\end{vmatrix}$$

```ad-note
- $\det(A\times B)=\det(A)\times \det(B)$

- $\det(A+B)\neq\det(A)+\det(B)$
- $\det(A^T)=\det(A)$
- $\det(A^{-1})=\frac{1}{\det(A)}$
- $\det(\text{adj}(A_{n\times n}))=\det(A_{n\times n})^{n-1}$
```

```ad-note
- If matrix $B$ is obtained by interchanging two rows from a matrix $A$ then $\det(B)=-\det(A)$

- If matrix $B$ is obtained from multiplying a row of matrix $A$ by a scalar $r$ then $\det(B)=r\det(A)$
- If matrix $B$ is obtained by addiing a multiple of row to another then $\det(A)=\det(B)$


```

### <span style="color: #ff5545;text-transform: capitalize;">Invertible matrix</span>
In linear algebra, an n-by-n square matrix $A$ is called invertible (also nonsingular or nondegenerate), if there exists an n-by-n square matrix $B$ such that
> $$AB=BA=I_n$$

where $I_n$ denotes the n-by-n identity matrix and the multiplication used is ordinary matrix multiplication.
```ad-note
The inverse of a matrix $A$ is denoted by $A^{-1}$
```
To invert a matrix, we first augment our matrix with the identity matrix of the same size
> $$A=\begin{bmatrix}-1&3/2\\1&-1\end{bmatrix}$$
> $$\downarrow\text{augmentation}$$
> $$\left[\begin{array}{cc|cc}-1& 3/2 & 1 & 0 \\
1 & -1 & 0 & 1 \\
\end{array}
\right]$$

Then we use [[Gauss’s method|gaussian elimination]] to turn the left side of the matrix into the identity matrix
> $$\left[\begin{array}{cc|cc}-1& 3/2 & 1 & 0 \\
1 & -1 & 0 & 1 \\
\end{array}
\right]\xrightarrow{r_1+r_2}\left[\begin{array}{cc|cc}-1& 3/2 & 1 & 0 \\
0 & 1/2 & 1 & 1 \\
\end{array}
\right]$$
> ___
> $$\left[\begin{array}{cc|cc}
-1& 3/2 & 1 & 0 \\
0 & 1/2 & 1 & 1 \\
\end{array}
\right]\xrightarrow{r_1-3r_2}\left[\begin{array}{cc|cc}
-1& 0 & -2 & -3 \\
0 & 1/2 & 1 & 1 \\
\end{array}
\right]$$
> ___
> $$\left[\begin{array}{cc|cc}
-1& 0 & -2 & -3 \\
0 & 1/2 & 1 & 1 \\
\end{array}
\right]\xrightarrow[2r_2\rightarrow r_2]{-r_1\rightarrow r_1}\left[\begin{array}{cc|cc}
1& 0 & 2 & 3 \\
0 & 1 & 2 & 2 \\
\end{array}
\right]$$

so
> $$A^{-1}=\begin{bmatrix}2&3\\2&2\end{bmatrix}$$