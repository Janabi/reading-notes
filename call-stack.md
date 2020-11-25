# The Call Stack
## The definition of the call stack bsaed on [Mozilla](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack) Javascript

***/"is a mechanism for an interpreter o keep track of its place in a script that calls multiple functions/"***

Lets take an example about that.
```
function greeting() { //second
   // Calling the sayingHello() function
   sayingHi(); //third
}
function sayingHi() { // fourth
   return "Hello Everyone!"; // fifth
}

// Invoke the `greeting` function
greeting();//first

```

- As we can see by following the steps of how the call stack start and end. it jumped into the last line of invoking the **greeting** function. Then start at the first line to run that function, however, there is an invoking of another function inside the **greeting** function which is **sayingHello** function.
- Therefore, **sayingHello** function will go into its function by returning the string \'Hello Everyone!\', then this statement will return in the **greeting** function again at sayingHello. and it will immediately print to us the statement Hello Everyone.

So to undertand more, take a careful look at the following figure and then read the net statement.
![figure1](https://cdn-media-1.freecodecamp.org/images/QgR2uIk7tW0YNz0Xm8g0jAPeRFI0e4sCejsv)
**The figure above describe how the call stack works, it first push the invoked function in the top of the stack and then after this function return a value, the call stack will poped it outside the stack and bring the next invoked function without stopping the procedure.**

The refereces for this note which goes for the following links:
- [link](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)
- [link](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)