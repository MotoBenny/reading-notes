# Read03

## Passing Functions as Props

What does .map() return?

- .map() returns an array of

If I want to loop through an array and display each value in JSX, how do I do that in React?

```javascript
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li>{number}</li>
);
```

Each list item needs a unique ____.

Key

What is the purpose of a key?

Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:

## The Spread Operator

What is the spread operator?

`...` is the spread operator.
The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

List 4 things that the spread operator can do.

Spread an array into separate arguments.
Copying an array
Concatenating or combining arrays
Using Math functions
Using an array as arguments
Adding an item to a list
Adding to state in React
Combining objects
Converting NodeList to an array

Give an example of using the spread operator to combine two arrays.

```javascript
const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍
```

Give an example of using the spread operator to add a new item to an array.

```javascript
const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]
```

Give an example of using the spread operator to combine two objects into one.

```javascript
const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂

```

### [How_to_Pass_Functions_between_Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

In the video, what is the first step that the developer does to pass functions between components?

creates his function, and passes in the person object.

In your own words, what does the increment function do?

The increment function takes in an, array of objects, grabs the correct object based on its name property, and adds +1 to the value of its count property.

How can you pass a method from a parent component into a child component?

you can create a prop with contains the method you want to call in the child

How does the child component invoke a method that was passed to it from a parent component?

this.props.increment.
