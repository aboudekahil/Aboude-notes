---
author: aboude
---

# Hash maps
___

Created on: 2022-01-03-21:01
Last modified: 2022-01-03-21:01

___

### <span style="color: #ff5545;text-transform: capitalize;">what are hashMaps</span>
[[Arrays]] store items as an ordered collection, and you have to access them with an index number (`int` type). A `HashMap` however, store items in "**key**/**value**" pairs, and you can access them by an index of another type (e.g. a `String`).

One [[Classes and Objects|object]] is used as a key (index) to another [[Classes and Objects|object]] (value). It can store different types: `String` keys and `Integer` values, or the same type, like: `String` keys and `String` values:

```ad-example
Create a `HashMap` [[Classes and Objects|object]] called **capitalCities** that will store `String` **keys** and `String` **values**
```java
import java.util.HashMap; // import the HashMap class

HashMap<String, String> capitalCities = new HashMap<String, String>();
```

### <span style="color: #ff5545;text-transform: capitalize;">add items</span>
The `HashMap` [[Classes and Objects|class]] has many useful [[methods]]. For example, to add items to it, use the `put()` method

```ad-example
```java
// Import the HashMap class
import java.util.HashMap;

public class Main {
  public static void main(String[] args) {
    // Create a HashMap object called capitalCities
    HashMap<String, String> capitalCities = new HashMap<String, String>();

    // Add keys and values (Country, City)
    capitalCities.put("England", "London");
    capitalCities.put("Germany", "Berlin");
    capitalCities.put("Norway", "Oslo");
    capitalCities.put("USA", "Washington DC");
    System.out.println(capitalCities);
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">access an item</span>
To access a value in the `HashMap`, use the `get()` method and refer to its key

```ad-example
```java
capitalCities.get("England");
```

### <span style="color: #ff5545;text-transform: capitalize;">remove an item</span>

To remove an item, use the `remove()` method and refer to the key

```ad-example
```java
capitalCities.remove("England");
```

To remove all items, use the `clear()` method

```ad-example
```java
capitalCities.clear();
```

### <span style="color: #ff5545;text-transform: capitalize;">hashMap size</span>
To find out how many items there are, use the `size()` method

```ad-example
```java
capitalCities.size();
```

### <span style="color: #ff5545;text-transform: capitalize;">loop through a hashMap</span>

Loop through the items of a `HashMap` with a **for-each** loop.

```ad-note
Use the `keySet()` method if you only want the keys, and use the `values()` method if you only want the values
```

```ad-example
```java
// Print keys
for (String i : capitalCities.keySet()) {
  System.out.println(i);
}
```

```ad-example
```java
// Print values
for (String i : capitalCities.values()) {
  System.out.println(i);
}
```

```ad-example
```java
// Print keys and values
for (String i : capitalCities.keySet()) {
  System.out.println("key: " + i + " value: " + capitalCities.get(i));
}
```

### <span style="color: #ff5545;text-transform: capitalize;">other types</span>
Keys and values in a HashMap are actually [[Classes and Objects|objects]]. In the examples above, we used [[Classes and Objects|objects]] of type "String". Remember that a String in Java is an [[Classes and Objects|object]] (not a primitive type). To use other types, such as int, you must specify an equivalent [[Wrapper classes|wrapper]] [[Classes and Objects|class]]: `Integer`. For other [[Variable types|primitive types]], use: `Boolean` for boolean, `Character` for char, `Double` for double, etc

```ad-example
Create a `HashMap` [[Classes and Objects|object]] called **people** that will store `String` **keys** and `Integer` **values**
```java
// Import the HashMap class
import java.util.HashMap;

public class Main {
  public static void main(String[] args) {

    // Create a HashMap object called people
    HashMap<String, Integer> people = new HashMap<String, Integer>();


    // Add keys and values (Name, Age)
    people.put("John", 32);
    people.put("Steve", 30);
    people.put("Angie", 33);

    for (String i : people.keySet()) {
      System.out.println("key: " + i + " value: " + people.get(i));
    }
  }
}
```

## Reference
[[Arrays]] | [[Classes and Objects]] | [[Methods]] | [[Wrapper classes]] | [[Variable types]]