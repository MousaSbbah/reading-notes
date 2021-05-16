# Express

### Q and A 

**1. What is difference between put and patch?**

|Put|	Patch|
|--|--|
|The embedded entity is believed to the modified version of the resources that are deposited on the original server. It is requested to the client to replace the stored is substituted.|	In this, the information regarding the way of modifying the original server which has the resources to produce a new version is found.|
|At the time of updating the resource, you need to forward full payload as the request.|At the time of updating the resource, you only need to send the parameter of the resource which you want to update.|



**2. Provide links to 3 services or tools that allow you to “mock” an API for development like `json-server`**

* [Postman Mock Server](https://learning.getpostman.com/docs/postman/mock-servers/setting-up-mock/)
* [MockServer](http://www.mock-server.com/)
* [Beeceptor](https://beeceptor.com/)

**3. Compare and contrast Swagger and APIDoc.js**


* **Popularity**: By comparing stats,  swagger-ui is more popular then apidocjs.
* **Consistency**: If we already using swagger for our Dotnetcore service, then implementing swagger tool will consist more from Info and UI prospective.
* **Implementation** complexity: apidocjs and swagger both required documentation content on implemented method as customize comment data. In addition they allow to write documentation data in separate resource file as .js and .json. If we already have swagger.json created by DotnetCore we can reuse more than 80% specification.
 * **Maintenance**: For apidocjs will have to modify documentation for each affected method/endpoints if service changed. In swagger we can limit changes. But by implementing apidocjs we can isolate the layer.
* **Other benefits**: Because swagger use plain .json that could be parsed through programing language, thus we can get advantage of various other 3rd parties in order to create http client and more. 
* **Future:** Due to popularity of swagger, apidocjs provide information about apidoc-swagger converter so we can switch apidoc to swagger anytime.



**4. Which HTTP status codes should be sent with each type of (un)successful API call?**

**4xx**

4xx errors are client-based errors. These errors usually occur when a service exists and a successful connection has been established with an API endpoint, but the request does not contain all of the information it requires to 'understand' the request.


**5. Compare and contrast SOAP and ReST**

**What is SOAP?**

SOAP is a protocol which was designed before REST and came into the picture. The main idea behind designing SOAP was to ensure that programs built on different platforms and programming languages could exchange data in an easy manner. SOAP stands for Simple Object Access Protocol.

**What is REST?**

REST was designed specifically for working with components such as media components, files, or even objects on a particular hardware device. Any web service that is defined on the principles of REST can be called a RestFul web service. A Restful service would use the normal HTTP verbs of GET, POST, PUT and DELETE for working with the required components. REST stands for Representational State Transfer.


##  What is NPM?

npm is the world's largest software registry. Open source developers from every continent use npm to share and borrow packages, and many organizations use npm to manage private development as well.

![npm](https://www.callicoder.com/assets/images/post/large/npm-package-manager-for-node-js.jpg)


## What is TDD?


“Test-driven development” refers to a style of programming in which three activities are tightly interwoven: coding, testing (in the form of writing unit tests) and design (in the form of refactoring).

It can be succinctly described by the following set of rules:

* write a “single” unit test describing an aspect of the program
* run the test, which should fail because the program lacks that feature
* write “just enough” code, the simplest possible, to make the test pass
* “refactor” the code until it conforms to the simplicity criteria
* repeat, “accumulating” unit tests over time