---
author: aboude
---
# Arrays
___

Created on: 2021-12-07-20:19
Last modified: 2021-12-09-14:18

___

### <span style="color: #ff5545;text-transform: capitalize;">What are arrays?</span>
Arrays are used to store multiple values in a single variable, instead of declaring separate variables for each value.

To declare an array, define the variable type with **square brackets**:
```ad-example
title:Syntax
```java
String[] cars;
```
___
To insert values to it, we can use an array literal - place the values in a comma-separated list, inside curly braces:
```ad-example
title:Syntax
```java
String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
```
```ad-example
title: Example of array of integers
```java
int[] myNum = {10, 20, 30, 40};
```

### <span style="color: #ff5545;text-transform: capitalize;">accessing the elements of arrays</span>
You access an array element by referring to the index number.

This statement accesses the value of the first element in cars:

```ad-example
```java
String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
System.out.println(cars[0]);
// Outputs Volvo
```
```ad-note
Array indexes start with 0: [0] is the first element. [1] is the second element, etc.
```

### <span style="color: #ff5545;text-transform: capitalize;">change an array element</span>

To change the value of a specific element, refer to the index number:
```ad-example
title:Syntax
```java
cars[0] = "Opel";
```
___
```ad-example
```java
String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
cars[0] = "Opel";
System.out.println(cars[0]);
// Now outputs Opel instead of Volvo
```

### <span style="color: #ff5545;text-transform: capitalize;">array length</span>
To find out how many elements an array has, use the `length` property:
```ad-example
```java
String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
System.out.println(cars.length);
// Outputs 4
```

### <span style="color: #ff5545;text-transform: capitalize;">Looping through an array</span>
You can loop through the array elements with the `for` loop, and use the `length` property to specify how many times the loop should run.
```ad-example
```java
String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
for (int i = 0; i < cars.length; i++) {
  System.out.println(cars[i]);
}
// prints each element in the array
```
___

There is also a "**for-each**" loop, which is used exclusively to loop through elements in arrays:
![[For-each loops#span style color ff5545 text-transform capitalize What are for each loops span]]

## Relevant 
[[Variables]] | [[Variable types]] | [[Loops]] | [[Java Syntax]] | [[Multi-Dimensional Arrays]]