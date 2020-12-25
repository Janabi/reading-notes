# Node.js
## What does node js exactly mean or do?

**We can describe it as in this [link](https://www.sitepoint.com/an-introduction-to-node-js/) /"Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library./"**

## So what do they mean by non-blocking or event-based?
It means that when you execute a javascript code which it includes a couple of functions, the program will run consecutively all the functions one by one, even if one of these functions contain a time out then it will just jump on the next one until all the function executed, then it will turn out to the time out function to run this lately.
***The figure below will clarify what I am trying to explain***
![Figure](https://uploads.sitepoint.com/wp-content/uploads/2012/10/1516152673node_event_loop.png)

***So whatever you set a time out for a function, the program will not wait until the function works and then will run the rest. instead, it will finish the rest and then come back to it later even if time was already passed!***
**Does that make sense! Cool! Right!**

## So now we can upload node js into our system? 
First of all, you need to install npm on your machine. npm stands for Node Package Manager which includes all the functions, methods that you will be using in all of node js projects. 
**Therefore, open your terminal or command prompt and type the following script:**
```
npm install -g jshint
```

**Then, go to your node js project folder and upload a modules folder where it has all of the packages that you need to run your javascript commands**
**The following command will upload the /"package.json/"**
```
npm init -y
```
**Next will upload the package modules by typing in the terminal**
```
npm install lodash --save
```

### Finally to check that node javascript works perfectly in the project folder.
First, create a javascript file and let it called /"server.js/", Then type the following scripts inside it.
```
const http = require('http');

http.createServer((request, response) => {
  response.writeHead(200);
  response.end('Hello, World!');
}).listen(3000);

console.log('Server running on http://localhost:3000');
``` 
After that go to your terminal and type the following command and you must get inside the terminal the sentence /'Hello, World!/'.
```
node server.js
```