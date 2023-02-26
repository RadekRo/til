# cloning a list without aliasing

When you are cloning a list by just assigning it to another variable, like this:
```
a = [1, 2, 3, 4]
b = a
print(b)
```
Output: `[1, 2, 3, 4]`\
You are not making an individual clone of the list. You are just making another instance of the same object.\
That means that any change to the first or second list will cause the changes in the other.
```
a[2] = 5
print(a) -> [1, 2, 5, 4]
print(b) -> [1, 2, 5, 4] !!
```
The quickiest way to avoid such a situation is to create a clone by leverage slicing:
```
b = a[:]
```
You've just created a separate instance which means there is no more straightforward connection between a and b.

Tricky!

---
_Last update: 26 Feb 2023_ 