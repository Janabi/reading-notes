# Hooks API

## Review, Research, and Discussion
### Why do we not need more .html pages in a multi-page React app?
**Because we can load a multiple components without loading the whole page.**

### If we wanted a component to show up on every page, where would we put it and why?
**Inside the <BrowserRouter/>. Outside the <Route/>.**

### What does props.children contain?
**props.children could contain a multiple elements or data that could be used in other files as HTML format.**

## Document the following Vocabulary Terms
- **_Composition_** is a way on how transfer a data from one components to others by using the props methodology.

- **_Children / Child Components_** is type of component that uses the children  of the other component to retrieve its elements and data inside it.

- **_Hash Routing_** is a way to link an anchor tag to other routes by passing the hashtag sign before the eact route without hitting the server or reload the whole page.

- **_Link Routing_** is a most common way in the react where you only pass a route to load a specify components.

## Preview
***Hooks is a method that used in React where specifically with a function only, it is a new way to handle a state data. However, this will initialize as an array of two elements which is the first one will be the initial value of the state and the second one is a function that will be used to update the value of the state. The useState function must be executing at exact same order without having any specified condition applies on it. Also, there is a useEffect where is applied a sied effect when anything happened in the web app. This method will took a two paramteres, the first one will be a callback function that where the changes is happened and the second one will be specify which variable are going to make this effect by passing it into an array.***