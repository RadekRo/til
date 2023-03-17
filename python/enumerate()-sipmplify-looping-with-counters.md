# enumerate() - simplify looping with counters

Let's say that you need to print all the indexes of the iterable object. You can do this as follows:
```
values = ["a", "b", "c"]
index = 0
for value un values:
    print(index, value)
    index += 1

Output:
0 a
1 b
2 c```
but there is a better and less erroneous way to do so. Here comes the enumerate():
```
values = ["a", "b", "c"]
for index, value in enumerate(values):
    print(index, value)

Output:
0 a
1 b
2 c```
enumerate() function let's you to not only interate thru the object but also following the current index.\n
That would create more stabilized and less erroneous code with no need of increment any auxiliary variable.

---
_Last update: 17 Mar 2023_ 