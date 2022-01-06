---
author: aboude
---
# Variables
---

Created on: 2021-12-04-19:57
Last Modified: 2021-12-05-22:55

---

## What are variables?
Variables are like a storage tool used in programming languages to store different values that we may want to use later. They are used inside [[Methods|methods]] and [[Classes and Objects|classes]]

---

## How are variables used?

* #### <span style="color: #ff5545;text-transform: capitalize;">Variable declaration. </span>
	Before we use a variable we need to declare it. 

	We declare a variable by writing its [[Variable types|type]] first then the name of said variable.

	```ad-warning
	Variable names **MUST** adhere to [[Identifiers|identidier]] rules
	```

	```ad-example
	```java
	int x;
	float y;
	String word;
	```````
	
	> x here is an integer $$\text{x} \in \mathbb{N}$$
	y is a real number $$\text{y} \in \mathbb{R}$$
	and word is basically text

	```ad-note
	title:Note: You can declare multiple variables at once like so:
	```java
	int x = 5, y = 6, z = 50;
	```
* #### <span style="color: #ff5545;text-transform: capitalize;">Variable assigning.</span>

	To assign a variable we use the ``=`` [[Operators|operator]] 
	```ad-example
	```Java
	x = 4;
	y = 5.5f;
	word = "Hello world!";
	``````




* #### <span style="color: #ff5545;text-transform: capitalize;"> Combining declaration and assigning </span>
	We can declare and assign a value in one line by doing the following:
	```Java
	int x = 4;
	float y = 4.3f;
	String word = "Hello World!";
	```

* #### <span style="color: #ff5545;text-transform: capitalize;"> Constants </span>
	Constants are [[Variables|variables]] that we assign only **<span style="color:#d76060">once</span>**, we **<span style="color:#d76060">cannot</span>** change its value after the first time.
	
	We declare a constant by using the **final** keyword.
	```ad-example
	```Java
	final int x = 4;
	final float y = 4.4f;
	final String word = "Hello World!"
	``````

---
## Relevant:
[[Identifiers]] | [[Operators]] | [[Variable types]]