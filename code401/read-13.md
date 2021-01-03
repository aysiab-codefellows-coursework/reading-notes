# Reading Assignment 13

### Review, Research & Discuss:
> 1. What does it mean that web sockets are bidirectional? Why is this useful?
- Bidirectional refers to the fact that a single port can both recieve event data and send event data. Bidirectionality allows for async responses. 
> 2. Does socket.io use HTTP? Why?
- HTTP is needed for the initial set up of connecting to a socket port. 
> 3. What happens when a client emits an event?
- This usually happens within the callback function of the client listening to another event. The event along with the data is then emitted to the server to handle. 
> 4. What happens when a server emits an event?
- The server only knows how to emit events, and respond to events coming from the client. 
> 5. What happens if a client “misses” an event?
- An event would only really be missed if there wasn't a client to listen for it. 
> 6. How can we mitigate this?



### Define Key Terms 
***Socket:*** is a designated endpoint on a server port 
***Web Socket:*** the client side socket 
***Socket.io:*** a JavaScript library that allows for data to be sent between a sever and client on an event basis 
***Client:*** Client is the web broswer where the user's rquests are sent from to a server 
***Server:*** Server side is where a program then can connect to, recieve, manipulae and send data back to a client with a response 
***OSI Model:*** shorthand for Open System Interconnection Model, and is a framweork "used to describe the functions of a netwroking system." There are 7 layers involved. 
***TCP Model:*** shorthand for Transmission Control Protocol, has 4 layers and is a more concise and reliable verison of the OSI model. 
***TCP:** Transmission Control Protocol 
***UDP:** User Datagram Protocol 
***Packets:*** small segment of data with a designated source, destination and information. Sent over UDP. 

### Resources
- [Forcepoint on OSI](https://www.forcepoint.com/cyber-edu/osi-model) 
- [Geeks For Geeks TCP](https://www.geeksforgeeks.org/tcp-ip-model/)