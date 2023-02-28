# inverting the dictionary

To invert pair key: value to value: key:
```
dict1={‘a’: 1, ‘b’: 2,‘c’: 3,‘d’: 4,‘e’: 5,‘f’: 6, ‘g’: 7}
dict2={v: k for k, v in dict1.items()}
print(dict2)
```
Output: `{1: ‘a’, 2: ‘b’, 3: ‘c’, 4: ‘d’, 5: ‘e’, 6: ‘f’, 7: ‘g’}`

---
_Last update: 28 February 2023_