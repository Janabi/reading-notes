# Authentication

## Review, Research, and Discussion

### Explain what a “Singleton” is (in Computer Science terms)
its creating a class to one instance.

### Explain how the Singleton pattern can be used with Node modules, specifically with classes
Sigleton pattern is used in the js classes to have the following:
- private constructor.
- having a getInstance method publicly in roder to return the instance of this class.

### If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
It depends on what exactly want the middleware function to implement, then I will build one and export it to the main javascript file where I am going to execute all of the routes including the middleware using the express module.


## Document the following Vocabulary Terms
- **_Router Middleware_** it is goes based on the client URL request and it is way DRYer than the application level middleware. The middleware is a function that have the access to request and response objects and also keep continuing the request-response cycle.

- **_Dynamic Module Loading_** it is an easier way to get the modules by using the import() function. This function will take a string of a scpecified module as a parameter.

- **_Singleton Pattern_** is a software design pattern that make a restriction on any class into one instance.

- **_CRUD -> REST Method Matches_** Create -> Post, Read -> Get, Update -> Put, and Delete -> Delete.

- **_Mock Testing_** it is a method that used to test your code, that its interacting in other system modules.