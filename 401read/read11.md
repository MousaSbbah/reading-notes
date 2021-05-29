## Review, Research, and Discussion

- **Why is access control important?**

    Access controls limit access to information and information
    processing systems. When implemented effectively, they mitigate the risk of information being accessed without the appropriate authorisation, unlawfully and the risk of a data breach.


- **Describe an application that would need access control.**

    Social media Groups 
The admin can add and remove member 
the normal user can just write without control the member

- **What is a role used for?**

    To give the permission based on this role



|Term||
|---|--|
|Authorization|the process of giving someone permission to do or have something.|
|Role Based Access Control|systems assign access and actions according to a person's role within the system.|
|Capabilities|the specific permissions that you assign to each user or to a User role.|


# **Event Driven Applications**

Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision. In this article we’re going to go over how Event-Driven Programming works and how we can make the best use of it in our Node.js projects.

## Event Emitters

EventEmitter is a **class** that helps us create a publisher-subscriber pattern in NodeJS.

With an event emitter, we can simply raise a new event from a different part of an application, and a listener will listen to the raised event and have some action performed for the event.

![](https://miro.medium.com/max/2625/1*uFzVNydvSRhSo1JsOyppag.png)
## Creating an Event Emitter

To create an event emitter, we need to create an instance of the event emitter instance from the ``events`` module in NodeJS.

```js
// Import events module
var events = require('events');

// Create an eventEmitter object
var eventEmitter = new events.EventEmitter();

```

### Methods

* addListener(event, listener)
* on(event, listener)
* once(event, listener)
* removeListener(event, listener)
* removeAllListeners([event])
* setMaxListeners(n)
* listeners(event)
* emit(event, [arg1], [arg2], [...])

### Class Methods
* listenerCount(emitter, event)
