# indexOf() 
#### return more than just first found index

__Syntax:__

`array.indexOf(searchElement[, fromIndex = 0]);`

Basically indexOf() returns first index of a passed element or -1 if the element
isn't found. You can choose from which element to start passing fromIndex value.

__Example:__

```
fruits = ['banana', 'orange', 'mango', 'kiwi', 'apple'];
fruits.indexOf('banana', [1]) // Returns -1 because banana has index[0].
fruits.indexOf('banana', [6]) // Returns -1 because array has only [0]-[4] indexes.
fruits.indexOf('banana') // Default: starts from [0], returns: 0
fruits.indexOf('banana', [0]) // Returns: 0
fruits.indexOf('banana', [-2]) // Returns: -1. Search starting index is [3].
``` 

What about the situation when we have more than just one the same element in array
and we would like to receive indexes of all of them?

__Solution:__

```
ourArray = [1, 2, 3, 4, 2, 0, 9, 8, 2];

indices=[];  // Builds an empty array fot indexes
idx = ourArray.indexOf(2) // we are searching for index of '2' starting with deafault [0]
while (idx != -1) {  // until reached -1 as a result 
  indices.push(idx); // push the index to indices array
  idx = ourArray.indexOf(2, idx + 1); // upgrade searching index start by 1 
}

Finally we will have an array called indices with all the founded indexes of 
number 2.

indices=[1, 4, 8];
```
---
_Last update: 10 Mar 2018_ 

