# replacing single if without else statement

Consider situation where you want your program to do something only if something else will take place but you don't have any else statement.
```
a = 2
b = 3

if a < b:
    print(a)
else:
    None

or

if a < b:
    print(a) // without else! which is truly a bad habit
```
You can of course do something like above but it doesn't look pretty, isn't it?\
In such case you can use `and` expression which can easily validate if your code should or shouldn't be omitted.
```
a < b and print(a)
```
Look's better? Sure it is. When the first part of the `and` expression will return `False` the second one will be omitted (not even considered). Shorter code make it easier to read and keeps your workbench clean!

---
_Last update: 8 March 2023_