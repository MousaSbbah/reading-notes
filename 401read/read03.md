# Express REST API
![](https://i.morioh.com/22dbc45a56.png)
**Name 3 real world use cases where you’d want to change the request with custom middleware**

1. authentication
2. API security
3. Error Handling

 **True or false: The route handler is middleware?**
 
true 

**In what ways can a middleware function end the process and send data to the browser?**

if the function has `res.<method>(data)`


<hr> 


![](https://miro.medium.com/max/642/1*kMNzu4zx40QvwQUWa9dCOw.png)
**Middleware**: Middleware literally means anything you put in the middle of one layer of the software and another. Express middleware are functions that execute during the lifecycle of a request to the Express server. Each middleware has access to the HTTP request and response for each route (or path) it’s attached to.

**Request Object :** The request object allows you to submit a POST or GET request to an URL. Essentially it provides a way to make REST API requests to another URL.




**Response Object :** The response object represents the HTTP response that an Express app sends when it gets an HTTP request.

**Application Middleware :** We can run middleware functions used when any routes are called by passing them to the `app.use` method as a callback.

**Routing Middleware :** works the same way as app-level middleware, but they’re bound to the instance of the express.Router() instead of the express instance.



![](https://blog.testlodge.com/wp-content/uploads/2018/04/tdd_v_bdd_cycle-1024x538.png)

**Test Driven Development :** is an evolutionary approach to development which combines test-first development where you write a test before you write just enough production code to fulfill that test and refactoring. In simple terms, test cases are created before code is written.

**Behavioral Testing :** 
Black Box Testing is known as Behavioral Testing. The testing of external behavior of the program is known as Black Box Testing.  It can be applied in software and any program. The main aim of black box testing is what is input and what gets output. The black box used to get different types of Errors such as function missing, Usability, Performance, Concurrency and timing Problems, Initializing and terminating errors etc. One of the Best examples of Black Box Testing is Calculator. It takes inputs from the user and shows outputs directly.


<hr>
<hr>

```
Which 3 things had you heard about previously and now have better clarity on?

    - middleware , routing and Testing

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    - Errors handler , REST and more about middleware
What are you most excited about trying to implement or see how it works?
    real world cases for the middleware 
```