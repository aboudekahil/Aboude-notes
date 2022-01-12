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

```ad-Dont
title: Before
```javascript
async function boot(){
	const user = await fetch('api.randomuser.me');
	
	console.log(user);
}

boot()
```

```ad-example
title: After
```javascript
const user = await fetch('api.randomuser.me');

console.log(user);
```

## Reference