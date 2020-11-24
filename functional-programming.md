# Concept of the Functional Programming in JavaScript
## what does the functional programming mean?

Functional programming in ***JavaScript*** means that the function we want to build which it should more immutable and pure. So how's that possible? then we have to create a function that will not make any changes to the existing declared variable.

### So what are the methods been used to help you reach the the concept of functional programming in your code?
- immutable function
let take an example of counter to make the variable of counter unchangable bu using an **arrow function**.
```
let counter = 1;
const incrementCounterByOne = (value) => value + 1;

```

if you console.log the function and later the counter, you realized that the counter variable after the incrementation inside the arrow function does not change.

- Pure Function Benefit
In the coming example, you will see how the array of list won't change by using a map method in javascript.
```
let list = [1, 2, 3, 4, 5];
const incrementNumbers = (list) => list.map(number => number + 1);
```

- Immutability
Means that the state of the variable won't change at any circumstances. You just need to make a new object with a new value.

- Referential transparency
It means that whatever you pass the same value, it will return the same value as long as you repeat calling the function itself.
**pure functions + immutable data = referential transparency**

- Functions as first-class entities
It is a kind of way that you are going to pass a variable or constant inside a function, and later this function will be calling on other function in order to return a result from a new function.

- Higher-order functions
that means as we did in the first-class entities but instead you will used a multi-function and pass them as arguments and then return a function as result itself.

Check more about the concept of the functional programming and also as a reference of this markdown file in this [link](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa).