# Reading Assignment 03
*Read:*
- [Review: ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)
- [Using Express Routing](https://expressjs.com/en/guide/routing.html)
- [Express Routing](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4)

### Review, Research & Discussion:
> 1. Name 3 real world use cases where you’d want to change the request with custom middleware:
- To validate names, zipcodes, and to format the request object. 

> 2. True or false: The route handler is middleware?
- Not entirely true, and not entirely false. It is more of a handler than anything else.

> 3. In what ways can a middleware function end the process and send data to the broswer?
- Validator middleware for say a password. If the password doesn't meet the validator requirements it will send back a response saying there was an error. 

> 4. At what point in the request lifecycle can you "inject" middleware?
 - Middleware can be injected at any given time during the request life cycle. Middleware methaphorically speaking act as signposts along the way. 

 > 5.What can cause express to error with "Request headers sent twice, cannot start a second response"?
 - I believe I rant into this exact error because I had an wrongly placed `next()`

Additional sources:
- [Tutorials Point](https://www.tutorialspoint.com/expressjs/expressjs_middleware.htm)
- [Medium](https://medium.com/@agoiabeladeyemi/a-simple-explanation-of-express-middleware-c68ea839f498)

 ### Vocabulary Terms
1. Middleware: Scripts that are added onto the server to handle additional tasks. 
2. Request Object: is used to gather and send infromation from the client/frontend to the server. 
3. Response Object: the returned information/tasks sent back to the client/frontend from the server. 
4. Application Middleware: Examples of application middleware are authenticators, validators, loggers. 
5. Routing Middleware: Express inherently has a Router method that helps handle routing. We used it in Lab 03. 
6. Test Driven Development: a development style where tests are derived first. This better helps a developer consider what the code is actually supposed to be doing. 
7. Behavioral Testing: human readable scripts that are able to test the functionality of your code. (Also known as Black Box Testing)