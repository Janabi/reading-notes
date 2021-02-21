# React Native

### What is react native?
***React native - it is an open source mobile application framework that was created by Facebook team and build up by Javascript language. This framework is used to create a mobile applications in multi-softwares like iOS, android, and windows.***

### How it works?
**React Native is like React, but it uses native components instead of web components as building blocks. So to understand the basic structure of a React Native app, you need to understand some of the basic React concepts, like JSX, components, state, and props.**

***React Native App Example:***
```
import React from 'react';
import { Text, View } from 'react-native';

const HelloWorldApp = () => {
  return (
    <View
      style={{
        flex: 1,
        justifyContent: "center",
        alignItems: "center"
      }}>
      <Text>Hello, world!</Text>
    </View>
  )
}
export default HelloWorldApp;
```

***If you would like to use it, there is a package as in the previous eaxmple, called React Native, that would have a  lot of react native elements that you can display the components. Also, there is no difference in using the state variable in both React and React Native.Then, you can define and use the state variable in either functions or classes by using Hooks.***
