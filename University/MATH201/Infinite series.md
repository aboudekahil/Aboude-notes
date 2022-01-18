---
author: aboude
---
# Infinite series
___

Created on: 2021-12-29-22:59
Last modified: 2022-01-18-15:19

___

### <span style="color: #ff5545;text-transform: capitalize;">What are inifinite series?</span>

Infinite series are the sum of infinitely many numbers related in a given way and listed in a given order.

For an infinite series $a_1 + a_2 + a_3 +\cdots$, a quantity $S_n = a_1 + a_2 +\cdots+ a_n$, which involves adding only the first n terms, is called a partial sum of the series.

 If $S_n$ approaches a fixed number $S$ as $n$ becomes larger and larger, the series is said to converge. 
 
 In this case, $S$ is called the sum of the series. An infinite series that does not converge is said to diverge. In the case of divergence, no value of a sum is assigned. For example, the $n$-th partial sum of the infinite series $1 + 1 + 1 +\cdots$ is $n$. As more terms are added, the partial sum fails to approach any finite value (it grows without bound). Thus, the series diverges. 
 
```ad-example
title:  An example of a convergent series is
$$1+\frac{1}{2}+\frac{1}{4}+\cdots+\frac{1}{2^n}$$ 
\
As _n_ becomes larger, the partial sum approaches 2, which is the sum of this infinite series.
```

### <span style="color: #ff5545;text-transform: capitalize;">Convergence tests</span>

Certain standard tests can be applied to determine the convergence or divergence of a given series, but such a determination is not always possible. 

##### DCT

In general, if the series $a_1 + a_2 +\cdots$ converges, then it must be true that an approaches $0$ as $n$ becomes larger.

Furthermore, adding or deleting a finite number of terms from a series never affects whether or not the series converges. Furthermore, if all the terms in a series are positive, its partial sums will increase, either approaching a finite quantity (converging) or growing without bound (diverging).

This observation leads to the conclusion that 
```ad-definition
**if** 
> $$0 \leq a_n \leq b_n $$

**and** $b_n$ is `convergent`

**Then** $a_n$ is `convergent`
```

##### LCT

```ad-definition
**if**
> $$a_n \geq 0,\quad b_n > 0$$

**and**
> $$c=\lim_{n\rightarrow\infty}{\frac{a_n}{b_n}}$$

**and**
> $$c>0,\quad c<\infty$$

**Then** either `both` series converge or `both` diverge
```

##### Ratio Test
```ad-definition
**if**
> $$a_n>0\,,\quad \frac{a_{n+1}}{a_n} < 1$$

**Then** $a_1+a_2+\cdots$ converges
```

##### Root Test
```ad-definition
**if**
> $$a_n>0\,,\quad \sqrt[n]{a_n} < 1$$

**Then** $a_1+a_2+\cdots$ converges
```

##### Integral test
```ad-definition
Suppose that $f(x)$ is a continuous, positive and decreasing function on the interval $\Big[k,\infty\Big)$ and that $f(n)=an$ **then**,

1. if $$

## Reference