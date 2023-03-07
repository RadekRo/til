# f-string

It is a common practice to add variables inside strings. F strings are by far the coolest way of doing it.\
To appreciate the f strings more, let’s first perform the operation with the format function.
```
name = 'John'
age = 15
print("{} is {} years old".format(name, age))
John is 15 years old
```
We specify the variables that go inside the curly braces by using the format function at the end.\ 
F strings allow for specifying the variables inside the string.
```
print(f"{name} is {age} years old")
John is 15 years old
```
F strings are easier to follow and type. Moreover, they make the code more readable.

Thanks to __Soner Yildirim__ and his 6 Python's Tricks article (_https://towardsdatascience.com/6-cool-python-tricks-you-should-know-bab1b6a42446_)

---
_Last update: 6 March 2023_
