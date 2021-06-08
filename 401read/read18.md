## Review, Research, and Discussion
In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

**What are serverless functions?**

A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

**If you were to create a system that emulated Lambda functions, how would you do it?**
- Open the Functions page on the Lambda console.

- Choose Create function.

- Under Basic information, do the following:

    - For Function name, enter my-function.

    - For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell,C#) Go, Java, Node.js, Python, and Ruby.

- Choose Create function.
**Describe how a CDN works**

A CDN (Content Delivery Network) is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user. 
## Document the following Vocabulary Terms
|Term||
|--|---|
|Serverless Functions|A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.|
|Cloud Storage|Cloud storage is a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service. It’s delivered on demand with just-in-time capacity and costs, and eliminates buying and managing your own data storage infrastructure. This gives you agility, global scale and durability, with “anytime, anywhere” data access.|
|CDN|A CDN (Content Delivery Network) is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user. |

# AWS: API, Dynamo and Lambda

## Amazon API Gateway

Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. APIs act as the "front door" for applications to access data, business logic, or functionality from your backend services. Using API Gateway, you can create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications. API Gateway supports containerized and serverless workloads, as well as web applications.

### API Types
- RESTful APIs
- WEBSOCKET APIs

###  How API Gateway Works
![](https://d1.awsstatic.com/serverless/New-API-GW-Diagram.c9fc9835d2a9aa00ef90d0ddc4c6402a2536de0d.png)


## Amazon DynamoDB

Amazon DynamoDB is a key-value and document database that delivers single-digit millisecond performance at any scale. It's a fully managed, multi-region, multi-active, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications. DynamoDB can handle more than 10 trillion requests per day and can support peaks of more than 20 million requests per second.

### Benefits
- Performance at scale
- No servers to manage
- Enterprise ready

### **Dynamoose**


Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.

#### **Key Features**
- Type safety
- High level API
- Easy to use syntax
- Ability to transform data before saving or retrieving documents
- Strict data modeling (validation, required attributes, and more)
- Support for DynamoDB Transactions
- Powerful Conditional/Filtering Support
- Callback & Promise support
