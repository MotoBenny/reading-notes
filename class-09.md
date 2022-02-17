Class-09.md

## **Table Of Contents**

_Read:_ 09 - Forms and Events

## ***Ducket HTML***

1. Chapter 7: “Forms” (p.144-175)
2. Chapter 14: “Lists, Tables & Forms” (pp.330-357)

## ***Ducket js***

1. Chapter 6: “Events” (pp.243-292)

## ***Ducket HTML***

### **Chapter 7: “Forms” (p.144-175)**

- HTML Forms are boxes the user can type in information.
- they can also be checkboxes, radio buttons, drop down menus and more.
- every form requires an action attribute.
- forms can be sent one of two methods, Get or Post.

 1. The get method adds the value of the form to the end of the url specified in the action attribute.
 2. the post method values are sent in HTTP headers, this makes them perfect for sensitive information. or for lots of form data.

- by default input type="password" will obscure the users inputs
- type="radio" will create a radio button, "checkbox" a checkbox

### **Chapter 14: “Lists, Tables & Forms” (pp.330-357)**

- list-style-type will denote the style of your UL bullet points. And can also accept symbols or emojis on a stylesheet
- table properties should be applied to make your table easier to read.
- border spacing can add gaps between the cells of your tables.
- fieldsets are great for styling the edges of a larger form and help by grouping together related form items.

## ***Ducket js***

### **Chapter 6: “Events” (pp.243-292)**

- As you browse a webpage your browser stores events, which you can use to trigger code. 
- to trigger an event with JS you must use a DOM query to get the DOM node, indicate which event on the node will trigger the response, then state the code you want to run.
- event handlers. `element.onevent = functioncall`
- event listeners are a more recent way to handle events. But are not always supported on older browsers. 
- `element.addEventListener('event',functionname [, BOOLEAN]`
- you cannot have parens after function names in event handlers or listeners. this requires a work around
```javascript
el.addEventListener('blur',function() {
  checkUsername(5);
}. false);
```
- Event flow allows you to listen for a specific event on parent element.

