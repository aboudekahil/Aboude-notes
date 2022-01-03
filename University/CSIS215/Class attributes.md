---
author: aboude
---
# Class attributes
___

Created on: 2022-01-03-11:56
Last modified: 2022-01-03-11:56

___

```ad-note
Another term for class attributes is **fields**
```

### <span style="color: #ff5545;text-transform: capitalize;">What are attributes?</span>
Class attributes are **values which are owned by the class itself**. They will be shared by all the instances of the class. Therefore they have the same value for every instance. We define class attributes outside all the methods, usually they are placed at the top, right below the class header.

```ad-example
x and y are attributes of the class `Main`
```java
public class Main {
  int x = 5;
  int y = 3;
}
```

### <span style="color: #ff5545;text-transform: capitalize;">Accessing attributes</span>
You can access attributes by creating an object of the class, and by using the dot syntax (`.`):

```ad-example
```java
public class Main {
  int x = 5;

  public static void main(String[] args) {
    Main myObj = new Main();
    System.out.println(myObj.x);
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">Modifying attributes</span>
You can modify attributes by using the assignment operator (`=`)
```ad-example
```java
public class Main {
  int x;

  public static void main(String[] args) {
    Main myObj = new Main();
    myObj.x = 40;
    System.out.println(myObj.x); // prints 40
  }
}
```

or override attributes
```ad-example
```java
public class Main {
  int x = 10;

  public static void main(String[] args) {
    Main myObj = new Main();
    myObj.x = 25; // x is now 25
    System.out.println(myObj.x);
  }
}
```

If you don't want the ability to override existing values, use the `final` [[Modifiers|modifier]]:

```ad-example
```java
public class Main {
  final int x = 10;

  public static void main(String[] args) {
    Main myObj = new Main();
    myObj.x = 25; // will generate an error: cannot assign a value to a final variable
    System.out.println(myObj.x);
  }
}
```
## Reference