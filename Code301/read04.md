# Read 04

## [React Forms](https://reactjs.org/docs/forms.html)

What is a ‘Controlled Component’?

in React, mutable state is typically kept in the state property of components, and only updated with setState().
We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

We should update the state as soon as the user input's them, that way the displayed value updates in real time as the user types. 

How do we target what the user is entering if we have an event handler on an input field?

When you need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name

# Ternary

Why would we use a ternary operator?

A ternary operator allows us to shorten a If statement to one line of code. 

Rewrite the following statement using a ternary statement:


```javascript
if(x===y){
  console.log(true);
} else {
  console.log(false);
}

x = y === true ?  console.log(true) : console.log(false);

```