# *args and **kwargs function parameters

#### *args

Imagine you have a function which multiplies values:
```
def multiply_two_numbers(a, b):
    return a * b

multiply(2, 3) // Returns: 6
```
After a few lines of code you are in need of a function that multiplies three values.\
Another function?\
Not necessary. Let's transform the function above to make it more universal.
```
def multiply(*args):
    result = 1
    for i in args:
        result *= i
    return result

multiply(2, 3, 4) // Returns: 24
multiply(1, 5, 6, 10) // Returns: 300
```
*args creates a tuple of arguments passed to the function ```(2, 3, 4), (1, 5, 6, 10)```

#### **kwargs

What about keywords arguments?
```multiply(a = 4, 3, 4) // Return: SyntaxError: positional argument follows keyword argument```
Here comes the **kwarg argument!\
Kwarg is a dictionary holding keypairs: keywords and it's argument.\
Let's modify our function to allow as passing not only simple arguments but also keyword aguments.\
Keep in mind that *args should __always__ be placed before **kwargs
```
def multiply(*args, **kwargs):
    result = 1
    for i in args:
        result *= i
    for j in kwargs:
        result *= kwargs[j]
    return result

multiply(3, 4, a = 4) // Returns: 48
```

Argument unpacking is very commonly used in Python. Keep that in mind.

---
_Last update: 6 March 2023_
