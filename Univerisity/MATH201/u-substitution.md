---
author: aboude
---
# u-substitution
___

Created on: 2021-12-24-18:19
Last modified: 2021-12-24-18:19

___

### <span style="color: #ff5545;text-transform: capitalize;">How to do u-substitution</span>
Most problems in integration that we face won’t be so simple. For example:
> $$\int 2x\cos(x^2)\,dx$$

The keen eye will notice that $2x\cos(x^2)$ is the derivative of $\sin(x^2)$ by using the chain rule, so
> $$\int 2x\cos(x^2)\,dx = \sin(x^2)+C$$

However, other integrals aren’t so obvious. Consider this problem
> $$\int x^3\sqrt{1-x^2}\, dx$$

We can make solving it easier by exchanging the variable inside the function, like $u=1-x^2$.

Which will turn the integral into $\int x^3\sqrt{u}\,dx$.

Now we need to change the $dx$ into a $du$.

By deriving both sides of $u=1-x^2$ with respect of $x$ we get $\frac{du}{dx}=-2x$ → $du=-2x\,dx$.

Now we can multiply the integral by $\frac{-2}{-2}$ to get $\frac{1}{-2}\int-2x^3\sqrt{u}\,dx$ which turns into $\frac{1}{-2}\int x^2\sqrt{u}\,du$.

Finally by using the fact that $u=1-x^2 \rightarrow x^2=1-u$ we can rewrite the integral as $\frac{1}{-2}\int (1-u)\sqrt{u}\,du$

Solving this integral is easy:
> $$\frac{1}{-2}\int (1-u)\sqrt{u}\,du = \frac{1}{-2}\int u^{1/2}-u^{3/2}\,du = \frac{1}{-2}(\frac{u^{3/2}}{3/2}-\frac{u^{5/2}}{5/2})+C =$$
> $$-2(\frac{(1-x^2)^{3/2}}{3/2}-\frac{(1-x^2)^{5/2}}{5/2}))+C$$

```ad-example
title:Summary
1. We find a value to exchange a variable to

1. We derive both the new variable and the value we chose to exchange it to with respect to $x$
2. We **substitue** the new variable and the derived value with the original value we chose and $dx$
3. We solve the integral then re-replace the new variable with the old value
```

## Reference
[[Table of integration formulas]]