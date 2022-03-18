# Read05

## [thinking in React](https://reactjs.org/docs/thinking-in-react.html)

What is the single responsibility principle and how does it apply to components?

A component should ideally only do one thing. If it grows it should be broken into sub-components. 

What does it mean to build a ‘static’ version of your application?

A static version of your application is the basic structure of the application, all the components in the right place, and proper Parent Child structure. But no interactivity/functionality.

Once you have a static application, what do you need to add?

A static application has no logic or functionality, it is simply the visible structure of your page.

What are the three questions you can ask to determine if something is state?

Is it passed in from a parent via props? If so, it probably isn’t state.
Does it remain unchanged over time? If so, it probably isn’t state.
Can you compute it based on any other state or props in your component? If so, it isn’t state.

How can you identify where state needs to live?

Identify every component that renders something based on that state.
Find a common owner component (a single component above all the components that need the state in the hierarchy).
Either the common owner or another component higher up in the hierarchy should own the state.
If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.


## [Higher order Function](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

What is a “higher-order function”?

Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions

Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

Returns the value of M if m is greater than N.

Explain how either map or reduce operates, with regards to higher-order functions.

.map will transform an existing array, by out putting a new array, comprised of all the values of the argument array, but after they have been passed through a function.
