# Reading Assignment 6
*Materials Reviewed*
- [Securing Passwords]()
- [Basic Auth]()
- [OWASP Auth Cheat Sheet]()
- [bcrypt docs]()

### Review, Research & Discuss
> 1. Explain what a “Singleton” is (in Computer Science terms)
- A singleton is an object that can only be instantiated one time. 

> 2. Explain how the Singleton pattern can be used with Node modules, specifically with classes
- A singleton pattern will make a single (hence singleton) instance of the object within a class. This single instance can be used to pass information around in the application. 


> 3. If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
- Determining middleware depends on the type of application I'm building. However, if I were to start building middleware, I would determine it's single function that needs to be applied to the other parts of the application, and attempt to build tests first following the TDD suggested guidelines before diving into the middleware itself. 


*Additional Resources*:
- [Singleton in JS](https://www.sitepoint.com/javascript-design-patterns-singleton/)


### Definitions 
**Router middleware:** router middleware performs the same as any other application middleware. This middleware is a apart of Express. 

**Dynamic module loading:** importing modularized code between files using `module.exports` and requiring them

**Singleton pattern:** restricts the instantiation of a class to a *single* object. 

**CRUD:** create, read, update, and delete.

**Mock testing:** mock testing is a way of unit testing that allows you make test assertions witout actually interacting with your actual server or database for example.