# Classes, Inheritance and Functional Prog

## Review, Research, and Discussion

### Why would you want to run JavaScript code outside of a browser?
**To clarify that you are using the javascript for the backend purposes that used node js and interact it with the database and some external resources.**

### What is the difference between a module and a package?
- **_module_ is a file or directory that would be found in node_modules folder which could be loaded later to your sever javascript file by require method.**
- **_package_ is a file or directory that would be add into the independencies key at package.json which in order to be published to the npm registry.**

### What does the node package manager do?
**It is an online repository that you cloud use to add, updates and uninstalls packages and module inside your node js project.**

### Provide code snippets showing 3 different ways to export a function from a node module
- Export Literal
**assign the exporting variable to a string literal in message.js:**
```
module.exports = 'Hello world';
```
**Importing the module into app.js**
```
var msg = require('./Messages.js');
console.log(msg);
```

- Export Object
**assign the exporting obejct of a certain key and property in message.js:**
```
module.exports.SimpleMessage = 'Hello world';
```
**Importing the module into app.js**
```
var msg = require('./Messages.js');
console.log(msg.SimpleMessage);
```

- Export Function
**assign the exporting a function in message.js:**
```
module.exports = function (msg) { 
    console.log(msg);
};
```

**Importing the module into app.js**
```
var msg = require('./Log.js');
msg('Hello World');
```

## Documenting the following Vocabulary Terms
- **Ecosystem**
It is more like everything working as a closed loop, so it will be easy to maintain and follow. 

- **Node js**
It is a runtime javascript environment, non-blocking, asynchronous event-driven language.

- **V8 Engine**
It is javascript Google chrome environment which is written in c++.

- **Module**
It is a file or directory that would be found in node_modules folder which could be loaded later to your sever javascript file by require method.

- **Package**
It is a file or directory that would be add into the independencies key at package.json which in order to be published to the npm registry.

- **NPM (Node Package Manager)**
It is an online repository that you cloud use to add, updates and uninstalls packages and module inside your node js project.

- **Server**
a server is a computer hardware and software that provide a data and functionalities to other devices.

- **Environment**
Set up a framework of a certain programming language.

- **interpreter**
it is a program which execute commands with a high-level language.

- **Compiler**
It is a program that will scan the whole block of codes and translate it into something more readable and show the results of it.