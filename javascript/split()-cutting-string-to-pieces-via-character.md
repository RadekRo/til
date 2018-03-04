# split() 
#### cutting string to pieces via character

If you would like to cut your string using a specified character
you can use split() method to do this.

`Remember that the character which you are providing as a cutter
will be distracted and removed from all the parts of the cutted string.`

__Example:__

```
const myString = 'Radek-Roclawski-IT';

const myPieces = mystring.split('-');

// Returns:
// myPieces = ['Radek', 'Roclawski', 'IT'];
// You can now simply get access to all the cutted parts using []
// myPieces[0] = Radek, etc.

---
_Last update: 04 Mar 2018_ 

```

