# TCP Servers

## Review, Research, and Discussion

### Given the examples of front-end events such as button click, window resize, form submit, etc, what are some examples of back-end events?
- to get data from certain resource.
- recieve a certain data.

### Why are events sometimes better than asynchronous actions with callbacks?
**Events can be used in serveral times but the async functions are only resolved once.**

### What does an EventEmitter instance do?
**EventEmitter is a singleton, means that it is a design pattern that restricts the instantiation of a class to one instance.**

### When is a program’s call stack, event queue, and event loop active?
**It is how the async functions run, where first the first method will pushed inside the call stack and once it needs a time to execute, it will go to the event queue and then finally will invoked at the event loop active where any statement will executing.**

## Document the following Vocabulary Terms
- **_observer pattern_** is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.

- **_Event Handler_** Event handlers can be used to handle and verify user input, user actions, and browser actions such as Things that should be done every time a page loads, and Things that should be done when the page is closed.

- **_Event Driven Programming_** Node. js uses events heavily and it is also one of the reasons why Node. js is pretty fast compared to other similar technologies.

- **_Event Loop_**  has one simple job — to monitor the Call Stack and the Callback Queue. If the Call Stack is empty, it will take the first event from the queue and will push it to the Call Stack, which effectively runs it.

- **_Event Queue_** A JavaScript runtime uses a message queue, which is a list of messages to be processed.

- **_Call Stack_** is a mechanism to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function.

- **_Subscribe_** is an object that represents a disposable resource, usually the execution of an Observable.

- **_database_** is an organized collection of structured information, or data, typically stored electronically in a computer system.