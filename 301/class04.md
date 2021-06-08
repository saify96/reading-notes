## What is a ‘Controlled Component’?
 - ### An input form element whose value is controlled by React in this way

## Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
 - ### we will update the state with their responses as soon as they enter them, because handleChange runs on every keystroke to update the React state, the displayed value will update as the user types.

## How do we target what the user is entering if we have an event handler on an input field?
 - ### this.state.value.

---

## Why would we use a ternary operator?
 - ### because it will help us to write shorter code, we can writle one line code insted of write if statment with multi-lines.

## Rewrite the following statement using a ternary statement:

####  if(x===y){
#### console.log(true);
####  } else {
#### console.log(false);
####  }

- ### soluation

#### x===y? console.log(true) : console.log(false)