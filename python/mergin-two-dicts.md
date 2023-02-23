# mergin two dictionaries 

Using `z = {**x **y}` you can easily merge two dicts together. 

__Example:__

```
a = {"a": 1, "b": 2, "c": 1}
b = {"a": 2, "d": 3, "e": 2}
z = {**a, **b}
```
// Returns:
// z = {"a": 2, "b": 2, "c": 1, "d": 3, "e": 2}
// Notice than if a key will reapet itself in the next merged dict it will be overwritten!

---
_Last update: 23 Feb 2023_ 