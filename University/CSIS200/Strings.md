---
author: aboude
---
# Strings
---

Created on: 2021-12-05-23:31
Last modified: 2021-12-05-23:31

---

### <span style="color: #ff5545;text-transform: capitalize;">What are strings?</span>
Strings are used for storing text.

A `String` [[Variables|variable]] contains a collection of [[Characters|characters]] surrounded by double quotes

```ad-example
```java
String greeting = "Hello";
```

### <span style="color: #ff5545;text-transform: capitalize;">String length.</span>
A String in Java is actually an object, which contain [[Methods|methods]] that can perform certain operations on strings. For example, the length of a string can be found with the `length()` [[Methods|method]].
```ad-example
```java
String txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
System.out.println("The length of the txt string is: " + txt.length());
```

### <span style="color: #ff5545;text-transform: capitalize;">String concatenation.</span>
The `+` [[Operators|operator]] can be used between strings to combine them. This is called **concatenation**.

```ad-example
```java
String firstName = "John";
String lastName = "Doe";
System.out.println(firstName + " " + lastName); 
//prints "John Doe"
```

```ad-note
title: If you add a number and a string, the result will be a string concatenation:
```java
String x = "10";
int y = 20;
String z = x + y;   // z will be 1020 (a String)
```

### <span style="color: #ff5545;text-transform: capitalize;">Special Characters</span>

Because strings must be written within quotes, Java will misunderstand this string, and generate an error:

```ad-warning
title: This will give an error
```java
String txt = "We are the so-called "Vikings" from the north.";
```

The solution to avoid this problem, is to use the **backslash escape character**.

The backslash (`\`) escape character turns special characters into string characters:

| Escape charcacter | Result          | Description   |
| ----------------- | --------------- | ------------- |
| \\'               | '               | Single quote  |
| \\"               | "               | Double quotes |
| \\\\              | \               | Backslash     |
| \n                | New line        |               |
| \r                | Carriage return |               |
| \t                | tab             |               |

```ad-example
```java
String txt = "We are the so-called \"Vikings\" from the north.";
```

### <span style="color: #ff5545;">.charAt()</span>

You can use the charAt() [[Methods|method]] to get a [[Characters|character]] at specific location inside a string.

```ad-example
```java
char a = "I'm aboude".charAt(4); // a = 'a'
```
```ad-note
Java counts positions from zero.  
0 is the first position in a string, 1 is the second, 2 is the third ...
```

## Relevant:
[[Characters]] | [[Variable types]] | [[Methods]] | [[Operators]]