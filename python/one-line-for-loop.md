# one line "for" loop
```
mylist = [200, 300, 400, 500]

result = [] 
for x in mylist: 
    if x > 250: 
        result.append(x) 
print(result) # [300, 400, 500]
```
one-line solution
```
result = [x for x in mylist if x > 250] 
print(result) # [300, 400, 500]
```
---
_Last update: 14 Mar 2023_ 
