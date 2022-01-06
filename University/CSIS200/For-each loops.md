---
author: aboude
---
# For each loop
___

Created on: 2021-12-07-21:04
Last modified: 2021-12-08-12:46

___

### <span style="color: #ff5545;text-transform: capitalize;">What are for each loops?</span>
For each [[loops]] are simplified [[For loops|for loops]] used specifically to iterate through [[Arrays|arrays]]. They give the benefit of being easier to write and read, in addition to iterate through an [[Arrays|array]] without having to track a counter.

```ad-example
title:Syntax
```java
for(type name: array_name){

}
```
___

```ad-example
```java
String[] names = new String[3] {"Sasha", "Levi", "Erwin"};

for(String name: names){
	System.out.println(name);
}
// prints all the names inside names one by one
```

In the example above we iterate through the `names` array without using a counter.

## Relevant 
[[For loops]] | [[Loops]] | [[Break-Continue]] | [[Arrays]] | [[Java Syntax]]