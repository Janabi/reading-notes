# Context API

## Review, Research, and Discussion
### Describe use cases for useMemo() and useReducer()
**_useReduce_ is the method to handle data just like useState but the reducer will deal with deep updates and complex one for the values.**
**_useMemo_ is the method that run during the rendering and will only recompute the memoized value when one of the dependencies has changed.**

### Why do custom hooks need the use prefix?
**It will good practice for the react to maintain the hooks.**

### What do custom hooks usually do?
**Create a custom hooks will make it easier to track the code and helps to create a custom one that would be used in several places within the web app.**

### Using any list of custom hooks, research and name one that you think will be useful in your applications
**useFrom -> would be use to get any changes to the input data and handle the submition.**

### Describe how a hook that fetches API data might work
**It will use every CRUD methods that will deal with the data API by using either axios, superagent or fetch.**

## Document the following Vocabulary Terms
- **_Reducer_** is a method that use to manage the changes of the state values.

## Preview
**Context API is a way to export a data within the components without having to use a props for each element in the rendering function. This could be done by using the context provider which is by import createContext from react package.**