# Json data file structure and retrieving data

To properly keep data in json file you must remember to use `"` before and after not only
the value but also the name of the object element.

__Example:__

```
users.json

[
    { "id": "1", "name": "Radek", "phone": "555233456" },
    { "id": "2", "name": "Kasia", "phone": "334233212" }
]
```

The easiest way to retrive data from the json file and putting them to the current state
with an error message if something wrong will occur is:

```
(...) extends Component {

state = {
            contents: [],
            error: null
        };

componentDidMount() {
        fetch('[dir]/users.json')
            .then(response => response.json())
            .then(data => this.setState({ contents: data }))
            .catch(error => this.setState({ error }))
    }
 
 (...)
    
    { this.state.error && <p>{ this.state.error.message }</p> }
    // this is the error message - put it inside your document structure    
}
```
---
_Last update: 04 Mar 2018_ 
