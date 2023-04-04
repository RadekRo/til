# merging two dictionaries

##### update() method
```
dict_1 = {'John': 15, 'Rick': 10, 'Misa' : 12 }
dict_2 = {'Bonnie': 18,'Rick': 20,'Matt' : 16 }
dict_1.update(dict_2)
print(dict_1)
```
Output: {'John': 15, 'Rick': 20, 'Misa': 12, 'Bonnie': 18, 'Matt': 16}\
Have in mind that if the same key will occur dict_1 value will be overwritten by dict_2

##### using ** operator
```
dict_1 = {'John': 15, 'Rick': 10, 'Misa' : 12 }
dict_2 = {'Bonnie': 18,'Rick': 20,'Matt' : 16 }
dict_3 = {**dict_1,**dict_2}
print(dict_3)
```
Output: {'John': 15, 'Rick': 20, 'Misa': 12, 'Bonnie': 18, 'Matt': 16}
As above if the same key will occur the second dictionary will overwrite the first one.

---
_Last update: 4th Apr 2023_ 