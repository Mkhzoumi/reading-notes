# React Forms


## What is a ‘Controlled Component’?
+ ## it's when we combined html form state with the react state, the react + component that renders a form will also have the ability to control what happens in that form on subsequent user input, the input form element whose value is controlled by react in that way is called controlled component. 

## Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
+ ## we update the value in state with their responses as soon as they enter them , so the display value will update as the user tyoes.

## How do we target what the user is entering if we have an event handler on an input field?
+ ## the value will be in event.target.value . 
## example about forms in React:

```
class NameForm extends React.Component {
  constructor(props) {
    super(props);
    this.state = {value: ''};

    this.handleChange = this.handleChange.bind(this);
    this.handleSubmit = this.handleSubmit.bind(this);
  }

  handleChange(event) {
    this.setState({value: event.target.value});
  }

  handleSubmit(event) {
    alert('A name was submitted: ' + this.state.value);
    event.preventDefault();
  }

  render() {
    return (
      <form onSubmit={this.handleSubmit}>
        <label>
          Name:
          <input type="text" value={this.state.value} onChange={this.handleChange} />
        </label>
        <input type="submit" value="Submit" />
      </form>
    );
  }
}
```

# The Conditional Ternary Operator

## Why would we use a ternary operator?
+ ## faster and less code, it can be written in one line.

## Rewrite the following statement using a ternary statement:

## using if:

```
 if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```

## using ternary:

```
x === y ? console.log(true) : console.log(false); 
```






# [back](../README.md)