# Routing

## Review, Research, and Discussion
### Do child components have direct access to props/state from the parent?
**Yes, definitly it could be possible by using the props from a specified element.**

### When a component “wraps” another component, how does the child component’s output get rendered?
**By importing the file of the child component and return its rendering in the return method.**

### Can a component, such as <Content />, which is a child also be used as a standalone component elsewhere in the application?
**Definilty by export and import it in a specified file and alse could pass any variable between opening and closing tag of the element and then call these variables by using props.children.**

### What trick can a parent use to share all props with it’s children
**As I mentioned in the previous question, by using the props.children where it get the values from the passing state variables between opening and closing tags.**

## Document the following Vocabulary Terms
- **_props.children_** is a way that components use a specified children prop to pass children elements directly into their output.

- **_composition_** is a mechanism way of inheriting a vaiable from the parent component to the child component by using props.children.