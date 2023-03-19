# several ways to get a list from dictionary

#### Starting dictionary:
```
a = {"a": 1, "b": 2, "c": 3, "d": 4}
```
#### List of tuples:
```
b = list(a.items())
```
Output: [('a', 1), ('b', 2), ('c', 3), ('d', 4)]
#### List of tuples:
```
c = list(zip(a.keys(), a.values()))
```
Output: [('a', 1), ('b', 2), ('c', 3), ('d', 4)]
#### List of lists:
```
d = [[k, v] for k, v in a.items()]
```
Output: [['a', 1], ['b', 2], ['c', 3], ['d', 4]]

---
_Last update: 19 Mar 2023_ 