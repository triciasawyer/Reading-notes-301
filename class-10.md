# Reading notes for class 10

## Understanding the JavaScript Call Stack

**What is a ‘call’?**
A call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

**How many ‘calls’ can happen at once?**
Express. js can handle approx 15,000 requests per second and the basic HTTP module, 70K requests per second

**What does LIFO mean?**
Last in, First out

**Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.**
function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();

**What causes a Stack Overflow?**
One of the most common causes of a stack overflow is the recursive function, a type of function that repeatedly calls itself in an attempt to carry out specific logic. Each time the function calls itself, it uses up more of the stack memory.

## JavaScript error messages

**What is a ‘reference error’?**
When you try to use a variable that is not yet declared. It's common when using const and let, since they are hoisted like var and function but there is a time between the hoisting and being declared so when you try to access them a reference error occurs, the fact that this happens to let and const is called Temporal Dead Zone (TDZ).

**What is a ‘syntax error’?**
This occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

**What is a ‘range error’?**
When you try to manipulate an object with some kind of length and give it an invalid length.

**What is a ‘type error’?**
When the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

**What is a breakpoint?**
It is a point of code where the debugger will automatically pause the JavaScript execution. While the code is paused, we can examine current variables, execute commands in the console etc. In other words, we can debug it.

**What does the word ‘debugger’ do in your code?**
It stops the execution of JavaScript, and calls (if available) the debugging function. This has the same function as setting a breakpoint in the debugger.

## Things I want to know more about

-How to fix errors and just becoming familiar with the errors and what they mean.
