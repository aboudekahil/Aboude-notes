---
author: aboude
---
# Sorting Algorithms
___

Created on: 2021-12-19-15:44
Last modified: 2021-12-19-15:44

___
### <span style="color: #ff5545;text-transform: capitalize;">Why?</span>
Ordering elements in an array is a problem that occurs a lot in programming, for example to make a Phone Book we need the names to be put in alphabetical order.

### <span style="color: #ff5545;text-transform: capitalize;">Bubble sort</span>
The bubble sort is one of the simplest sorting algorithms, but not one of the most efficient. It puts a list into increasing order by successively comparing neighbor elements, interchanging them if they’re not in the right order. To carry out the bubble sort, we perform the basic operation, that is, interchanging a larger element with a smaller one following it, starting at the beginning of the list, for a full pass. We iterate this procedure until the sort is complete.

```ad-note
title:pseudo code
**procedure** bubblesort($a_1$,...,$a_n$:real numbers with $n\geq 2$)
**for** $i := 1$ to $n-1$
$\quad$**for** $j:=1$ **to** $n-i$
$\qquad$**if** $a_j > a_{j+1}$ **then** interchange $a_j$ and $a_{j+1}$ 
```

### <span style="color: #ff5545;text-transform: capitalize;">Insertion sort</span>
The insertion sort is a simple sorting algorithm, but it is usually not the most efficient. To sort a list with n elements, the insertion sort begins with the second element. The insertion sort compares this second element with the first element and inserts it before the first element if it does not exceed the first element and after the first element if it exceeds the first element. At this point, the first two elements are in the correct order. The third element is then compared with the first element, and if it is larger than the first element, it is compared with the second element; it is inserted into the correct position among the first three elements.

```ad-note
title:pseudo code
**procedure** insertionSort($a_1,a_2,...,a_n$:real numbers with $n \geq 2$)
**for** $j:=2$ to $n$
$\quad$$i:=1$
$\quad$**while** $a_j > a_i$
$\qquad$$i := i+1$
$\quad$$m:=a_j$
$\quad$**for** $k:=0$ **to** $j-i-1$
$\qquad$$a_{j-k}:=a_{j-k-1}$
$\quad$$a_i:=m$
```
## Reference
[[Algorithms]] | [[Searching Algorithms]]