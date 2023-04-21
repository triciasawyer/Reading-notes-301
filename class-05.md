# Reading notes for class 5

## React Docs - Thinking in React

**What is the single responsibility principle and how does it apply to components?**
(SRP) is that every class, module, or function in a program should have one responsibility/purpose in a program. As a commonly used definition, "every class should have only one reason to change".

**What does it mean to build a ‘static’ version of your application?**
Static frameworks are pre-compiled libraries that are linked to your app during the build process. This means that the framework code is included in the final app binary and cannot be updated or changed at runtime.

**Once you have a static application, what do you need to add?**
You need to add interactivity.

**What are the three questions you can ask to determine if something is state?**
Identifying components that use state. ProductTable needs to filter the product list based on that state (search text and checkbox value).
SearchBar needs to display that state (search text and checkbox value).
Find their common parent: The first parent component both components share is FilterableProductTable.
Decide where the state lives: We’ll keep the filter text and checked state values in FilterableProductTable.

**How can you identify where state needs to live?**
Identify every component that renders something based on that state.
Find their closest common parent component—a component above them all in the hierarchy.
Decide where the state should live. Often, you can put the state directly into their common parent.
You can also put the state into some component above their common parent.
If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common parent component.

## Higher-Order Functions

**What is a “higher-order function”?**
They are functions that operate on other functions, either by taking them as arguments or by returning them.

**Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?**
Line 2 is creating a return that takes in m, and allows m to be greater than n.

**Explain how either map or reduce operates, with regards to higher-order functions.**
The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. The new array will have the same length as the input array, but its content will have been mapped to a new form by the function.
