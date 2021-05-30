## Review, Research, and Discussion



- **UDP is often refereed to as a connectionless protocol. Why is this?**
    UDP is a connectionless protocol. It is known as a datagram protocol because it is analogous to sending a letter where you don't acknowledge receipt.

- **Can a socket server application have multiple socket connections?**
    Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to.

- **Can a socket connection application be connected to multiple socket servers?**
    Yes 

- **Can an application be both a socket server and a socket connection?**
 yes! You can do that if you're willing to use two different ports.


## Terms

|Term||
|--|--|
 |Observer Pattern|is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.|
|Listener|a function that is invoked when a particular event occurs, typically with an event object containing information about the event.|
|Event Handler|when the listener is active the event will be fired once and the callback acts as the event handler|
|Event Driven Programming|a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision. |
|Event Loop|The event loop is what allows Node.js to perform non-blocking I/O operations — despite the fact that JavaScript is single-threaded — by offloading operations to the system kernel whenever possible.|
|Event Queue|An event queue is a repository where events from an application are held prior to being processed by a receiving program or system. |
|Call Stack| is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.|
|Emit/Raise/Trigger|Emit's job is to trigger named event(s) which in turn cause functions called listeners to be called.|
|Subscribe|is the easiest way to subscribe either dom events in browser or node.js events.|
|database| is an organized collection of structured information|


## What is the OSI Model?

The OSI Model (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software.

### **The 7 Layers of the OSI Model**


- Physical Layer
- Data Link Layer
- Network Layer
- Transport Layer
- Session Layer
- Presentation Layer
- Application Layer

![aa](https://cehv.com/wp-content/uploads/2021/03/osi-model-7-layers-1024x734-1.jpg)

### TCP Three-Way Handshake Process

TCP traffic begins with a three-way handshake. In this TCP handshake process, a client needs to initiate the conversation by requesting a communication session with the Server:

![](https://i0.wp.com/networksigma.com/wp-content/uploads/2020/08/3-Way-TCP-Handshake.png?fit=1009%2C521&ssl=1)

- **Step 1**: In the first step, the client establishes a connection with a server. It sends a segment with SYN and informs the server about the client should start communication, and with what should be its sequence number.
- **Step 2**: In this step server responds to the client request with SYN-ACK signal set. ACK helps you to signify the response of segment that is received and SYN signifies what sequence number it should able to start with the segments.
- **Step 3**: In this final step, the client acknowledges the response of the Server, and they both create a stable connection will begin the actual data transfer process.

# **Socket`.`io**
![](https://miro.medium.com/max/2792/1*tWm33yhceKIL22QqOORu2w.png)
Socket.IO is a JavaScript library for real-time web applications. It enables real-time, bi-directional communication between web clients and servers. It has two parts: a client-side library that runs in the browser, and a server-side library for node.js. Both components have an identical API.

## Real-time applications
A real-time application (RTA) is an application that functions within a period that the user senses as immediate or current.

![](https://www.medrectech.com/image/rta.png)

Some examples of real-time applications are −

- **Instant messengers** − Chat apps like Whatsapp, Facebook Messenger, etc. You need not refresh your app/website to receive new messages.

- **Push Notifications** − When someone tags you in a picture on Facebook, you receive a notification instantly.

- **Collaboration Applications** − Apps like google docs, which allow multiple people to update same documents simultaneously and apply changes to all people's instances.

- **Online Gaming** − Games like Counter Strike, Call of Duty, etc., are also some examples of real-time applications.

## Why Socket.IO?

Writing a real-time application with popular web applications stacks like LAMP (PHP) has traditionally been very hard. It involves polling the server for changes, keeping track of timestamps, and it is a lot slower than it should be.

Socket.IO is quite popular, it is used by Microsoft Office, Yammer, Zendesk, Trello, and numerous other organizations to build robust real-time systems. It one of the most powerful JavaScript frameworks on GitHub, and most depended-upon NPM (Node Package Manager) module. Socket.IO also has a huge community, which means finding help is quite easy.




