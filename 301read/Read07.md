# REpresentational State Transfer (REST)
![aa](https://miro.medium.com/max/590/1*TJ0moenk4v9Lr8_Xp192rw.png)
**REST**, or **REpresentational State Transfer**, is an architectural style for providing standards between computer systems on the web, making it easier for systems to communicate with each other. REST-compliant systems, often called RESTful systems, are characterized by how they are stateless and separate the concerns of client and server. We will go into what these terms mean and why they are beneficial characteristics for services on the Web.

## Communication between Client and Server
In the REST architecture, clients send requests to retrieve or modify resources, and servers send responses to these requests. Let’s take a look at the standard ways to make requests and send responses.

## Making Requests
REST requires that a client make a request to the server in order to retrieve or modify data on the server. A request generally consists of:

* an HTTP verb, which defines what kind of operation to perform
* a header, which allows the client to pass along information about the request
* a path to a resource
* an optional message body containing data
### HTTP Verbs
![aa](https://www.edureka.co/blog/wp-content/uploads/2019/06/CRUD-Operations-What-is-REST-API-Edureka-1.png)
There are 4 basic HTTP verbs we use in requests to interact with resources in a REST system:

**`GET`** — retrieve a specific resource (by id) or a collection of resources

**`POST`** — create a new resource

**`PUT`** — update a specific resource (by id)

**`DELETE`** — remove a specific resource by id

![aa](https://miro.medium.com/max/3200/1*HBsBP4Ycvs-0LxGDmqPOJQ.png)



 