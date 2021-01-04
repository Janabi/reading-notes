# Express Routing & Connected API

## Review, Research, and Discussion

### Name 3 real world use cases where you’d want to change the request with custom middleware
- Middleware function myLogger
- Middleware function requestTime
- Middleware function validateCookies

### True or false: The route handler is middleware?
- True

### In what ways can a middleware function end the process and send data to the browser?
when you will not call the next() function, then simply the request - response cycle will end up early.

### At what point in the request lifecycle can you “inject” middleware?
it's going to be in the middle of getting the request routes and the callback function that handle the request and give the response object.

### What can cause express to error with “Request headers sent twice, cannot start a second response”
The error "Error: Can't set headers after they are sent." means that you are either in the body or finished state. When you got this kind of error, then go to check the anything that is related to the header that you already sent.

## Document the following Vocabulary Terms

- ***Middleware -*** it is a block of codes that can let you access the request and response objects, also you can do the next to go executing other middleware functions.

- ***Request Object -*** it is an object that either get it as a queries from the requested url or parameters in the url also. So then we can use them to decide the next functionality will be.

- ***Response Object -*** it is an object that the developer will send it as a json or string that might be you will add them to the app's database.

- ***Application Middleware -*** is applied by using either app.use or app.Method where Method means the CRUD verbs - (get, post, put, and delete).

- ***Routing Middleware -*** is applied by using the express router, like router.use or router.Method where Method means the CRUD verbs - (get, post, put, and delete).