# Reading notes for class 2

## React lifecycle

**Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**
Render

**What is the very first thing to happen in the lifecycle of React?**
constructor

**Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates. What does componentDidMount do?**
constructor, render, react updates, componentDidMount, componentWillUnmount.

## React State Vs Props

**What types of things can you pass in the props?**
We can pass any data type as props in React components: object, array, boolean, number, string, function, etc.

**What is the big difference between props and state?**
State is internal and controlled by the component itself while props are external and controlled by whatever renders the component.

**When do we re-render our application?**
When React needs to update the app with some new data. Usually, this happens as a result of a user interacting with the app or some external data coming through via an asynchronous request or some subscription model

**What are some examples of things that we could store in state?**
The state is encapsulated data where you store assets that are persistent between component renderings. The state is just a fancy term for a JavaScript data structure. If a user changes state by interacting with your application, the UI may look completely different afterwards, because it's represented by this new state rather than the old state.

## Things I want to know more about
