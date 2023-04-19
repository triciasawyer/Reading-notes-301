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
Known as array concatenation -
Ex.
const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩

**Give an example of using the spread operator to add a new item to an array.**
Ex.
const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍

**Give an example of using the spread operator to combine two objects into one.**
Ex.
[...["😋😛😜🤪😝"]] // Array [ "😋😛😜🤪😝" ]
[..."🙂🙃😉😊😇🥰😍🤩!"] // Array(9) [ "🙂", "🙃", "😉", "😊", "😇", "🥰", "😍", "🤩", "!" ]

const hello = {hello: "😋😛😜🤪😝"}
const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }

## How to Pass Functions Between Components

**In the video, what is the first step that the developer does to pass functions between components?**

**In your own words, what does the increment function do?**
The increment function takes a variable and changes its value, and also returns this value.

**How can you pass a method from a parent component into a child component?**
You can use props to transfer the data. The Child will access the data in the props. An example like this where you want to transfer a message from Parent to Child. The Parent pass the data in message, and the Child got the data in props.

**How does the child component invoke a method that was passed to it from a parent component?**
You pass the function reference to the child component as a prop. Then you can call that parent's function from the child component like props, parentMethodName().

## Things I want to know more about
