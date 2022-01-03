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

## Reference