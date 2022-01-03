---
author: aboude
---
# Hash set
___

Created on: 2022-01-03-23:26
Last modified: 2022-01-03-23:26

___

### <span style="color: #ff5545;text-transform: capitalize;">what is a hashSet</span>
A HashSet is a collection of items where every item is unique, and it is found in the `java.util` package

```ad-example
Create a `HashSet` object called **cars** that will store strings
```java
import java.util.HashSet; // Import the HashSet class

HashSet<String> cars = new HashSet<String>();
```

### <span style="color: #ff5545;text-transform: capitalize;">add items</span>
The `HashSet` class has many useful methods. For example, to add items to it, use the `add()` method

```ad-example
```java
// Import the HashSet class
import java.util.HashSet;

public class Main {
  public static void main(String[] args) {
    HashSet<String> cars = new HashSet<String>();
    cars.add("Volvo");
    cars.add("BMW");
    cars.add("Ford");
    cars.add("BMW");
    cars.add("Mazda");
    System.out.println(cars);
  }
}
```

```ad-note
 In the example above, even though BMW is added twice it only appears once in the set because every item in a set has to be unique
```

### <span style="color: #ff5545;text-transform: capitalize;">check if an item exists</span>
To check whether an item exists in a HashSet, use the `contains()` method

```ad-example
```java
cars.contains("Mazda");
```

### <span style="color: #ff5545;text-transform: capitalize;">remove an item</span>
To remove an item, use the `remove()` method
```ad-example
```java
cars.remove("Volvo");
```

To remove all items, use the `clear()` method

```ad-example
```java
cars.clear();
```

### <span style="color: #ff5545;text-transform: capitalize;">hashSet size</span>

To find out how many items there are, use the `size` method
```ad-example
```java
cars.size();
```

## Reference