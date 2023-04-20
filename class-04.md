# Reading notes for class 4

## React Docs - Forms

**What is a ‘Controlled Component’?**
A controlled component is a component that is controlled by React state, while an uncontrolled component is a component that maintains its own internal state. A controlled component receives its current value and an update callback via props, and the parent component manages the state of the component.

**Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why?**

**How do we target what the user is entering if we have an event handler on an input field?**
When you need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name.

## The Conditional (Ternary) Operator Explained

**Why would we use a ternary operator?**
The ternary operator valuates conditions to present a true or false value, (if/else conditional statements) but with more concise syntax and parameters than other methods

**Rewrite the following statement using a ternary statement:**
**if(x===y {**
    **console.log(true);**
**} else { console.log(false);}**

if x === y { console.log(?);
}  else console.log (!);
