---
author: aboude
---
# Inner classes
___

Created on: 2022-01-03-16:41
Last modified: 2022-01-03-16:41

___

### <span style="color: #ff5545;text-transform: capitalize;">What’s an inner class?</span>
In Java, it is also possible to nest [[Classes and Objects|classes]] (a [[Classes and Objects|class]] within a [[Classes and Objects|class]]). The purpose of nested [[Classes and Objects|classes]] is to group [[Classes and Objects|classes]] that belong together, which makes your code more readable and maintainable.

To access the inner [[Classes and Objects|class]], create an [[Classes and Objects|object]] of the outer [[Classes and Objects|class]], and then create an [[Classes and Objects|object]] of the inner [[Classes and Objects|class]]

```ad-example
```java
class OuterClass {
  int x = 10;

  class InnerClass {
    int y = 5;
  }
}

public class Main {
  public static void main(String[] args) {
    OuterClass myOuter = new OuterClass();
    OuterClass.InnerClass myInner = myOuter.new InnerClass();
    System.out.println(myInner.y + myOuter.x);
  }
}

// Outputs 15 (5 + 10)
```

### <span style="color: #ff5545;text-transform: capitalize;">private inner class</span>
Unlike a "regular" [[Classes and Objects|class]], an inner [[Classes and Objects|class]] can be `private` or `protected`. If you don't want outside [[Classes and Objects|objects]] to access the inner [[Classes and Objects|class]], declare the [[Classes and Objects|class]] as `private`:
```ad-example
```java
class OuterClass {
  int x = 10;

  private class InnerClass {
    int y = 5;
  }
}

public class Main {
  public static void main(String[] args) {
    OuterClass myOuter = new OuterClass();
    OuterClass.InnerClass myInner = myOuter.new InnerClass();
    System.out.println(myInner.y + myOuter.x);
  }
}
// If you try to access a private inner class from an outside class, an error occurs
```

### <span style="color: #ff5545;text-transform: capitalize;">Static inner class</span>
An inner [[Classes and Objects|class]] can also be `static`, which means that you can access it without creating an [[Classes and Objects|object]] of the outer [[Classes and Objects|class]]:
```ad-example
```java
class OuterClass {
  int x = 10;

  static class InnerClass {
    int y = 5;
  }
}

public class Main {
  public static void main(String[] args) {
    OuterClass.InnerClass myInner = new OuterClass.InnerClass();
    System.out.println(myInner.y);
  }
}

// Outputs 5
```
```ad-note
just like `static` [[Class attributes|attributes]] and methods, a `static` inner class does not have access to members of the outer class.
```

## Reference