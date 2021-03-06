---
author: aboude
---
# Counting sample points
___

Created on: 2022-01-26-12:43
Last modified: 2022-01-31-12:42

___
### <span style="color: #ff5545;text-transform: capitalize;">Multiplication rule</span>

If a first operation can be performed in $n_1$ ways and a second experiment can be performed in $n_2$, the two experiments can be performed together in $n_1 \times n_2$ ways

```ad-note
title: special case

if an axperiment resulting in $n$ out comes is repeated $p$ times, the obtained number of outcomes is: 
> $$n^p$$
```
___
```ad-example
title: Example 1
If a pair of dice is thrown $1$ time, the number of outcomes is 
> $$6 \times 6 = 6^2$$
```
```ad-example
title: Example 2
if a student must choose $2$ courses, one from a selection of $4$ and the other from a selection of $2$ then the number of possible outcomes is
> $$4 \times 2 = 8$$
```
```ad-example
title: Example 3
How many even, four digit numbers: $(0,1,2,5,6,9)$ where each digit can only be used once?

first of all we need to look at the number of the conditions put at our number:
	1. the number has to be 4 digits
	2. the first number cannot be 0
```

### <span style="color: #ff5545;text-transform: capitalize;">Permutation</span>
It’s the number of ways of permuting $n$ distinct objects (with order):

> $$n!$$

### <span style="color: #ff5545;text-transform: capitalize;">Circle permutation</span>
It’s the number of ways of permuting $n$ distinct objects in a closed path:
> $$(n-1)!$$

### <span style="color: #ff5545;text-transform: capitalize;">Permutation with similar objects</span>
It’s the number of ways of permuting $n$ objects where $n_1$ are similar, $n_2$ are similar $\cdots n_k$ are similar is

> $$\frac{n!}{n_1!\,n_2!\,\cdots\,n_k!}$$

### <span style="color: #ff5545;text-transform: capitalize;">Partitioning into groups</span>
It’s the number of ways of partitioning $n$ elements into $k$ groups containing respectively $n_1$ elements,$\cdots\,n_k$ elements is:

> $$\frac{n!}{n_1!\,n_2!\,\cdots\,n_k!}$$

### <span style="color: #ff5545;text-transform: capitalize;">Combination (without repitition)</span>

If you have $n$ distinct object divided into $p$ people in groupe 1 and $n-p$ people in group 2 you use `combination`

> $$\frac{n!}{p!(n-p)!}=C^p_n={n\choose p}$$

### <span style="color: #ff5545;text-transform: capitalize;">Arrangement (without repitition)</span>

It’s the number of ways of choosing $p$ objects out of $n$ distinct objects where the order matters

> $$n\times(n-1)\times\cdots\times(n-p+1)$$
> $$P_n^p = A_n^p = \frac{n!}{(n-p)!}=C^p_n \times p!$$

```ad-note
number of ways of choosing $p$ objects out of $n$ `with` repitition
> $$n^p$$
```

## Reference
[[Sample Space]] | [[Event]]