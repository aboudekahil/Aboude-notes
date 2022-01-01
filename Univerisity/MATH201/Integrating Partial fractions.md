---
author: aboude
---
# Integrating Partial fractions
___

Created on: 2021-12-29-22:57
Last modified: 2021-12-31-18:12

___
### <span style="color: #ff5545;text-transform: capitalize;">What are partial fractions? and how do we integrate </span>
Partial fractions are fractions composed of 2 polynomials: $\frac{F(x)}{G(x)}$. When you want to integrate a partial fraction, you face two cases.

The first is when  $\deg(F(x))>\deg(G(x))$, in that case we do Euclidean division.

The second is when $\deg(F(x))<\deg(G(x))$, in that case we do partial fraction decomposition.

### <span style="color: #ff5545;text-transform: capitalize;">Euclidean division</span>

Let $R(x)=\frac{F}{G}$ be a rational function where $F$ and $G$ are polynomials and  $\deg(F)>\deg(G)$. Then we can preform [Euclidean division](https://en.wikipedia.org/wiki/Euclidean_division_of_polynomials) in order to transform the original equation.
> $$R(x)=\frac{F}{G} = E+\frac{F_1}{G}$$

$E$ and $F_1$ are polynomials where $E$ is the result of the [Euclidean division](https://en.wikipedia.org/wiki/Euclidean_division_of_polynomials) and $F_1$ is the remainder$\Big\{0\leq \deg(F_1) \leq\deg(G)\Big\}$

This helps integration by simplifying the equation and taking it apart and turning it into a simpler form
> $$\int R(x)\,dx=\int\frac{F}{G}\,dx=\int E\,dx+\int\frac{F_1}{G}\,dx$$

### <span style="color: #ff5545;text-transform: capitalize;">Partial fraction decomposition</span>
Let $R(x)=\frac{F}{G}$ be a rational function where $F$ and $G$ are polynomials and  $\deg(F)<\deg(G)$ and $G$ is factorized.

In this case we use the fact that $\frac{a}{b}+\frac{c}{d}=\frac{ad+bc}{cd}$

So we decompose $\frac{F}{G}$ into $\frac{a_1}{G_1}+\frac{a_2}{G_2}+\cdots+\frac{a_n}{G_n}$ where $a_1,a_2,...,a_n$ are unknown variables and $G_1,G_2,...,G_n$ are all the factors of $G$ 

```ad-example
> $$\frac{4}{(x-1)(x-4)}=\frac{a_1}{(x-1)}+\frac{a_2}{(x-4)}$$
```
$a_1$ and $a_2$ here can be found by multiplying the equation with $(x-1)(x-4)$ then replacing $x$ with the roots of $(x-1)(x-4)$ aka 1 and 4, then we get $a_1$ and $a_2$

```ad-note
if one of the factors of the denominator is of second degree the we do the decompostition like: 
> $$\frac{4x^2-8x+16}{x(x^2-4x+8)}=\frac{A}{x}+\frac{Bx+C}{x^2-4x+8}$$
```

This helps integration by simplifying the equation and taking it apart and turning it into a simpler form
> $$\int\frac{4x^2-8x+16}{x(x^2-4x+8)}\,dx=\int\frac{A}{x}\,dx+\int\frac{Bx+C}{x^2-4x+8}\,dx$$

## Reference
[[Table of integration formulas]]