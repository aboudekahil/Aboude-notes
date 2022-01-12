---
aliases: [ES2022]
author: aboude
---
# Everything new in ES2022
___

Created on: 2022-01-12-17:51
Last modified: 2022-01-12-17:51

___

### <span style="color: #ff5545;text-transform: capitalize;">Top level await</span>
When using async await functionality in javascript you can now use the await keyword outside an asynchrenous function.

```ad-definition
title: Before
```javascript
async function boot(){
	const user = await fetch('api.randomuser.me');
	
	console.log(user);
}

boot()
```

```ad-definition
title: After
```javascript
const user = await fetch('api.randomuser.me');

console.log(user);
```

### <span style="color: #ff5545;text-transform: capitalize;">.at() array method</span>
In javascript you can’t use negative array indices with the bracket syntax because of how objects in javascript are made, instead you would have to use the .length property to count from the last index.

Now with .at() method you can get any element using positive and negative indicies.

```ad-example
```javascript
let arr = [0, 1, 2, 3, 4, 5, 6];

arr[4] // returns 4
arr.at(4) // returns 4

arr[-2] //returns an error
arr[arr.length - 2] // returns 5
arr.at(-2) // returns 5
```

### <span style="color: #ff5545;text-transform: capitalize;">Object.hasOwn()</span>

In JavaScript there already exists an `Object.prototype.hasOwnProperty` but, as the MDN documentation also suggests, it’s best to not use hasOwnProperty outside the prototype itself as it is not a protected property, meaning that an object could have its property called `hasOwnProperty` that has nothing to do with `Object.prototype.hasOwnProperty`.

## Reference