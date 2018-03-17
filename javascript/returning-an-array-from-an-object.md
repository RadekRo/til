# object.keys/values/entries() 
#### returning an array from an object

If you would like to return an array from an object you can use one of three
avaliable methods:

* `Object.key(obj)` - returns an array of an `obj` keys.
* `Object.values(obj)` - returns an array of an `obj` values.
* `Object.entries(obj)` - returns an array of an `obj` where each key and value
is holded in a separated array.

__Example:__

```
myObject = { a: 1, b: 2, c: 3 }

Object.keys(myObject) // returns an array ["a", "b", "c"]
Object.values(myObject) // returns an array [1, 2, 3]
Object.entries(myObject) // returns an array of arrays [ ["a", 1], ["b", 2], ["c", 3] ]
```

---
_Last update: 17 Mar 2018_ 

```