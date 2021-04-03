# Node.js

## What Is Node.js?

Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.

## Hello, World!” the Node.js Way
You can check that Node is installed on your system by opening a terminal and typing `node -v`. If all has gone well, you should see something like `v12.14.1` displayed. This is the current LTS version at the time of writing.

Next, create a new file **hello.js** and copy in the following code:
```js
console.log("Hello, World!");
```
This uses Node’s built-in console module to display a message in a terminal window. To run the example, enter the following command:
```cmd
node hello.js
```
If Node.js is configured properly, “Hello, World!” will be displayed.


## The Node.js Execution Model

![Execution Model](https://uploads.sitepoint.com/wp-content/uploads/2012/10/1516152673node_event_loop.png)


## “Hello, World!” — Server Version

```js
const http = require('http');

http.createServer((request, response) => {
  response.writeHead(200);
  response.end('Hello, World!');
}).listen(3000);

console.log('Server running on http://localhost:3000');
```

To run this, copy the code into a file named hello-world-server.js and run it using node hello-world-server.js. Open up a browser and navigate to **http://localhost:3000** to see “Hello, World!” displayed in the browser.


The anonymous function is called with two arguments (`request` and `response`). These contain the request from the user and the response, which we use to send back a 200 HTTP status code, along with our **“Hello World!”** message.

Finally, we tell the server to listen for incoming requests on `port 3000,` and output a message to the terminal to let us know it’s running.

## What Are the Advantages of Node.js?
Aside from speed and scalability, an often-touted advantage of using JavaScript on a web server — as well as in the browser — is that your brain no longer needs to switch modes. You can do everything in the same language, which, as a developer, makes you more productive (and hopefully, happier). For example, you can easily share code between the server and the client.

Another of Node’s big pluses is that it speaks JSON. JSON is probably the most important data exchange format on the Web, and the lingua franca for interacting with object databases (such as MongoDB). JSON is ideally suited for consumption by a JavaScript program, meaning that when you’re working with Node, data can flow neatly between layers without the need for reformatting. You can have one syntax from browser to server to database.



