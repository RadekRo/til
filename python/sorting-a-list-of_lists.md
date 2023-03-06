# sorting a list of lists

Consider we have a list of lists.
```lst = [[2, 7], [7, 3], [3, 8], [8, 7], [9, 7], [4, 9]]```
We can sort the list based on the first or second items of the inner lists by using the sort function with a lambda function.
```lst.sort(key = lambda inner:inner[1])
print(lst)
[[7, 3], [2, 7], [8, 7], [9, 7], [3, 8], [4, 9]]```
The list is sorted based on the second items. We can do the same with the first items just by changing the 1 to 0.
```lst.sort(key = lambda inner:inner[0])
print(lst)
[[2, 7], [3, 8], [4, 9], [7, 3], [8, 7], [9, 7]]```

Thanks to __Soner Yildirim__ and his 6 Python's Tricks article (_https://towardsdatascience.com/6-cool-python-tricks-you-should-know-bab1b6a42446_)

---
_Last update: 6 March 2023_