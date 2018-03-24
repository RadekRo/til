# display: none vs visibility: hidden
#### usability difference

Main difference between `display:none` and `visibility: hidden` is
page space usability for both of them. 

`display:none` hides element definitely. It means that
not only the exact element is hidden on page
but also a space that it occupied is cleared.
Page looks like this element never existed.

`visibility: hidden` only hides element's visibility. 
It means that all the space that is occupied by the element
still remains on page. The only difference is that this
element is not visible itself.

__Example__

```
FIRST ELEMENT
SECOND ELEMENT
THIRD ELEMENT
FOURTH ELEMENT
```

using `display: none` on SECOND ELEMENT:

```
FIRST ELEMENT
THIRD ELEMENT
FOURTH ELEMENT
```

using `visibility: hidden` on SECOND ELEMENT:

```
FIRST ELEMENT

THIRD ELEMENT
FOURTH ELEMENT
```

Got it? ;)

---
_Last update: 24 Mar 2018_ 
