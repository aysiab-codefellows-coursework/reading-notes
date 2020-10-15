# Reading Assignment Nine
*Sections Read:*
- [Functional Code](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)
- [Refactoring Code](https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec)

### Refactoring Code to be Functional 
Functional code is easily readable, and treats programming computation as "the evaluation of mathetical functions and avoids changing-state and mutable data."

Pure funtions are an important part of functional programming. These funcctions should return the same result if given the same arguments; generally, global variables should be avoided without being passed as an argument. 

Immutability is another important part of functional programming, which is why recursion is often recommended to handle iterative actions. The whole point of immutability is so our code becomes predictable and consistent. 

Functional code is at large the reason to use Array.map(), .filter(), .reduce(), .forEach() and arrow codes. 


Below is an example of a function that takes in an argument for an array and multplies all elements by two, returning a new array with the values.
```
function mulitplyByTwo(arr) {
    let ret = [];
    for(let i = 0; i < arr; i++) {
        ret.push(arr[i] * 2)
    }
}
```

This is how the code should be refactored based on the concepts of functional programming.
```
function multiplebyTwo(arr) {
    let ret = arr.map(value => value * 2);
}

```

