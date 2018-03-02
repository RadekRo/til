# Target attribute of an event constructor

Thanks to the target attribute you can pass the event values or other elements to
the called function.

__Example:__

`<input name="Flag" value="RisedUp" onChange={ this.handleFlagChange }>`

Now I can call a name and value thanks to a target attribute:

```
handleFlagChange = ({ target: { name, value } }) => {
    this.setState({
        [ name ]: value
    })
}
```

That will set state of a Flag element to RisedUp. You can use only value if you want
 and change state of an other existing value in state or do whatever you want with these 
 values.
 
 ---
 _Last update: 02 March 2018_ 