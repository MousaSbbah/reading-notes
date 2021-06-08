## Review, Research, and Discussion


**List the AWS Database offerings and talk about the pros and cons of each**
- Relational
- Key-value	
- In-memory	
- Document	
- Wide-column	
- Graph
- Time series	
- Ledger

**A pros and cons :** list is a simple but powerful decision-making tool used to help understand both sides of an argument. Pros are listed as arguments in favor of making a particular decision or action. Cons are listed arguments against it.

**Pros and cons list examples**


- **Examples of Pros:**

New car is safer

New car gets better gas mileage

New car has more cargo space 

- **Examples of Cons:**

New car is expensive

Old car runs fine

Insurance will cost more on the new car

In the above example, you see that both sides of the argument or decision are being weighed out. This will help the person decide on whether or not purchasing the new car is a good decision. 
**What’s the difference between a FIFO and a standard queue?**

Standard queues guarantee that a message is delivered at least once and duplicates can be introduced into the queue. FIFO queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue.

**How can the server be assured a message was properly received?**

## Document the following Vocabulary Terms

|Term||
|--|--|
|Serverless API|Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers. A serverless application runs in stateless compute containers that are event-triggered, ephemeral (may last for one invocation), and fully managed by the cloud provider.|
|Triggers|are pieces of code that will automatically respond to any events in DynamoDB Streams. Triggers allow you to build applications that will then react to any data modification made in DynamoDB tables. By enabling DynamoDB Streams on a table, you will be able to associate an ARN with your Lambda function.|
|Dynamo vs Mongo|1. MongoDB is vendor agnostic, Open Source, and can be deployed anywhere. DynamoDB is only available on AWS.// 2. DynamoDB is a fully managed AWS service, MongoDB can be self installed or fully managed with MongoDB Atlas.///3. DynamoDB as an integrated AWS service makes it easier to develop end to end solutions.///4. DynamoDB uses tables, items and attributes, MongoDB uses JSON-like documents.//5. DynamoDB supports limited data types and smaller item sizes; MongoDB supports more data types and has fewer size restrictions.|
|Dynamoose vs Mongoose|Dynamoose is a modeling tool for Amazon's DynamoDB (inspired by Mongoose).|


# SQS 

Amazon Simple Queue Service (SQS) is a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications. SQS eliminates the complexity and overhead associated with managing and operating message oriented middleware, and empowers developers to focus on differentiating work. Using SQS, you can send, store, and receive messages between software components at any volume, without losing messages or requiring other services to be available. Get started with SQS in minutes using the AWS console, Command Line Interface or SDK of your choice, and three simple commands.

SQS offers two types of message queues. Standard queues offer maximum throughput, best-effort ordering, and at-least-once delivery. SQS FIFO queues are designed to guarantee that messages are processed exactly once, in the exact order that they are sent.

## Benefits

- Eliminate administrative overhead
- Keep sensitive data secure
- Reliably deliver messages
- Scale elastically and cost-effectively

# SNS
Amazon Simple Notification Service (Amazon SNS) is a fully managed messaging service for both application-to-application (A2A) and application-to-person (A2P) communication.

The A2A pub/sub functionality provides topics for high-throughput, push-based, many-to-many messaging between distributed systems, microservices, and event-driven serverless applications. Using Amazon SNS topics, your publisher systems can fanout messages to a large number of subscriber systems including Amazon SQS queues, AWS Lambda functions and HTTPS endpoints, for parallel processing, and Amazon Kinesis Data Firehose. The A2P functionality enables you to send messages to users at scale via SMS, mobile push, and email.

## Benefits

- Modernize and decouple your applications
- Send messages directly to millions of users
- Reliably deliver messages
- Automatically scale your workload
- Ensure accuracy with message ordering and deduplication
- Simplify your architecture with Message Filtering
## How it works

- **Pub / Sub**

![](https://d1.awsstatic.com/diagrams/Product-page-diagram-Amazon-SNS_event-driven-SNS-compute%402X_.4b9c0a75aa40bda9cdb12f0176930a12da2872bf.png)

# SNS vs SQS

**SNS** is a distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS.

**SQS** is distributed queuing system. Messages are not pushed to receivers. Receivers have to poll or pull messages from SQS. Messages can't be received by multiple receivers at the same time. Any one receiver can receive a message, process and delete it. Other receivers do not receive the same message later. Polling inherently introduces some latency in message delivery in SQS unlike SNS where messages are immediately pushed to subscribers. SNS supports several end points such as email, SMS, HTTP end point and SQS. If you want unknown number and type of subscribers to receive messages, you need SNS.








