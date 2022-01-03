---
author: aboude
---
# Wrapper classes
___

Created on: 2022-01-03-15:54
Last modified: 2022-01-03-15:54

___
### <span style="color: #ff5545;text-transform: capitalize;">What are wrapper classes?</span>
Wrapper [[Classes and Objects|classes]] provide a way to use primitive [[Variable types|data types]] (`int`, `[[Booleans|boolean]]`, etc..) as [[Classes and Objects|objects]].

The table below shows the primitive type and the equivalent wrapper [[Classes and Objects|class]]:

| Primitive data type | Wrapper Class |
|:-------------------:|:-------------:|
|        byte         |     Byte      |
|        short        |     Short     |
|         int         |    Integer    |
|        long         |     Long      |
|        float        |     Float     |
|       double        |    Double     |
|       boolean       |    Boolean    |
|        char         |   Character   |

Sometimes you must use wrapper [[Classes and Objects|classes]], for example when working with Collection [[Classes and Objects|objects]], such as [[ArrayList]], where primitive types cannot be used (the list can only store [[Classes and Objects|objects]]):
```ad-Dont
```java
ArrayList<int> myNumbers = new ArrayList<int>(); // Invalid
```
```ad-Do
```java
ArrayList<Integer> myNumbers = new ArrayList<Integer>(); // Valid
```

### <span style="color: #ff5545;text-transform: capitalize;">Creating wrapper objects</span>
To create a wrapper [[Classes and Objects|object]], use the wrapper [[Classes and Objects|class]] instead of the primitive type. To get the value, you can just print the [[Classes and Objects|object]]

```ad-example
```java
public class Main {
  public static void main(String[] args) {
    Integer myInt = 5;
    Double myDouble = 5.99;
    Character myChar = 'A';
    System.out.println(myInt); // 5
    System.out.println(myDouble); // 5.99
    System.out.println(myChar); // A
  }
}
```

Since you're now working with [[Classes and Objects|objects]], you can use certain [[methods]] to get information about the specific [[Classes and Objects|object]].

For example, the following [[methods]] are used to get the value associated with the corresponding wrapper [[Classes and Objects|object]]: `intValue()`, `byteValue()`, `shortValue()`, `longValue()`, `floatValue()`, `doubleValue()`, `charValue()`, `booleanValue()`.

```ad-example
```java
public class Main {
  public static void main(String[] args) {
    Integer myInt = 5;
    Double myDouble = 5.99;
    Character myChar = 'A';
    System.out.println(myInt.intValue()); // 5
    System.out.println(myDouble.doubleValue()); // 5.99
    System.out.println(myChar.charValue()); // A
  }
}
```

Another useful method is the `toString()` method, which is used to convert wrapper [[Classes and Objects|objects]] to [[strings]].

```ad-example
In the following example, we convert an `Integer` to a `String`, and use the `length()` method of the `String` [[Classes and Objects|class]] to output the length of the "string"
```java
public class Main {
  public static void main(String[] args) {
    Integer myInt = 100;
    String myString = myInt.toString();
    System.out.println(myString.length());
  }
}
```

## Reference
[[Classes and Objects]] | [[Variable types]] | [[ArrayList]] | [[Methods]] | [[Strings]] | [[Booleans]]