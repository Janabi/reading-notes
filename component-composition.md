# Component Composition

## Review, Research, and Discussion
### Can a parent component access the state of a child component?
**Definitley by using the props methodology, that will pass a created properties and give it the state data that would be sent to the parent.**

### What can be passed along in a prop variable?
**It could include any type of data (number, string, array, boolean, ...etc).**

### How can a child component “know” the state of another component?
**Simply by using the react props inside the another component that we want to send its child state.**

## Document the following Vocabulary Terms
- **_component props_** is a method to export some data between the components.

- **_component state_** is a build-in object in each react component and could only be used within the same component.

- **_application state_** is a parent or root component that will have all of the children inside of it and render it to the HTML file.


## Preview

***Component Composition- it is a way to avoid the drilling props in many levels and only using a shorthand method within the HTML elements which called createContext() where by default it will pass the prop value all of the given level without go through them and define it again with each level.***