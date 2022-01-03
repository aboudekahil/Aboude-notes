---
author: aboude
---
# ArrayList
___

Created on: 2022-01-03-20:13
Last modified: 2022-01-03-20:13

___
### <span style="color: #ff5545;text-transform: capitalize;">what are arraylists</span>
The `ArrayList` class is a resizable array, which can be found in the `java.util` package.

The difference between a built-in array and an `ArrayList` in Java, is that the size of an array cannot be modified (if you want to add or remove elements to/from an array, you have to create a new one). While elements can be added and removed from an `ArrayList` whenever you want. The syntax is also slightly different

```ad-example
Create an `ArrayList` object called **cars** that will store strings
```java
import java.util.ArrayList; // import the ArrayList class

ArrayList<String> cars = new ArrayList<String>(); // Create an ArrayList object
```

### <span style="color: #ff5545;text-transform: capitalize;">Add packages</span>
The `ArrayList` class has many useful methods. For example, to add elements to the `ArrayList`, use the `add()` method
```ad-example
```java
import java.util.ArrayList;

public class Main {
  public static void main(String[] args) {
    ArrayList<String> cars = new ArrayList<String>();
    cars.add("Volvo");
    cars.add("BMW");
    cars.add("Ford");
    cars.add("Mazda");
    System.out.println(cars);
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">access an item</span>

## Reference