# Reading Assignment Ten
*Read:*
- [MDN Callstack](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)
- [JavaScript Callstack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

### The Call Stack
The call stack is like an recipe but for code. Executing one function at a time, especially within single threaded interpretors such as JavaScript. This is known as synchronous.

The best way of visualizing the call stack is by looking at some code. 


```
function telephone() {
    console.log('Ring, ring!')
    personA()

}

function personA() {
    personB();
    console.log('No, this is Patrick');
}

}

function personB() {
    console.log('Is this the Krusty Krab?')
}

telephone();
```
Our console would log:
- Ring ring!
- Is this the Krusty Krab?
- No, this is Patrck. 

But what is realyl happening beneath the surface? Well... 

The first thing that happens is we call `telephone()`. This function get added to the stack, and our interpretor will then go down line by line `console.log('Ring, ring!')` before calling `personaA()`. `personaA()` then gets added to the stack after `telephone()`, reading line by line to call `personaB()`. When `personB()` gets called our interpretor will then read `console.log('Is this the Krusty Krab?')`. After that, `personB()` is fulfilled and popped off from our call stack. We return to the last function that called it `personA()` and fulfill the `console.log('No, this is Patrick')`. `personA()` is now popped off the stack leaving our first call of `telephone()`, but now that the last line of code in the function has been called, `telephone()` finally gets popped off the stack. Despite being the first one called, telephone is the last one to go. 

The call stack works on a Last In, First Out basis (LiFo).