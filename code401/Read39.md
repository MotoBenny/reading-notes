## [create-nextjs-app](https://nextjs.org/learn/basics/create-nextjs-app)

To build a complete web application with React from scratch, there are many important details you need to consider:

-   Code has to be bundled using a bundler like webpack and transformed using a compiler like Babel.
-   You need to do production optimizations such as code splitting.
-   You might want to statically pre-render some pages for performance and SEO. You might also want to use server-side rendering or client-side rendering.
-   You might have to write some server-side code to connect your React app to your data store.

A _framework_ can solve these problems. But such a framework must have the right level of abstraction — otherwise it won’t be very useful. It also needs to have great "Developer Experience", ensuring you and your team have an amazing experience while writing code.

### Next.js: The React Framework

Enter **Next.js**, the React Framework. Next.js provides a solution to all of the above problems. But more importantly, it puts you and your team in the [pit of success](https://blog.codinghorror.com/falling-into-the-pit-of-success/) when building React applications

`npx create-react-app _________` where the blank is the app name 'demo_app'
`npm run dev` spin up the dev environment on port 3000

Then proceed to edit and customize your page to your goal!

## [React context](https://www.freecodecamp.org/news/react-context-for-beginners/)

React context is a tool to manage and share state in your react applications

Allows the transfer of all sorts of state data more easliy, such as user location data, theme data (light/dark) authentication data and more. 

Data should be placed on React context that does not need to be updated often.

Why? Because context was not made as an entire state management system. It was made to make consuming data easier.

_You can think of React context as the equivalent of global variables for our React components._

React context helps us avoid the problem of props drilling.

**Props drilling** is a term to describe when you pass props down multiple levels to a nested component, through components that don't need it.

