---
author: aboude
---
# Iterator
___

Created on: 2022-01-03-20:49
Last modified: 2022-01-03-20:49

___

### <span style="color: #ff5545;text-transform: capitalize;">what is an iterator?</span>
An `Iterator` is an object that can be used to loop through collections, like ArrayList and HashSet. It is called an "iterator" because "iterating" is the technical term for looping.

To use an Iterator, you must import it from the `java.util` package.

### <span style="color: #ff5545;text-transform: capitalize;">getting an iterator</span>
The `iterator()` method can be used to get an `Iterator` for any collection

```ad-example
```java
// Import the ArrayList class and the Iterator class
import java.util.ArrayList;
import java.util.Iterator;

public class Main {
  public static void main(String[] args) {

    // Make a collection
    ArrayList<String> cars = new ArrayList<String>();
    cars.add("Volvo");
    cars.add("BMW");
    cars.add("Ford");
    cars.add("Mazda");

    // Get the iterator
    Iterator<String> it = cars.iterator();

    // Print the first item
    System.out.println(it.next());
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">looping through a collection</span>
To loop through a collection, use the `hasNext()` and `next()` methods of the `Iterator`:
```ad-exam
```java
while(it.hasNext()) {
  System.out.println(it.next());
}
```
## Reference