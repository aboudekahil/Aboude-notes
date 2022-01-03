---
author: aboude
---
# Wrapper classes
___

Created on: 2022-01-03-15:54
Last modified: 2022-01-03-15:54

___
### <span style="color: #ff5545;text-transform: capitalize;">What are wrapper classes?</span>
Wrapper classes provide a way to use primitive data types (`int`, `boolean`, etc..) as objects.

The table below shows the primitive type and the equivalent wrapper class:

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

Sometimes you must use wrapper classes, for example when working with Collection objects, such as `ArrayList`, where primitive types cannot be used (the list can only store objects):
```ad-Dont
```java
ArrayList<int> myNumbers = new ArrayList<int>(); // Invalid
```
```ad-Do
```java
ArrayList<Integer> myNumbers = new ArrayList<Integer>(); // Valid
```

## Reference