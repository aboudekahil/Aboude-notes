---
author: aboude
---
# Numbers
---

Created on: 2021-12-05-15:42
Last modified: 2021-12-05-15:42

---
### <span style="color: #ff5545;text-transform: capitalize;">how are numbers used in java?</span>
Primitive number [[Variable types|types]] are divided into two groups:

**Integer types** stores whole numbers, positive or negative (such as 123 or -456), without decimals. Valid types are `byte`, `short`, `int` and `long`. Which type you should use, depends on the numeric value.

>$$\text{Integer types} \in \mathbb{N}$$

**Floating point types** represents numbers with a fractional part, containing one or more decimals. There are two types: `float` and `double`.
> $$\text{Floating point types} \in \mathbb{R}$$

### <span style="color: #ff5545;text-transform: capitalize;">Integer types.</span>
```ad-example
title:Byte:
```java
byte myNum = 100;
```
```ad-example
title:Short:
```java
short myNum = 5000;
```
```ad-example
title:Int:
```java
int myNum = 100000;
```
```ad-example
title:Long:
```java
long myNum = 15000000000L;
```
```ad-note
* the `int` data type is the preferred data type when we create variables with a numeric value.
* when using a long value you should end the number with an `L` i.e `4000L`
```

### <span style="color: #ff5545;text-transform: capitalize;">Floating point types.</span>
```ad-example
title: Float:
```java
float myNum = 5.75f;
```
```ad-example
title: Double:
```java
double myNum = 19.99;
```

```ad-note
* `Double` is the preffered floating point type
* When using `float` you should end the number with an `f` i.e `40.5f`
```
 ```ad-note
title:A floating point number can also be a scientific number with an "e" to indicate the power of 10:
```java
float f1 = 35e3f; //35000.0
double d1 = 12E4; //120000.0
```

## Relevant:
[[Variables]] | [[Variable types]] | [[Type Casting]]