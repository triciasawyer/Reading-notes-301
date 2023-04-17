# Reading ntoes class 1

## Component-Based Architecture

*What is a “component”?*
Components are independent and reusable bits of code. They serve the same purpose as JavaScript functions, but work in isolation and return HTML. Components come in two types, Class components and Function components.

*What are the characteristics of a component?*
Characteristics of a component are like JavaScript functions. They accept arbitrary inputs (props) and return React elements describing what should appear on the screen.

*What are the advantages of using component-based architecture?*
The benefits are reduced development and testing time, enhanced reliability (because components are pre-tested), and the flexibility to change applications by adding or replacing components without major disruption

## What is Props and How to Use it in React

*What is “props” short for?*
Properties

*How are props used in React?*
Props are used to store data that can be accessed by the children of a React component. They are part of the concept of reusability.

*What is the flow of props?*
There are basically two ways that data gets handled in React: props and state (available through this.state ). Although a component can’t change its own props, it can change its state. Props and state are used as input for the render() method to determine its output. The render() method also calls the diff algorithm which recognizes any changes in the component and logs them for batching to the “real” DOM.

## Things I want to know more about

-I want to know more about properties and how vanilla JavaScript translates over into react.
