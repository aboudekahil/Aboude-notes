---
author: aboude
---
# Characters
---

Created on: 2021-12-05-22:53
Last modified: 2021-12-05-22:53

---

### <span style="color: #ff5545;text-transform: capitalize;">What are characters?</span>
The `char` data [[Variable types|type]] is used to store a **<span style="color:#d76060"> single</span>** character. The character must be surrounded by single quotes, like `'A'` or `'c'`.

```ad-example
```java
char myGrade = 'B';
System.out.println(myGrade); //prints B
```

Alternatively, you can use ASCII/Unicode values to display certain characters:

```ad-example
```java
char myVar1 = 65, myVar2 = 66, myVar3 = '\u0067';
System.out.println(myVar1); //b
System.out.println(myVar2); //c
System.out.println(myVar3); //d
```

<iframe src="http://www.csc.villanova.edu/~tway/resources/ascii-table.html" width=1000 height=640>

## Relevant:
[[Strings]] | [[Variable types]]