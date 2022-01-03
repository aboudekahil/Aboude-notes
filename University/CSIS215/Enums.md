---
author: aboude
---
# Enums
___

Created on: 2022-01-03-15:21
Last modified: 2022-01-03-15:21

___

### <span style="color: #ff5545;text-transform: capitalize;">What are enums?</span>
An `enum` is a special "class" that represents a group of **constants** (unchangeable variables, like `final` variables).

To create an `enum`, use the `enum` keyword (instead of class or interface), and separate the constants with a comma. Note that they should be in uppercase letters:

```ad-example
```java
enum Level {
  LOW,
  MEDIUM,
  HIGH
}
```
You can access `enum` constants with the **dot** syntax
```ad-example
```java
Level myVar = Level.MEDIUM;
```

```ad-note
**Enum** is short for "enumerations", which means "specifically listed".
```

### <span style="color: #ff5545;text-transform: capitalize;">Enums inside class</span>
You can also have an `enum` inside a class
```ad-example
```java
public class Main {
  enum Level {
    LOW,
    MEDIUM,
    HIGH
  }

  public static void main(String[] args) {
    Level myVar = Level.MEDIUM; 
    System.out.println(myVar); // prints “MEDIUM”
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">Enums inside a switch statements</span>
Enums are often used in `switch` statements to check for corresponding values
```ad-example
```java
enum Level {
  LOW,
  MEDIUM,
  HIGH
}

public class Main {
  public static void main(String[] args) {
    Level myVar = Level.MEDIUM;

    switch(myVar) {
      case LOW:
        System.out.println("Low level");
        break;
      case MEDIUM:
         System.out.println("Medium level");
        break;
      case HIGH:
        System.out.println("High level");
        break;
    }
  }
}
```
## Reference