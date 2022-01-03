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
Create a `HashSet` [[Classes and Objects|object]] called **cars** that will store [[strings]]
```java
import java.util.HashSet; // Import the HashSet class

HashSet<String> cars = new HashSet<String>();
```

### <span style="color: #ff5545;text-transform: capitalize;">add items</span>
The `HashSet` [[Classes and Objects|class]] has many useful [[methods]]. For example, to add items to it, use the `add()` method

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

### <span style="color: #ff5545;text-transform: capitalize;">loop through a hashSet</span>
Loop through the items of an `HashSet` with a **for-each** loop

```ad-example
```java
for (String i : cars) {
  System.out.println(i);
}
```

### <span style="color: #ff5545;text-transform: capitalize;">other types</span>

Items in an HashSet are actually [[Classes and Objects|objects]]. In the examples above, we created items ([[Classes and Objects|objects]]) of type "String". Remember that a String in Java is an [[Classes and Objects|object]] (not a primitive type). To use other types, such as int, you must specify an equivalent wrapper [[Classes and Objects|class]]: `Integer`. For other primitive types, use: `Boolean` for boolean, `Character` for char, `Double` for double, etc

```ad-example
Use a `HashSet` that stores `Integer` objects
```java
import java.util.HashSet;

public class Main {
  public static void main(String[] args) {

    // Create a HashSet object called numbers
    HashSet<Integer> numbers = new HashSet<Integer>();

    // Add values to the set
    numbers.add(4);
    numbers.add(7);
    numbers.add(8);

    // Show which numbers between 1 and 10 are in the set
    for(int i = 1; i <= 10; i++) {
      if(numbers.contains(i)) {
        System.out.println(i + " was found in the set.");
      } else {
        System.out.println(i + " was not found in the set.");
      }
    }
  }
}
```

## Reference