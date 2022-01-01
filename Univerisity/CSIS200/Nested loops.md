---
author: aboude
---
# Nested loops
___

Created on: 2021-12-11-16:25
Last modified: 2021-12-11-16:25

___

### <span style="color: #ff5545;text-transform: capitalize;">what are nested loops</span>

Nested loops are [[Loops|loops]] within [[Loops|loops]].

```ad-example
```java
for(int i = 1; i <= 30; i++){
	for(int j = (i-1)*10; j <= i*10; j++){
		System.out.print(j + " ");
	}
	System.out.println()
}
// outputs
// 0 1 2 3 4 5 6 7 8 9 10
// 10 11 12 13 14 15 16 17 18 19 20
// 20 21 22 23 24 25 26 27 28 29 30
```

## Relevant 
[[Loops]]