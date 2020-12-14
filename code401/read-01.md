 # Reading Assignment 01

### Array.map & Array.reduce
*Simple definitions:* The `Array.map()` is an integrated method within the Array object in JavaScript that creates a a new array by using a callback function on the data from the original array.

`Array.reduce()` can be used similarly to produce a single output after executing a callback function on the values of the original array.


**EXAMPLE**
```
let pets = [{"name": "mr. peanutbutter", "age": 1, "type": "dog"},{"name": "princess carolyn", "age": 5, "type": "cat"}.{"name": "bojack", "age": 12, "type": "horse"}]

// array.map() to create a new array of only the names
let names = pets.map(pet => pet.name)

// names should now be 
// ["mr. peanutbutter","princess carolyn","bojack"]

// array.reduce() to find the oldest age of any of the pets 
let oldest = pets.reduce((accum, pet) => {
    if(accum < pet.age) {
        accum = pet.age;
    }
}, 0)

// oldest should be equal to 12
```

***`superagent` examples***
```

let url = 'https://swapi.dev/api/people'

// .then
function getCharacters(url) {
    superagent.get(url)
    .then(data => {
        let characters = JSON.parse(data.text);
        characters = characters.results;
        console.log(characters);
    })
}

// await async 
function async getCharacters(url) {
    let rawData = await superagent.get(url);
    rawData = JSON.parse(rawData.text)
    let characters = rawData.results
    console.log(characters)
}

```
***Promises***
Promises are a JavaScript object that return a value sometime in the future. They promise to return something at some point *later*. They have 3 states: resolve, reject and then. Resolve means the promise succeeded, rejected means the promise failed, and .then allows you to continue to do logic with the returned value. 

[MDN on promises](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)

***Are all callbacks async?***
No, not all callback fuctions are async. Callback functions that involve external resources and data tend to be async, but other callback functions that handle simple logic are not.  

[Scotch.io article](https://scotch.io/courses/10-need-to-know-javascript-concepts/callbacks-promises-and-async) on promises, callbacks & async 