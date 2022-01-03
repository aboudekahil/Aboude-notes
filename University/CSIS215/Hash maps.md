---
author: aboude
---

# Hash maps
___

Created on: 2022-01-03-21:01
Last modified: 2022-01-03-21:01

___

### <span style="color: #ff5545;text-transform: capitalize;">what are hashMaps</span>
Arrays store items as an ordered collection, and you have to access them with an index number (`int` type). A `HashMap` however, store items in "**key**/**value**" pairs, and you can access them by an index of another type (e.g. a `String`).

One object is used as a key (index) to another object (value). It can store different types: `String` keys and `Integer` values, or the same type, like: `String` keys and `String` values:

```ad-example
Create a `HashMap` object called **capitalCities** that will store `String` **keys** and `String` **values**
```java
import java.util.HashMap; // import the HashMap class

HashMap<String, String> capitalCities = new HashMap<String, String>();
```

### <span style="color: #ff5545;text-transform: capitalize;">add items</span>
The `HashMap` class has many useful methods. For example, to add items to it, use the `put()` method

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



## Reference