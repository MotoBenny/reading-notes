# Read 01

## Introduction to React and Components

### Component=based Architecture

[component-based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

#### Reading assignment questions

1. What is a “component”?

- A modular reusable set of well-defined functionality,
- A software object, intended to work with other components,

2. What are the characteristics of a component?

- reusability - components are designed to be modular and can be used in different situations and tasks.
- replaceable - components can be freely substituted with other similar components.
- non specific Context - This means the component isn't specialized and can apply to different contexts.
- extensible - component can be extended from existing components to provide new behavior.
- encapsulated - A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.
- independent - designed to have minimal dependencies on other components.

3. What are the advantages of using component-based architecture?

- ease of deployment - easy to replace older components with minimal or no impact to others or the system
- reduced cost - allows you to spread the cost of development.
- ease of deployment - Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.
- reusability - modular nature means similar components can be used for many jobs.
- modification of technical complexity - this point literally doesn't mean anything. Modifying the complexity could easily be a negative thing, this is a very poorly written article.
- reliability - increases since the reliability of each individual component increases reliability of whole system.
- maintenance and evolution - easy to change and update without effecting other parts of the system
- independent - modular nature, since components don't relay on each-other, allowing different teams to work in parallel. increasing development productivity.

### Reading notes

CBA focuses on breaking a design down to individual functional parts, these parts would contain all they need to be functional.
containing all methods, events, properties they need within them.

the primary objective of CBA is to ensure each component is fully reusable, wherever its needed.

### What is “Props” and how to use it in React?

[What is “Props” and how to use it in React?](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0)

#### Reading assignment questions

1. What is “props” short for?

- "props" is shorthand for properties.

2. How are props used in React?

- properties are used to pass data from one component to another.

3. What is the flow of props?

- data flow is always one way from parent element to child element.

### Reading notes
