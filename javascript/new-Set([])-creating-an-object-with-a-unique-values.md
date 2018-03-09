# new Set([]) 
#### creating an object with a unique values

Using `new Set([iterable])` creates __an object__ with a unique values. That means that 
if you pass a set of values to `new Set` and some of them will repeat itself - `new Set`
will create an object where all repeats will occur as one entry.

*iterable - means: able to be counted.*

__Example:__

```
const mySet = new Set([1, 2, 3, 4, 4, 5, 6, 6, 6]);

// Returns:
// mySet = {1, 2, 3, 4, 5, 6}.

const mySet = new Set();

// Returns an empty object, similar to: mySet = {};

const x = [1, 2, 3, 4, 5, 6, 7, 1, 2, 3, 4, 5, 6, 7, 8];
const mySet = new Set([...x]); // concat of x

// Returnes an object with 8 values.
// mySet = {1, 2, 3, 4, 5, 6, 7, 8}
```

__Warning:__ 

`NaN` in mySet is equal to `NaN` (NaN === NaN) however `NaN !== NaN` in JS.

---
_Last update: 09 Mar 2018_ 

