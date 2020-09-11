# Class 10: Reading Assignment 10
*Sections read:*
- Ch. 10 (JavaScript&JQuery)

### Error Handling & Debugging
1. JavaScript reads code _______________. Sometimes a line of code will call for a function, JavaScript will ____________ on top of it's current task. 
2. **True or False:** Exceptions are JavaScript statements that execute for a given anticipated error. 
3. **True or False:** There are five built-in error objects in JavaScript. 
4. **Name:** two built-in JavaScript error objects 
5. What error would this code throw?
```
var colors = ['blue','red','purple 'orange', 'green'];
```
6. Which three statements can be used to handle errors gracefully?
7. **True or False** the JavaScript console in your web broser can tell you where the problem is with a script via line number. 
8. What is the use of a breakpoint in debugging?
9. How does `try`, `catch`, `finally` work?
```
try {
    // what does try do?
} catch (exception) {
    // what does catch do?
} finally {
    // what does finally do?
}

```
10. What is the syntax for creating your own error?

<hr />

### Answers
1. One line at a time, stack 
2. True
3. False
4. Accepted answers: `error`, `SyntaxError`, `ReferenceError`, `TypeError`, `RangeError`, `URIError`, `EvalError`
5. `SyntaxError: Expected Token ']'`
6. `try`, `catch`, `throw`, `finally`
7. True
8. Breakpoints are used to pause the execution of a script at a given line. 
9. `try`: this code will try to execute first, `catch (exception)`: if there is an exception then this code will also be ran, `finally` this code always get run regardless of the success or failure of the `try`
10. `throw new Error('error message')`