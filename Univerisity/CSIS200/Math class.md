---
author: aboude
---
# The math class
___

Created on: 2021-12-07-19:31
Last modified: 2021-12-07-19:31

___

### <span style="color: #ff5545;text-transform: capitalize;">What is the math class?</span>

The Java Math [[Classes|class]] has many [[Methods|methods]] that allows you to perform mathematical tasks on [[Numbers]].

```ad-warning
When using the math class be sure to write `Math` with the `M`  capitalized. 
```
___
### <span style="color: #ff5545;">Math.max(x,y)</span>
The `Math.max(x,y)` method can be used to find the highest value between _x_ and _y_.
```ad-example
```java
Math.max(5, 10); // returns 10
```
___
### <span style="color: #ff5545;">Math.min(x,y)</span>
The `Math.min(x,y)` method can be used to find the smallest value between _x_ and _y_.
```ad-example
```java
Math.min(5, 10);
```
___
### <span style="color: #ff5545;">Math.abs(x)</span>
The `Math.abs(x)` method returns the absolute (positive<span style="color:18a05e">`fas:Plus`</span>) value of _x_.
```ad-example
```java
Math.abs(-4.7);
```
___
### <span style="color: #ff5545;">Math.random()</span>
`Math.random()` returns a random [[Numbers|number]] between 0.0 (inclusive), and 1.0 (exclusive).
```ad-example
```java
Math.random();
```
To get more control over the random number, e.g. you only want a random number between 0 and 100, you can use the following formula:
```ad-example
```java
int randomNum = (int)(Math.random() * 101);  // 0 to 100
```

## Relevant 
[[Numbers]] | [[Classes]] | [[Methods]]