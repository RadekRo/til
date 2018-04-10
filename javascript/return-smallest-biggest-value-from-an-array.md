# Return smallest/biggest value from an array

The easiest way to return a smallest od biggest value from an array is using a 
combination of `concat` and `Math.max`, `Math.min`.

__Example:__

```markdown
a = [1, 2, 3, -10, 0]

function findSmallestNum(arr) {
return Math.min(...arr)
}

function findBiggestNum(arr) {
return Math.max(...arr)
}

findSmallestNum(a) // returns: -10
findBiggestNum(a) // returns: 3

```
 
---
_Last update: 10 Apr 2018_ 