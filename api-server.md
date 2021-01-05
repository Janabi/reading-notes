# API Server

## Review, Research, and Discussion

### How does route prefixing work with an external routing module?

**By adding at the top level directory in the js route file the following code.**
```
// Our external route
var externalRoutes = require('./routes/externalRoutes');
app.use('/externalRoutes', externalRoutes);
```

### When routing, what’s the difference between app.get('/data/:id') and app.get('/data/:name')?
The differences is that in the request paramters. In the first route, it will take an id as a parameter inside the callback function, however, the second route will take name asa parameter inside its callback function.

### Explain how Express handles routing conflicts?
by taking the first route coming in order that has the same method.

### What are the ways that a browser can send “data” or request variables to an HTTP server
- /category?name=:name --> this way to get it as ````req.query```.
- /category/:name --> this way to egt it as ```req.params```.

## Document the following Vocabulary Terms

- _Routing_ is the way of how the application's endpoits in the URL will respond to the user request.

- _Route Prefixing_ is the way that you will use the same route over the CRUD methodologies.

- _Request Body_ it will get through sending a variables by a post method.

- _Request Params_ it will get from the url route as a paramter.

- _Request Query_ it will get from the url but this time after the question marks.