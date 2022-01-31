# Basic Probability Rules
___

Created on: 2022-01-31-12:56
Last modified: 2022-01-31-12:56

___

### <span style="color: #ff5545;text-transform: capitalize;">Some rules</span>
The probability of an event $A$ is the sum of weights of sample points in $A$, given that the weught of sample space $S$ is $1$.

> $$P(\emptyset)=0,\,P(S)=1,\,0\leq P(A) \leq 1$$

If $A_1$ and $A_2$ are mutually exclusive

> $$P(A_1 \cup A_2)=P(A_1)+P(A_2)$$
> $$P(A \cup B) = P(A)+P(B)-P(A\cap B)$$

```ad-definition
If $A_1…A_n$ are mutually exclusive **then**

> $$P(A_1\cup A_2 ... \cup A_n)=P(A_1)+P(A_2)+\cdots+P(A_n)$$
```
```ad-definition
If $A^\prime$ is the complimentary of $A$ **then**:

> $$A\cup A^\prime = S$$
> $$1 = P(S) = P(A\cup A^\prime) = P(A)+P(A^\prime)
> P(A^\prime) = 1-P(A)
```
```ad-definition
when we have a union of more than one event the formula becomes

> $$P(A\cup B\cup C)=P(A)+P(B)+P(C)-P(A\cap B)-P(A\cap C)-P(B\cap C)+P(A\cap B\cap C)$$
```

```ad-note
IF all the sample points are equally likely to occur **then**

> $$P(A)=\frac{\text{number of favorable outcomes}}{\text{number of possible outcomes}}$$
```
## Reference