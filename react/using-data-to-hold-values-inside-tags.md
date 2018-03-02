# Using data to hold values inside tags

If you want to hold more than just name and value or other standard html values 
 of the input or other html tag while using React you can use data to do it. 
 
__Example:__

I want to hold task id inside input element to have the opportunity to use it inside 
called function while changes made to this specific element.

`<input name="[task-name]" value="[current-value]" data-task-id="[current-task-id]" onChange={ this.handleInput }>`

Handling data-task-id inside function called:

``` 
handleInput = (event) => {
    
    this.setState({    
        [your-name]: event.target.dataset.taskId
    })
}
```

This will add current task id to the specified [your-name] inside state element.

---
_Last update: 02 March 2018_ 