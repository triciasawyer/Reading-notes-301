# Reading notes for class 3

## React Docs - lists and keys

**What does .map() return?**
A new array with transformed elements and the same amount of data

**If I want to loop through an array and display each value in JSX, how do I do that in React?**

**Each list item needs a unique ____.**
Key

**What is the purpose of a key?**
The purpose of a key is to create and return an array iterator object which contains the keys for every index in an array.

## The Spread Operator

**What is the spread operator?**
It is used to make deep copies of JS objects. When we have nested arrays or nested data in an object, the spread operator makes a deep copy of top-level data and a shallow copy of the nested data. Using this operator makes the code concise and enhances its readability.

**List 4 things that the spread operator can do.**
Copying an array, combining arrays, adding an item to a list, and using an array as arguments.

**Give an example of using the spread operator to combine two arrays.**

**Give an example of using the spread operator to add a new item to an array.**

**Give an example of using the spread operator to combine two objects into one.**

## How to Pass Functions Between Components

**In the video, what is the first step that the developer does to pass functions between components?**
**In your own words, what does the increment function do?**
**How can you pass a method from a parent component into a child component?**
**How does the child component invoke a method that was passed to it from a parent component?**
