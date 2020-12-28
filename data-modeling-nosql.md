# Data Modeling & NoSQL Databases

## Review, Research, and Discussion

### Name 3 advantages to Test Driven Development
- It would help to have a better undertsanding on how your web application is perfurming.
- It would make your code much cleaner and qualified.
- Easy refactoring any mistakes that you might made later.

### In what case would you need to use beforeEach() or afterEach() in a test suite?
- Execute a function after each one of the tests in this file completes.
- Execute a function before each one of the tests in this file completes.

### What is one downside of Test Driven Development
**It has an additional complexity that sometimes will make some bugs and you have to change the way you coded.**

### What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
**It is time consumer where you create a new constructors that has the same properties as the first constructor.**

### Name a use case for a static method
**A static belongs to the class rather than to the object.**

### Write an example of a Higher Order function and describe the use case it solves
```
function sayName(name) {
    console.log("Hello ", name);
}
function sayHello(name, func) {
    return function() {
        func(name);
    }
}

let greeting = sayHello("Janabi", sayName);
greeting();
```
**As we saw in the previous example, the usage of high order functions is that it will return a function instead of any other data types.**

## Documenting the following Vocabulary Terms

- ***functional programming***
It is a method that you structure and construct yout code by using functions.

- ***pure function***
Means that it is a way to use a function in order to make some implementation for a valid variable without harming it after invoking the variable anywhere outside the function.

- ***higher-order function***
It is a function that returning another function to run a certain results. 

- ***immutable state***
It is a way to assign a variable to a new value, or maybe that happened in a function where it used that variable. 

- ***object***
It is a sets of keys and values where you can create it using either constructor or new Object().

- ***Object Oriented Programming***
It is a concept in all programming languages where you are going to deal with objects or classes which contain a sets of different data type variables.

- ***Class***
It is new concept where is written in 2015 where ES6 released. It does the same as prototype and contructor functioning but with more readable and cleaner codes.

- ***prototype***
A way to create a method for a certain constructor object which helps to implement some certain conditions for the properties of this object.


- ***super***
It is a resereved ward where you can used it to get the same properties of original constructor and allowing you to add even more for the new one.

- ***inheritance***
It means that you are inherent some variables between the objects.


- ***constructor***
It is a function or a class in order to create an object.

- ***instance***
The new object variable declared and initiated from certain constructor, therefore, this variable is instance of the constructor object.

- ***context***
It is either function, global or eval.

- ***this***
this is a reserved word that determined by how the function is called. 

- ***Test Driven Development (TDD)***
It is a methodolgy that determine on how your code should be worked.

- ***jest***
It is a node package where the developer can use it to run the test files.

- ***Continuous Integration (CI)***
It is the practice of automating the combination of code changes from multiple developers into a single software project.

- ***unit test***
It is the unit that used to test your code, for example, jest.