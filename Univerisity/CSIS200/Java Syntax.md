---
author: aboude
---
# Java Syntax
---

Created on: 2021-12-05-13:43
Last Modified: 2021-12-05-13:43

---

### <span style="color: #ff5545;text-transform: capitalize;">A Basic Java Program</span>

```Java
public class Main {
  public static void main(String[] args) {
    System.out.println("Hello World");
  }
}
```

Every line of code that runs in Java must be inside a **[[Classes and Objects|class]]**. In our example, we named the class **<span style="color:#d76060">Main</span>**. 

```ad-warning
* A class should always start with an uppercase first letter.

* The name of the java file **<span style="color:#d76060">must match</span>** the class name. When saving the file, save it using the class name and add ".java" to the end of the filename.
```


### <span style="color: #ff5545;text-transform: capitalize;">the main method </span>
The `main()` [[Methods|method]] is **<span style="color:#d76060">REQUIRED</span>** and you will see it in every Java program:
```java
public static void main(String[] args)
```

Any code inside the `main()` method will be executed.

### <span style="color: #ff5545;text-transform: capitalize;">println()	</span>
Inside the `main()` [[Methods|method]], we can use the `println()` method to print a line of text to the screen:

```java
public static void main(String[] args) {
  System.out.println("Hello World");
}
```

```ad-note
* The curly braces `{}` marks the beginning and the end of a block of code.

* Each code statement must end with a semicolon.
```

## Relevant:
[[Classes and Objects]] | [[Methods]]