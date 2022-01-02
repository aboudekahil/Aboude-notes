---
author: aboude
---
# Searching Algorithms
___

Created on: 2021-12-19-15:43
Last modified: 2021-12-19-15:43

___
### <span style="color: #ff5545;text-transform: capitalize;">Why use them?</span>
The problem of searching through an ordered array of elements occurs very commonly in programming. For example searching a dictionary for a word to check its spelling. However we need to search the array effectively in order to save time. 

```ad-note
In this note we'll be assuming that we're searching for $x$ in the array $A$, we'll denote the elements of the array with $a_i$ with $i$ being its index.
Arrays start woth the index 0.
```

### <span style="color: #ff5545;text-transform: capitalize;">Linear search</span>
Linear search of sequential search is probably the first algorithm anyone thinks of when faced with a searching problem. 

##### How?
First we compare $x$ with $a_0$, if $x = a_0$ then the solution is $a_0$, otherwise we move on to $a_1$ and do the same.

```ad-note
title:pseudo code
**procedure** linear search($x$: integer, $a_1$, $a_2$,...,$a_n$: distinct integers)
$i := 1$
**while** ($i \leq n$ and $x \neq a_i$)
$\quad$$i := i + 1$ 
**if** $i \leq n$ **then** location $:= i$ 
**else** location $:= 0$
**return** location

{location is the subscript of the term that equals x, or is 0 if x is not found}
```

### <span style="color: #ff5545;text-transform: capitalize;">Binary search</span>
This algorithm can be used when the list has terms occurring in order of increasing size. Binary search proceeds by comparing $x$ with the middle element in the array. 

\
If $x$ is equal to the element, then we found our solution.

Else if $x$ is smaller than the middle element, then we cut the array in half, take the left side and do the binary search on the half that’s left.

Else if $x$ is bigger than the middle element, then we cut the array in half, take the right side and do binary search on the half that’s left.

Repeat these steps until the element is found.


```ad-note
title:pseudo code
**procedure** binary search ($x$: integer, $a_1$, $a_2$,...,$a_n$: increasing integers)
$i := 1$ {$i$ is left endpoint of search interval}
$j := n$ {$j$ is right endpoint of search interval}
**while** $i < j$
$\quad$$m := \lfloor(i+j)/2\rfloor$
$\quad$**if** $x > a_m$ **then** $i := m + 1$
$\quad$**else** $j := m$ 
**if** $x = a_i$ **then** location $:= i$ 
**else** location $:= 0$
return location

{location is the subscript i of the term ai equal to x, or 0 if x is not found}
```

## Reference
[[Algorithms]] | [[Sorting Algorithms]]