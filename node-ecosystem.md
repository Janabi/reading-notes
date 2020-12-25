# Node Ecosystem

## Array.map()
**It is used to iterate each element in the array and create a new array with the samelength as the previous one. It is good to make a certain change within each element inside the array without harming the original one.**
***Let's take an example:***
```
let numbers = [9, 11, 8, 4, 5];

let newNum = numbers.map(num=>{ num*2 });
// newNum = [18, 22, 16, 8, 10]
// numbers  = [9, 11, 8, 4, 5]
```

## Array.reduce()
**It is used to reduce the elements of an array into different output based on the condition and data type that you want to get.**
***Let's take an example:***
```
let numbers = [9, 11, 8, 4, 5];

let evenNum = numbers.reduce((acc, val)=>{
    if(num % 2 === 0) {
        return num;
    }
}, [])
// numbers = [9, 11, 8, 4, 5]
// evenNum = [8, 4]
```

## Superagent
**It is a client-side request library that will request a certain data from specific API and later response it to the browser.**
**So what does _promise_ esactly mean? Promise as it means when you want a certain result to recieve whatever the time will take, that's what exactly happen behind the sence with promises in javascript.**
***Lets take a look at how to write a 'superagent' syntax:***
```
function cityLatLong(cityName) {
  try {
    // getting the lattiude and logitude from geocode API at a certain city name.
    let data = superagent.get(`https://geocode.xyz/${cityName}?json=1`)
    console.log(`Lat: ${data.body.latt},`, 
                `Long: ${data.body.longt}`
                );
  } catch(err) {
    // print out any error if you got it
    console.error(err)
  }
}
```

***So now let us use async/await which both means that 'async' the function that you used is only returning promises and 'await' will make the javascript wait until the promises return results.***

```
async function cityLatLong(cityName) {
  try {
    let data = await superagent.get(`https://geocode.xyz/${cityName}?json=1`)
    console.log(`Lat: ${data.body.latt},`, 
                `Long: ${data.body.longt}`
                );
  } catch(err) {
    console.error(err)
  }
}
```

## Are all callback functions considered to be Asynchronous? Why or Why Not?
No, for several reasons:
- The asynchronous functions are only those who require a data from external resources.
- The rest may or may not be asynchronous such as array.forEach(), array.sort(), String.replace() and others are synchronous functions.