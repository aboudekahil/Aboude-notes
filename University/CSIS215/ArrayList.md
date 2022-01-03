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
To access an element in the `ArrayList`, use the `get()` method and refer to the index number
```ad-example
```java
cars.get(0);
```

### <span style="color: #ff5545;text-transform: capitalize;">change and item</span>
To modify an element, use the `set()` method and refer to the index number

```ad-example
```java
cars.set(0, "Opel");
```

### <span style="color: #ff5545;text-transform: capitalize;">Remove an item</span>
To remove an element, use the `remove()` method and refer to the index number:
```ad-example
```java
cars.remove(0);
```
To remove all the elements in the `ArrayList`, use the `clear()` method
```ad-example
```java
cars.clear();
```
### <span style="color: #ff5545;text-transform: capitalize;">arrayList size</span>
To find out how many elements an ArrayList have, use the `size` method
```ad-example
```java
cars.size();
```
### <span style="color: #ff5545;text-transform: capitalize;">loop through an array list</span>
Loop through the elements of an `ArrayList` with a `for` loop, and use the `size()` method to specify how many times the loop should run
```ad-example
```java
public class Main {
  public static void main(String[] args) {
    ArrayList<String> cars = new ArrayList<String>();
    cars.add("Volvo");
    cars.add("BMW");
    cars.add("Ford");
    cars.add("Mazda");
    for (int i = 0; i < cars.size(); i++) {
      System.out.println(cars.get(i));
    }
  }
}
```

You can also loop through an `ArrayList` with the **for-each** loop

```ad-example
```java
public class Main {
  public static void main(String[] args) {
    ArrayList<String> cars = new ArrayList<String>();
    cars.add("Volvo");
    cars.add("BMW");
    cars.add("Ford");
    cars.add("Mazda");
    for (String i : cars) {
      System.out.println(i);
    }
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">other types</span>
Elements in an ArrayList are actually objects. In the examples above, we created elements (objects) of type "String". Remember that a String in Java is an object (not a primitive type). To use other types, such as int, you must specify an equivalent wrapper class: `Integer`. For other primitive types, use: `Boolean` for boolean, `Character` for char, `Double` for double, etc

```ad-example
```java
import java.util.ArrayList;

public class Main {
  public static void main(String[] args) {
    ArrayList<Integer> myNumbers = new ArrayList<Integer>();
    myNumbers.add(10);
    myNumbers.add(15);
    myNumbers.add(20);
    myNumbers.add(25);
    for (int i : myNumbers) {
      System.out.println(i);
    }
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">sort an arrayList</span>

## Reference