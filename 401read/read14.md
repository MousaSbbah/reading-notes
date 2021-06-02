## Review, Research, and Discussion


- **What’s the difference between a FIFO and a standard queue?**

     Standard queues guarantee that a message is delivered at least once and duplicates can be introduced into the queue. FIFO queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue.

- **How do you test an event driven system?**

    There are multiple levels of tests you will typically write for your system. In the most canonical case, you will write unit tests, service tests, and end-to-end tests. In each of these cases, your System Under Test (SUT, what is actually being tested) comprises a different part of your application.
- **What classic design pattern is best represented by event driven programming?**

    The Singleton Design Pattern


## terms

|term||
|--|---|
|FIFO Queue|FIFO (First-In-First-Out) queues are designed to enhance messaging between applications when the order of operations and events is critical|
|Pub/Sub|an asynchronous messaging service that decouples services that produce events from services that process events.|




#  AWS SNS and SQS

The Amazon Simple Queue Service (SQS) and the Amazon Simple Notification Service (SNS) are important “glue” components for scalable, cloud-based applications (see the Reference Architectures in the AWS Architecture Center to learn more about how to put them to use in your own applications).

One common design pattern is called “fanout.” In this pattern, a message published to an SNS topic is distributed to a number of SQS queues in parallel. By using this pattern, you can build applications that take advantage parallel, asynchronous processing. For example, you could publish a message to a topic every time a new image is uploaded. Independent processes, each reading from a separate SQS queue, could generate thumbnails, perform image recognition, and store metadata about the image:

![](https://media.amazonwebservices.com/blog/sns_sqs_image_proc_2.png)

![](https://miro.medium.com/max/723/1*DRrTtdyah9NHwR0VCm6MWA.png)
