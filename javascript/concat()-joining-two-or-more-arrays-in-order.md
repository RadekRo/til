# concat() 
#### create a new array from the given arrays

Using `concat()` creates a new array of given arrays. It holds the order of the given
arrays holding the same values without changing it. 

__Example:__

```
const firstArray = [1, 2, 3, 'a', 'done'];
const secondArray = [5, 6, 7, 'a', 'failed'];
const thirdArray = firstArray.concat(secondArray);

// Returns:
// thirdArray = [1, 2, 3, 'a', 'done', 5, 6, 7, 'a', 'failed']

const firstArray = [1, 2, 3, 'a', 'done'];
const secondArray = [5, 6, 7, 'a', 'failed'];
const thirdArray = [7];
const fourthArray = firstArray.concat(secondArray, thirdArray);

// Returns:
// fourthArray = [1, 2, 3, 'a', 'done', 5, 6, 7, 'a', 'failed', 7];

```

__EcmaScript 6 (new!)__

EcmaScript 6 shortened `arr.concat()` to `[...arr]` which means that instead of `fourthArray = firstArray.
concat(secondArray, thirdArray)`, you can use a shorter `fourthArray = [...firstArray, ...secondArray, ...thirdArray]`
meaning exactly the same.

---
_Last update: 09 Mar 2018_ 

