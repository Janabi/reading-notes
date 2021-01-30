# Component Based UI

## Review, Research, and Discussion

### Name 5 Javascript UI Frameworks (other than React)
- angular.js
- Bootstrap
- Vue.js
- Ember.js
- Meteor.js

### What’s the difference between a framework and a library?
The main deifferent of both concepts is based of inversion of control. Library is a set of code where you are in charge of use it within your app, so you can choose it wherever and whenever you've liked. However, the framework is a set of libraries where you have a limited of choices based on the available server that it has nad it will strict you where and when are you using this service.

### Document the following Vocabulary Terms
- **_Rendering_** is a way to display the outpu from the back end part and display it into a form of HTML and CSS in the web browser using  one of rendering methodology.

- **_Templates_** make an HTML template for a certain data that came up from a server side.

- **_state_** is a well known tool to coordinate your code. it defines the status of your prgram whether it shows as text, boolean or number.

## Preview

**_React_ is a common javascript library that used to render a data from a server side into an HTML elements that could be displayed at the web browser. it could be used within the same JS file to render the data into HTML code, this methodology is called JSX.**
- Here is a simple example of starting a react code:
```
ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);
```