# Custom Hooks

## Review, Research, and Discussion
### What does a component’s lifecycle refer to?
**Starting from a mounting through updating till it will reach unmounting.**

### Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect
**useCallback will be useful for prevention recreation of a function.**

### Why are functional components preferred over class components?
**It is much easier to track the code and test it. Also, It will be used to separate a presentational components without putting them in one variable.**

### What is wrong with the following code?
```
import React, {useState, useEffect} from 'react';

function MyComponent(props) {
  const [count, setCount] = useState(0);

  function changeCount(e) {
    setCount(e.target.value);
  }

  let renderedItems = []

  for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update');
    }, [count]);

    renderedItems.push(<div key={i}>Item</div>);
  }

  return (<div>
     <input type='number' value={count} onChange={changeCount}/>
      {renderedItems}
    </div>);
}
```
**The useEffect must be somewhere outside the for loop.**

## Document the following Vocabulary Terms
- **_state hook_** is a new method that used from React package to initialize and update the state inside a function.
- **_effect hook_** is a method that sued from React package to apply a side effect once the user has done any interacts on the web page.
- **_reducer hook_** is a way to manage a state variable.

## Preview
***useReducer -> is a new method from React package to handle your state varaible within a certain component and re-render a components once the changes applied on the state. This method will take two parameters, which the first one will be for a function that will apply a changes and the initial value as an object.***