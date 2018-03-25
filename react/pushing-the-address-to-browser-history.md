# Pushing the address to browser history

If you would like to dynamically change components within your project by using a
 for ex. button, you can push the address to browser history using: `this.props.history.push()`.

__Example:__

__Main component:__ (where you are using Route to change address) 

```
import { BrowserRouter } from 'react-router-dom'

(...)

<BrowserRouter>
    <React.Fragment>
        <Route path="[location]" component={ [component name] } />
    </React.Fragment>
</BrowserRouter>
```

__Usage in current component:__ (where you are putting a button)

```
handleSubmit = () => {
        this.props.history.push('[location]');
};

(...)

<button onClick={ this.handleSubmit }>Submit</button>

```

---
_Last update: 28 Feb 2018_ 