---
author: aboude
---
# Multi-Dimensional Arrays
___

Created on: 2021-12-11-16:24
Last modified: 2021-12-11-16:25

___

A multidimensional array is an [[Arrays|array]] of arrays.

To create a two-dimensional array, add each array within its own set of **curly braces**.

```ad-example
```java
int[][] myNumbers = { {1, 2, 3, 4}, {5, 6, 7} };
```
**myNumbers** is now an array with two arrays as its elements.

To access the elements of the **myNumbers** array, specify two indexes: one for the array, and one for the element inside that array.

```ad-example
This example accesses the third element (2) in the second array (1) of myNumbers:
```java
int[][] myNumbers = { {1, 2, 3, 4}, {5, 6, 7} };
int x = myNumbers[1][2];
System.out.println(x); // Outputs 7
```

We can also use a [[For loops|for loop]] inside another [[For loops|for loop]] to get the elements of a two-dimensional array (we still have to point to the two indexes).

```ad-example
```java
public class Main {
  public static void main(String[] args) {
    int[][] myNumbers = { {1, 2, 3, 4}, {5, 6, 7} };
    for (int i = 0; i < myNumbers.length; ++i) {
      for(int j = 0; j < myNumbers[i].length; ++j) {
        System.out.println(myNumbers[i][j]);
      }    
	 }
  }
}
```

Image of 2d array of numbers.
![[arr.png]]
## Relevant 
[[Arrays]] | [[For loops]]