# Reading Assignment Six
*Sections Read:*
- [Intro to Node.JS](https://www.sitepoint.com/an-introduction-to-node-js/)

### What is Node.js?
According to StackOverflow:
> Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.

This does not mean that Node.js runs in Google's Chrome browser, but rather is build upon the same engine that Chrome uses. At its simplest definition, Node.JS is a JavaScript runtime. 

In your terminal, you should be able to use `node my_file_name.js` and as long as Node.JS is configured properly, the file will run. 

### What is the most common use case for Node.js?
While there are *many*, the most common use case for Node.js is running JavaScript on the server. Node.js is single threaded and more importantly even-driven. 

Because Node's execution model is single threaded and event driven, it causes very little overhead in the server. Node also seaks well with JSON which is what makes it so popular. 

Node is suited well to build applications that have some form of live or real time interaction. It's good at building APIs that handle a large amount of requests that are I/O driven. 