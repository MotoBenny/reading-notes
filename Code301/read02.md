# Read 02

### React: Component Lifecycle Events

[React: Component Lifecycle Events](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

#### Reading assignment questions

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

- render happens first according to the diagram.

2. What is the very first thing to happen in the lifecycle of React?

- Mounting.

3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

- constructor, render, react Updates, componentDidMount, componentWillUnmount

4. What does componentDidMount do?

- initialization that requires DOM nodes should go here.

### Reading notes

In react you can define components as classes or functions, the methods you can use on these are called lifecycle events.

### React: State vs Props

[React State vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

#### Assignment questions

1. What types of things can you pass in the props?

- props are basically the argument to a function. for example in a counter, you would pass in the initial counter value you want.

2. What is the big difference between props and state?

- State is inside a component, and can be updated inside the component. Where props get passed into the component and cannot be updated inside a component.
state is when you need to change or update something displaying based on a users action.

3. When do we re-render our application?

- we would re-render when the user updates or enters some data on the application, When a State has been changed by the user, we would re-render.

4. What are some examples of things that we could store in state?

- inside a form, as a counter we are using to iterate.
