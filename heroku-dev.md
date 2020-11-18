# Heroku Development
## What is Heroku? What is the point of using it?

The Heroku is a cloud platform that will give you a global server where you can deploy your website and everyone in this world can see it.

**First you need to check if you have Haroku and node in your machine by using terminal. Therefore, you can create a local server by writing the following couple of codes inside a file hwere you can name it whatever you like or maybe server.js**
```
var http = require("http");

http.createServer(function(request, response) {
  response.writeHead(200, {"Content-Type": "text/plain"});
  response.write("It's alive!");
  response.end();
}).listen(3000);
```

***In order to make it world wide and everybody in this world can see it. Then you can apply the following codes:***
```
var http = require("http");
var fs = require("fs");
var path = require("path");
var mime = require("mime");
```
Firstly, we declare some variables like those responsible for HTTP functionality, how it going to interact with the file system, allow to handle the file path and lastly define the content type of file "MIME-type".

Then, we create a json file and fill it with the information regarding of the plug-in with MIME-type.
```
{
  "name" : "blog",
  "version" : "0.0.1",
  "description" : "My minimalistic blog",
  "dependencies" : {
    "mime" : "~1.2.7"
  }
}
```

***The follwoing codes are needed to send an error if there is any problem with the internet connection and otherwise send it to display the page.***
```
function send404(response) {
  response.writeHead(404, {"Content-type" : "text/plain"});
  response.write("Error 404: resource not found");
  response.end();
}
```
```
function sendPage(response, filePath, fileContents) {
  response.writeHead(200, {"Content-type" : mime.lookup(path.basename(filePath))});
  response.end(fileContents);
}
```

***Finally, we just need to create an HTTP server to run our website perfectly.***
```
var server = http.createServer(function(request, response) {
  var filePath = false;

  if (request.url == '/') {
    filePath = "public/index.html";
  } else {
    filePath = "public" + request.url;
  }

  var absPath = "./" + filePath;
  serverWorking(response, absPath);
});
```