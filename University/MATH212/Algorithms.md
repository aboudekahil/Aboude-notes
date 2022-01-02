---
author: aboude
---
# Algorithms
___

Created on: 2021-12-19-12:15
Last modified: 2021-12-19-12:15

___

### <span style="color: #ff5545;text-transform: capitalize;">What are algorithms?</span>
An algorithm is a finite sequence of instructions to preform a computation or to solve a problem.

```ad-example
Here we're describing an algorithm to find the max number in a sequence of numbers:
1. Set the temporary maximum equal to the first integer in the sequence. (The temporary maximum will be the largest integer examined at any stage of the procedure.) 

3. Compare the next integer in the sequence to the temporary maximum, and if it is larger than the temporary maximum, set the temporary maximum equal to this integer.
4. Repeat the previous step if there are more integers in the sequence.
5. Stop when there are no integers left in the sequence. The temporary maximum at this point is the largest integer in the sequence.
```

### <span style="color: #ff5545;text-transform: capitalize;">Pseudo code</span>

An algorithm can also be described using a computer language. **However**, when that is done, only those instructions permitted in the language can be used. This often leads to a description of the algorithm that is complicated and difficult to understand. **Also**, because many programming languages are in common use, it would be undesirable to choose one particular language. So, instead of using a particular computer language to specify algorithms, a form of **pseudocode**,


```ad-example
Example of the max algorithm in pseudocode:
> $\text{procedure max(}a_1, a_2,\cdots,a_n: \text{integers})$
$\text{max} := a_1$
$\text{for i} := \text{2 to n}$ 
$\qquad \text{if max < }a_i \text{ then max := }a_i$ 
$\text{return max\{max is the largest element\}}$
```

### <span style="color: #ff5545;text-transform: capitalize;">properties of algorithms</span>

There are several properties that algorithms generally share. They are useful to keep in mind when algorithms are described. These properties are:

| <span style="color: #ff5545">Name</span> |                                     <span style="color: #ff5545">Description</span>                                     | 
|:----------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------:|
|               ***Input***                |                                            An algorithm takes input values.                                             |
|               ***Output***               |    For each set of inputs, an algorithm produces an output value. The output values are the solution to the problem.    |
|            ***Definiteness***            |                              The steps of the algorithms **must** be defined specifically.                              |
|            ***Correctness***             |                   An algorithm should produce the correct output values for each set of input values.                   |
|             ***Finiteness***             |    An algorithm should produce the desired output after a finite (but perhaps large) number of steps for any input.     |
|           ***Effectiveness***            |            It must be possible to perform each step of an algorithm exactly and in a finite amount of time.             |
|             ***Generality***             | The procedure should be applicable for all problems of the desired form, not just for a particular set of input values. |

## Reference
[[Searching Algorithms]] | [[Sorting Algorithms]]