---
author: aboude
---
# Trigonometric substitution
___

Created on: 2021-12-29-22:57
Last modified: 2022-01-01-13:28

___
### <span style="color: #ff5545;text-transform: capitalize;">what is trig substitution?</span>
In mathematics, trigonometric substitution is the substitution of trigonometric functions for other expressions. In calculus, trigonometric substitution is a technique for evaluating integrals. There are 3 cases for the substitution, when $a^2-x^2$, when $a^2-x^2$ and when $x^2-a^2$.
### <span style="color: #ff5545">Case I: Integrals Containing $a^2 − x^2$</span>
let $x=a\sin(\theta)$ and use the identity $1-\sin^2(\theta)=\cos^2(\theta)$
```ad-example
> $$\int\frac{dx}{\sqrt{a^2-x^2}}$$ 
 
let
> $$x=a\sin{\theta},\,dx=a\cos{\theta}d\theta,\,\theta=\arcsin{\frac{x}{a}}$$

Then,
> $$\begin{align*}
\int\frac{dx}{\sqrt{a^2-x^2}}&=\int\frac{a\cos{}\,d\theta}{\sqrt{a^2-a^2\sin^2{\theta}}}\\ \\
&=\int\frac{a\cos{\theta}\,d\theta}{\sqrt{a^2(1-\sin^2\theta)}}\\ \\
&=\int\frac{a\cos{\theta}\,d\theta}{\sqrt{a^2\cos^2\theta}}\\ \\
&=\int\,d\theta \\ \\
&=\theta + C \\ \\
&=\arcsin{\frac{x}{a}}+C \\ \\
\end{align*}$$
```

##### Geometric construction for Case I
![[Case I geomteric construction.png]]
### <span style="color: #ff5545">Case II: Integrals Containing $a^2+x^2$</span>
Let $x=a\tan{\theta}$ and use the identity $1+\tan^2\theta=\sec^2\theta$
```ad-example
> $$\int\frac{dx}{a^2+x^2}$$

Let,
> $$x=a\tan\theta,\,dx=a\sec^2\theta\,d\theta,\,\theta=\arctan{\frac{x}{a}}$$

Then,
> $$\begin{align*}
> \int\frac{dx}{a^2+x^2}&=\int\frac{a\sec^2\theta\,d\theta}{a^2+s^2\tan^2\theta}\\ \\
&= \int\frac{a\sec^2\theta\,d\theta}{a^2(1+\tan^2\theta)} \\ \\
&= \int\frac{a\sec^2\theta\,d\theta}{a^2\sec^2\theta} \\ \\
&= \int\frac{d\theta}{a} \\ \\
&=\frac{\theta}{a}+C \\ \\
&= \frac{1}{a}\arctan\frac{x}{a}+C
> \end{align*}$$
```
##### Geometric construction for Case II
![[Case II geomteric construction.png]]
### <span style="color: #ff5545">Case III: Integrals Containing $x^2-a^2$</span>
Let $x=a\sec\theta$ and use the identity $\sec^2\theta-1=\tan^2\theta$

```ad-example
> $$\sqrt{x^2-a^2}$$

Let 
> $$x=a\sec\theta,\,dx=a\sec\theta\tan\theta\,d\theta,\,\theta=\sec^{-1}(\frac{x}{a})$$

Then,
> $$\begin{align*}
\int\sqrt{x^2-a^2}\,dx&=\int\sqrt{a^2\sec^2\theta-a^2}\cdot a\sec\theta\tan\theta\,d\theta \\ \\
&=\int\sqrt{a^2(\sec^2\theta-1)}\cdot a\sec\theta\tan\theta\,d\theta \\ \\
&=\int\sqrt{a^2\tan^2\theta}\cdot a\sec\theta\tan\theta\,d\theta \\ \\
&=\int a^2\sec\theta\tan^2\theta\,d\theta \\ \\
&=a^2\int (\sec\theta)(\sec^2\theta-1)\,d\theta \\ \\
&=a^2\int(\sec^3\theta-\sec\theta)\,d\theta
> \end{align*}$$

Finally, we do some trigonometric math and do the rest of the equation.
```
##### Case III geomteric construction
![[Case III geomteric construction.png]]
## Reference
[[Table of integration formulas]] | [[u-substitution]]