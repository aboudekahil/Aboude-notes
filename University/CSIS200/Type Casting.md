---
author: aboude
---
# Type Casting
---

Created on: 2021-12-05-14:30
Last modified: 2021-12-05-14:31

---
### <span style="color: ff5545;text-transform: capitalize;">What is type casting? </span>
Type casting is when you assign a value of one primitive data type to another type.

In Java, there are two types of casting:

-   **[[Type Casting#span style color ff5545 text-transform capitalize Widening Casting span|Widening Casting]]** (automatically) - converting a smaller type to a larger type size  
    `byte` -> `short` -> `char` -> `int` -> `long` -> `float` -> `double`

-   **[[Type Casting#span style color ff5545 text-transform capitalize Narrowing casting span|Narrowing Casting]]** (manually) - converting a larger type to a smaller size type  
    `double` -> `float` -> `long` -> `int` -> `char` -> `short` -> `byte`

### <span style="color: #ff5545;text-transform: capitalize;"> Widening Casting. </span>
Widening casting is done automatically when passing a smaller size type to a larger size type:
```ad-example
```java
public class Main {
  public static void main(String[] args) {
    int myInt = 9;
    double myDouble = myInt; // Automatic casting: int to double

    System.out.println(myInt);      // Outputs 9
    System.out.println(myDouble);   // Outputs 9.0
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;"> Narrowing casting </span>
Narrowing casting must be done manually by placing the type in `parentheses` in front of the value:

```ad-example

```java
public class Main {
  public static void main(String[] args) {
    double myDouble = 9.78d;
    int myInt = (int) myDouble; // Manual casting: double to int

    System.out.println(myDouble);   // Outputs 9.78
    System.out.println(myInt);      // Outputs 9
  }
}
```

## Relevant:
[[Variables]] | [[Variable types]] | [[Java Syntax]]