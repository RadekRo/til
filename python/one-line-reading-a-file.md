# one line reading a file
```
with open("data.txt", "r") as file:   
    data = file.readline()   
    print(data) # Hello world  
```
one-line solution
```
data = [line.strip() for line in open("data.txt","r")]   
print(data) # ['hello world', 'Hello Python']
```
---
_Last update: 15 Mar 2023_ 