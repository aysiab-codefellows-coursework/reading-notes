# Reading Assignment 12

### Review, Reseach & Discuss:
> 1. What is the benefit of transforming data into packets?
- Packets allow for more network flexibility since the data is split into independent pieces of another. 

> 2. UDP is often refereed to as a connectionless protocol. Why is this? 
- UPD doesn't need to establish a connection between a client and server to send data. 

> 3. Can a socket server application have multiple socket connections?
- Yes, a socket server applicaiton can have multiple socket connections. 

> 4. Can a socket connection application be connected to multiple socket servers?
- The answer is convoluted, but I do not believe so. Sockets can only listen to a single port, and changing the port wouldn't do anything for this to add multiple socket servers. 

> 5. Can an application be both a socket server and a socket connection?
- Yes! A socket can both send off and listen to events. 

### Define Key Terms
***Observer Pattern:*** a design pattern where an object called the subject maintains a list of objects depending on it (observers) and notifys them of any changes to the state. 
***Listener:*** the listener is apart of the events/sockets object and is responsible for listening to certain events as they are fired off 
***Event Handler:*** this is the function that handles the logic for a given event 
***Event Driven Programming:*** the flow of the app is determined by how events are fired off and recieved 
***Event Loop:*** a design pattern that follows very similarly to a JavaScript synchronous call stack where one event must be executed before another event can be fired off
***Event Queue:*** event queue keeps track of events before they are executed
***Call Stack:*** the call stack is the order of operations for functions before they are executed 
***Emit/Raise/Trigger:*** the syntax for triggering a certain event 
***Subscribe:*** attaching a socket to certain channels 
***Database:*** data storage structure 

### Resources
- [O'Reilly](https://www.oreilly.com/library/view/learning-javascript-design/9781449334840/ch09s05.html)
- [Medium](https://medium.com/@Rahulx1/understanding-event-loop-call-stack-event-job-queue-in-javascript-63dcd2c71ecd)