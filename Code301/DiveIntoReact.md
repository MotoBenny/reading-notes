# Read01

## Dive Into React

Reading notes from [this](https://www.youtube.com/watch?v=FRjlF74_EZk) video.

### Assignment Questions

1. What is React?

- React is a user interface Library, Used to create UI for webpages/applications etc.

2. What is a component?

- A component within React is a small piece of code that contains a portion of the user UI.

3. What is the dataflow of React?

- React has a one way data flow.

4. How do we make a React element a DOM element?

- A React element does not become a DOM element until it is passed through ReactDOM

5. React is a User Interface ______.

- Library

6. Which direction does data flow in React?

- Data flows down one way through a React App

7. Every component manages its own ____.

- Component State.

### My Viewing Notes

High Level React Points.

  1. A User Interface Library
    - It us used to create user interfaces, websites, applications, anything the user is going to interact with.

  2. Component Architecture
    - A component is a small piece of code that fills a portion of the user interface.

  3. Data Flow in React
    - React has a one way data flow.

  4. Component State
    - This means we manage state data or changes are happening with the application, but they are controlled at a component level.

### User interface Library

- React is agnostic, It doesn't care where the user interface is being displayed. I.E. On a browser, or within an application.

- Always needs to be used in conjunction with a second lib, like ReactDOM or ReactServer.

- A React Element is **NOT** a DOM Element.

- A React Element is simply a native JS Object.

- Being a user interface library, you can use React to create simply a small tool on a webpage, or the entire webpage itself.

### Component Architecture

  1. For example. The Header component of react contains, HTML, and may contain things like a logo/advert/nav buttons/ etc.

### Data flows down one way

  1. Data flows down through all React Elements from the top, You can further dial what gets the data, via which react component you call, much like parameters.

  2. If the component does something with that Data, You need to then call for that newly updated data again, from say, React App. You cannot then pass that data back up to the element above it.
