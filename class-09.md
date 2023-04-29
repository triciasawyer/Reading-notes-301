# Reading notes for class 9

## Functional Programming Concepts

**What is functional programming?**
An approach to software development that uses pure functions to create maintainable software.

**What is a pure function and how do we know if something is a pure function?**
Pure functions are the functions that always yield consistent output and do not have any side effects. You know if something is a pure function if it returns the same result if given the same arguments (it is also referred as deterministic)
It does not cause any observable side effects

**What are the benefits of a pure function?**
The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts.

**What is immutability?**
When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

**What is Referential transparency?**
Basically, if a function consistently yields the same result for the same input, it is referentially transparent.

## Node JS Tutorial for Beginners #6 - Modules and require()

**What is a module?**
A file containing related code.

**What does the word ‘require’ do?**
The require method is used to load and cache JavaScript modules.

**How do we bring another module into the file the we are working in?**
You need to import the module, using the require key.

**What do we have to do to make a module available?**
You then need to export the module on that file.

## Things I want to know more about

Modules and how the passing of props and things work.