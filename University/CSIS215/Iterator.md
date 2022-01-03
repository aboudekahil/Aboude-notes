---
author: aboude
---
# Iterator
___

Created on: 2022-01-03-20:49
Last modified: 2022-01-03-20:49

___

### <span style="color: #ff5545;text-transform: capitalize;">what is an iterator?</span>
An `Iterator` is an [[Classes and Objects|object]] that can be used to loop through collections, like [[ArrayList]] and HashSet. It is called an "iterator" because "iterating" is the technical term for looping.

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
To loop through a collection, use the `hasNext()` and `next()` [[methods]] of the `Iterator`:
```ad-example
```java
while(it.hasNext()) {
  System.out.println(it.next());
}
```

### <span style="color: #ff5545;text-transform: capitalize;">removing items from a collection</span>
Iterators are designed to easily change the collections that they loop through. The `remove()` method can remove items from a collection while looping.

```ad-example
Use an iterator to remove [[numbers]] less than 10 from a collection
```java
import java.util.ArrayList;
import java.util.Iterator;

public class Main {
  public static void main(String[] args) {
    ArrayList<Integer> numbers = new ArrayList<Integer>();
    numbers.add(12);
    numbers.add(8);
    numbers.add(2);
    numbers.add(23);
    Iterator<Integer> it = numbers.iterator();
    while(it.hasNext()) {
      Integer i = it.next();
      if(i < 10) {
        it.remove();
      }
    }
    System.out.println(numbers);
  }
}
```

```ad-note
Trying to remove items using a **for loop** or a **for-each loop** would not work correctly because the collection is changing size at the same time that the code is trying to loop.
```

## Reference
[[Classes and Objects]] | [[ArrayList]] | [[Methods]] | [[Numbers]]