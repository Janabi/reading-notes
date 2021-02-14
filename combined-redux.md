# Redux - Combined Reducers

### Comibned Redux
**_combineReducers_ is simply a utility function to simplify the most common use case when writing Redux reducers.**
**Also, _combineReducers_ is entirely possible to write reducer logic without using it, and it is quite common to need to write custom reducer logic for cases that _combineReducers_ does not handle. It will call each slice reducer with its current slice of state and the current action.**

### Defining State Shape
**There are two ways to define the initial shape and contents of your store's state. First, the _createStore_ function can take _preloadedState_ as its second argument. Also, _combineReducers_ takes an object full of slice reducer functions, and creates a function that outputs a corresponding state object with the same keys.**

***The state produced by combineReducers() namespaces the states of each reducer under their keys as passed to combineReducers(). For example, we have this following example of the counter:***
```
export default function counter(state = 0, action) {
  switch (action.type) {
    case 'INCREMENT':
      return state + 1
    case 'DECREMENT':
      return state - 1
    default:
      return state
  }
}
```

```
import { combineReducers } from 'redux'
import todos from './todos'
import counter from './counter'

export default combineReducers({
  counter
})
```