# pseudo-classes and pseudo-elements

### pseudo-classes

__Refererred:__

`:link` - every `<a>` tag with `href` attribute leading to unvisited page.  
`:visited` - every `<a>` tag with `href` attribute leading to visited page.

__Dynamic:__

`:focus` - an element that might be activated is some way or might receive 
data entered via keyboard.  
`:hover` - mouse is over that element.   
`:active` - element is just activated, for ex. pressed, clicked. It might be 
as an blink of an eye.  

Remember about __LVHA__ rule. Which means that you should always use pseudo-classes
in particular order: :link, :visited, :hover, :active (if all of them are used).

__Descendant:__

`:first-child` - first child of an element.  
`:last-child` - last child of an element.  
`:nth-child(n)` - the `n`th child of the element.  
`:only-child` - the element without any siblings.  
`:last-of-type` - last element of it's type among the group of siblings.  

__Forms:__

`:in-range` - represents the value that is between min and max value of an `<input>`
element.  
`:out-of-range` - represents the value that is out of min and max value of an `<input>`
element.  
`:read-only` - represents the `<input>` element that is not editable by the user.  
`:required` - represents the `<input>`, `<textarea>` or `<select>` that has `required` 
attribute set on it.

### pseudo-elements

`::first-line` - styling first line of the element's text.  
`::first-letter` - styling first letter of the element's text.  
`::before` - entering some text before specified element.  
`::after` - entering some text after specified element.  
`::selection` - applies styles to an element that has been highlighted by the user.  
`::placeholder` - represents the placeholder's text of an element.

__Example:__

```markdown
CSS: 
p::first-line {
    color: red;
}

p::first-letter {
    font-size: 20px;
}

HTML:
<p>Long time ago<br/> // First letter will have 20px size, this line will have the blue color
In the Galaxy far far away...</p>
```
---
_Last update: 24 Mar 2018_ 