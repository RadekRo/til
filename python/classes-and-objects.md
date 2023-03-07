# classes and objects

#### class, object and its representation
```
class Person: // creating a class named Person
  def __init__(self, name, age):
    self.name = name
    self.age = age

p1 = Person("John", 36) // creating an Object (from Person class)

print(p1) // Output: <__main__.Person object at 0x15039e602100>
```
If you want to have a more detailed/personalized representation of the created object you can use `__str__()` function inside the class to create it.
```
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

  def __str__(self): // creating a string representation of an Object
    return f"{self.name}({self.age})"

p1 = Person("John", 36)

print(p1) // Output: John(36)
```
#### object's methods
```
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

  def myfunc(self): // a myfunc method within Person class
    print("Hello my name is " + self.name)

p1 = Person("John", 36)
p1.myfunc() // Output: Hello my name is John
```
__Important__\
The self parameter is a reference to the current instance of the class, and is used to access variables that belong to the class.

#### modify Object's properties
```
print(p1.age) // Output: 36
p1.age = 40
print(p1.age) // Output: 40
```
#### delete objects properties
```
del p1.age
print(p1.age) // Output: AttributeError: 'Person' object has no attribute 'age'
```

---
_Last update: 6 March 2023_