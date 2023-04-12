# The print functions "end" parameter
```
a = ["english", "french", "spanish", "german", "twi"]
for language in a:
    print(language, end=" ")

Output: english french spanish german twi
```
It is quite common to use a print statement without defining any of its optional parameters. Consequently, several Pythonistas are unaware that you can control the output to some degree.

One optional parameter we can change is end. The end parameter specifies what should be shown at the end of a call to a print statement.

The default of end is "\n" which tells Python to start a new line. In the code above, we changed it to space. Thus, the output returned all the elements of our list are printed on the same line.


#### Thanks to Kurtis Pykes's _"30 Cool Python Tricks For Better Code With Examples"_
---
_Last update: 23 March 2023_