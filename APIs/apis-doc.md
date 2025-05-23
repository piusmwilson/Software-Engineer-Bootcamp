# Application Programming Interfaces(APIs)

## Table Of Contents

- [Introduction](#introduction)
- [What is an Application Programming Interfaces](#what-is-an-application-programming-interfaces)

## Introduction

As an integral part of modern development, Application Programming Interfaces (APIs) allow software applications to communicate and use functions from other software applications or services. This documentation has been curated from researched information on APIs from various sources as well as learning resources. My goal is to have it inform beginners seeking knowledge on APIs as well as a reference point for API related information.

As an API Designer you should be able to;-
- Describe how APIs help customers consume digital information
- Describe the stages of the API lifecycle
- Summarize the various API styles, along with their advantages and limitations
- Elaborate on the principles of good design and catering to the developer experience
- Overcome common API design challenges
- Outline the processes involved in architecting an API
- Describe how to perform effective change management for your APIs


## What is an Application Programming Interfaces

An Application Programming Interfaces (API) is a software interface that connects different applications and systems as they share information and other resources. Its a building block that works behind the scenes to expose the resources of one software application/system to another enabling seamless intergration.

APIs, provide a manner in which software applications communicate with each other by abstracting the complexity of applications to allow developers to use only the essentials of the software they are working with.

They define the methods and data formats an application should use in order to perform tasks, like sending, retrieving, or modifying data. APIs also allow applications to exchange data and functionality with ease, thus enabling integration and convergence of technological services. 

In the context of APIs, the word Application refers to any software with a distinct function. Interface can be thought of as a contract of service between two applications. This contract defines how the two communicate with each other using requests and responses. Their API documentation contains information on how developers are to structure those requests and responses.

API architecture is usually explained in terms of client and server. The application sending the request is called the client, and the application sending the response is called the server.

## What are the different types of APIs?

APIs are classified both according to their architecture and scope of use. We have already explored the main types of API architectures so let’s take a look at the scope of use.

Private APIs
These are internal to an enterprise and only used for connecting systems and data within the business.

Public APIs 
These are open to the public and may be used by anyone. There may or not be some authorization and cost associated with these types of APIs.

Partner APIs 
These are only accessible by authorized external developers to aid business-to-business partnerships.

Composite APIs 
These combine two or more different APIs to address complex system requirements or behaviors. 

## How do APIs work?

API architecture is usually explained in terms of client and server. The application sending the request is called the client, and the application sending the response is called the server.

**There are four different ways that APIs can work depending on when and why they were created.**

### SOAP APIs 
These APIs use Simple Object Access Protocol. Client and server exchange messages using XML. This is a less flexible API that was more popular in the past.

### RPC APIs
These APIs are called Remote Procedure Calls. The client completes a function (or procedure) on the server, and the server sends the output back to the client.

### Websocket APIs
Websocket API is another modern web API development that uses JSON objects to pass data. A WebSocket API supports two-way communication between client apps and the server. The server can send callback messages to connected clients, making it more efficient than REST API.

### REST APIs
These are the most popular and flexible APIs found on the web today. The client sends requests to the server as data. The server uses this client input to start internal functions and returns output data back to the client. 

REST stands for Representational State Transfer. REST defines a set of functions like GET, PUT, DELETE, etc. that clients can use to access server data. Clients and servers exchange data using HTTP.

The main feature of REST API is statelessness. Statelessness means that servers do not save client data between requests. Client requests to the server are similar to URLs you type in your browser to visit a website. The response from the server is plain data, without the typical graphical rendering of a web page.

#### What are the benefits of REST APIs?
REST APIs offer four main benefits:

1. **Integration** 
APIs are used to integrate new applications with existing software systems. This increases development speed because each functionality doesn’t have to be written from scratch. You can use APIs to leverage existing code.

2. **Innovation** 
Entire industries can change with the arrival of a new app. Businesses need to respond quickly and support the rapid deployment of innovative services. They can do this by making changes at the API level without having to re-write the whole code.

3. **Expansion**
APIs present a unique opportunity for businesses to meet their clients’ needs across different platforms. For example, maps API allows map information integration via websites, Android,iOS, etc. Any business can give similar access to their internal databases by using free or paid APIs.

4. **Ease of maintenance**
The API acts as a gateway between two systems. Each system is obliged to make internal changes so that the API is not impacted. This way, any future code changes by one party do not impact the other party.

#### How to secure a REST API?
All APIs must be secured through proper authentication and monitoring. The two main ways to secure REST APIs include:

1. **Authentication tokens** 
These are used to authorize users to make the API call. Authentication tokens check that the users are who they claim to be and that they have access rights for that particular API call. For example, when you log in to your email server, your email client uses authentication tokens for secure access.

2. **API keys** 
API keys verify the program or application making the API call. They identify the application and ensure it has the access rights required to make the particular API call. API keys are not as secure as tokens but they allow API monitoring in order to gather data on usage. You may have noticed a long string of characters and numbers in your browser URL when you visit different websites. This string is an API key the website uses to make internal API calls.

## What are API integrations?

API integrations are software components that automatically update data between clients and servers. Some examples of API integrations are when automatic data sync to the cloud from your phone image gallery, or the time and date automatically sync on your laptop when you travel to another time zone. Enterprises can also use them to efficiently automate many system functions.

## What is an API endpoint and why is it important?
API endpoints are the final touchpoints in the API communication system. These include server URLs, services, and other specific digital locations from where information is sent and received between systems. API endpoints are critical to enterprises for two main reasons: 

1. Security
API endpoints make the system vulnerable to attack. API monitoring is crucial for preventing misuse.

2. Performance
API endpoints, especially high traffic ones, can cause bottlenecks and affect system performance.

## What is an API gateway?
An API Gateway is an API management tool for enterprise clients that use a broad range of back-end services. API gateways typically handle common tasks like user authentication, statistics, and rate management that are applicable across all API calls.

## API Design, API Architrcture

The term "API design" or "API Architecture" refers to the process of developing a software interfrace that exposes backend data and application functionality for use in new applications. This includes the process of bridging between your APIs and developers to enable the creation of applications that allow the end users to consume the APIs.

### API Design

a solid understanding of what APIs are forms the basic cornerstone of API design. 

API design, as a key part of any software development process thus,

- Its basics encompass  _understanding the principles of what an API is, how it works, and the various types of APIs, such as REST, SOAP, and GraphQL_. 
- It also includes _understanding the standards and best practices in API design to ensure the development of powerful, user-friendly, and secure APIs_. 

The foundation of API Design lies in this knowledge, setting the stage for more complex API designing and development.

### Requirements of a Well-Designed API

- Security, the APi should be protected against attacks and misuse.
- Usability, The API should be easy for developers to leverage effectively.
- Scalability, The API should be able to handle rapid spikes in traffic.
- Testability, The API should be designed in a way that it helps developers experiment with functionality.
- Reliability, The API should be robust enough to minimize downtime.

Dividing an API architecture into layers simplifies the process of interface design, where each equality is abstracted away from API implementation and handled in a centralised server architecture, which can then be used across multiple interfaces.
These layers can be **_the security layer, caching layer, representation layer, orchestration layer_**.

### Steps of a Basic API Design Approach

- Start by determining the goals of the API.
- Then Identify the intended users.
- Proceed to design the interfaces.
- Evaluate progress.
- the go on to implement.

### API Styles or standards

**Standards** are usually formal documents that establish uniform engineering or technical criteria, methods, processes, and practices. Organisations that define internet standards include;- IETF(_HTTP, URI,Basic Auth_), W3C(_SOAP, HTML,RDF_), OASIS(_ebXML,DocBook,WS-Security_) while **Styles** refer to abstract plans or conventions for the construction of an object or a system, such as architectural blueprints, engineering drawings or business processes.

When designing APIs, its important to think about what style of API would be most suitable for your organisation, business or innovation initiatives.
Similar to  architecture, when designing buildings in construction, various architectural styles also exsist when designing APIs and using a predifined solution structure helps speed up the process of designing your API solution.

#### **Common API Styles include:**

- **Tunnel Sytyle(SOAP):** also referred to as web service style, standing for **_Simple Object Access Protocol_** which is the most well known implementation of the tunnel style. Tunneling APIs builds on the common pattern of calling functions within a programming language, but extend that pattern to remote services.
     - **SOAP usually:**
       - Exposes an RPC-like interface & provides an interface descriptor for binding.
       - Uses an XML-Centric message format.
       - Uses HTTP as a transport protocol for a higher application-level protocol.
 
- **URI style(CRUD):** CRUD which stands for _Create, Read, Update & Delete_ refers to operations performed on a resource centric via web URI. URI-Based APIs provide an intuitive, simple way for application developers to invoke requests. Well designed APIs of this style employ "hackable" URI designs, which also act as a form of self-documentation.
The reliance on HTTP protocol can also act as an advantage for client application developers who are familiar with the protocol.

**With URI Style:**
    - An object or resource-centric API is exposed.
    - URIs and query parameters are used to identify and filter objects.
    - CRUD operations are mapped to HTTPS methods

- **Hypermedia Style(REST):** REST stands for **_Representational State transfer_** which Is similar to the URI style but utilizes hypermedia( which includes rick content types, hyperlinks, and other native HTTP tooling) to create interactions focused on tasks rather than on objects.
- 
 **Some characteristics of a REST API are that it:**
   - Exposes a task-based interface, often oincorporating a workflow or state machine.
   - uses media to describe link semantics, template-based input and message structures.
   - Provides its own URIs. 

- **Event-Driven/Reactive Style:** includes the websocket protocol, which transmits data between a client and server with low overhead.

- **GraphQL:** Is a query language for APIs originally developed at Facebook(Now Meta) that was intended for flexibility of arguments. It allows client users to tell the API exactly how to present the retrieved data without needing to create a large collection of unnecessary requests or responses.

- **gRPC:** Is a HTTP2-based protocol that orignated at google, intended for high scale communication. It is language-agnostic and emphasizes a `contract-first` approach to API development, which requires client and server to agree on the payload format but allows for performance at scale.

### What is GraphQL?

GraphQL is a query language that was developed specifically for APIs. It prioritizes giving clients exactly the data they request and no more. It is designed to make APIs fast, flexible, and developer-friendly. As an alternative to REST, GraphQL gives front-end developers the ability to query multiple databases, microservices, and APIs with a single GraphQL endpoint. Organizations choose to build APIs with GraphQL because it helps them develop applications faster.

## How to create an API?
Due diligence and effort are required to build an API that other developers will want to work with and trust. These are the five steps required for high-quality API design:

1. Plan the API 
API specifications, like OpenAPI, provide the blueprint for your API design. It is better to think about different use cases in advance and ensure the API adheres to current API development standards.

2. Build the API
 API designers prototype APIs using boilerplate code. Once the prototype is tested, developers can customize it to internal specifications.

3. Test the API  
API testing is the same as software testing and must be done to prevent bugs and defects. API testing tools can be used to strength test the API against cyber attacks.

4. Document the API  
While APIs are self-explanatory, API documentation acts as a guide to improve usability. Well-documented APIs that offer a range of functions and use cases tend to be more popular in a service-oriented architecture.

5. Market the API 
Just as Amazon is an online marketplace for retail, API marketplaces exist for developers to buy and sell other APIs. Listing your API can allow you to monetize it.

### Common Challenges of API Design

- **Managing Cost:** From managing multiple gateway servers and instances to building an entire API Management program from the ground up, the wrong infrastructure approach can lead to unnecessary and unweidly expenses.

- **Scalability:** Addressing scalability early on in the process can help define early adoption, future success, and the lifespan of an API.

- **Security:** Security should be incorporated at the infrastructure level. This requires a multi-pronged approach that includes leveragig an API Gateway to easily validate, authorize and control the access of legitimate API consumers, as well as protect endpoints against malicious traffic.

### API Design Obstacles

Some obstacles that an API designer may face during the design process include;
- The perspective obstacle.
- The Bias obstalce.
- The Assumption obstacle.
- The resource obstacle.

## What is API testing?
API testing strategies are similar to other software testing methodologies. The main focus is on validating server responses. API testing includes:

- Making multiple requests to API endpoints for performance testing.
- Writing unit tests for checking business logic and functional correctness.
- Security testing by simulating system attacks. 

## API Management Concepts

Application Programming Interface management, or API management, consists of a set of tools and services that enable developers and companies to build, analyze, operate, and scale APIs in secure environments. API management can be delivered on-premises, through the cloud, or using a hybrid on-premises – SaaS (Software as a Service) approach.

### How to write API documentation?

Writing comprehensive API documentation is part of the API management process. API documentation can be auto-generated using tools or written manually. Some best practices include:

- Writing explanations in simple, easy-to-read English. Documents generated by tools can become wordy and require editing.
- Using code samples to explain functionality.
- Maintaining the documentation so it is accurate and up-to-date.
- Aiming the writing style at beginners
- Covering all the problems the API can solve for the users.

### API Change Management

In API design, change management includes Versioning APIs, and communicating what is new as well as the risks and considerations for upgrading. Teams will be providing clear release histories, to  help track new and deprecated features and bugs not matter which version a user is running.

In such instances teams will want to be able to support backward compartibility or even make upgrading or migration processes as painless as possible when choosing to deprecate features of or an entire API.

#### Define API Versioning

Because API Versioning can often be a controversial topic in the API Design Community, it's believed that if you can avoid or don't need to version then don't do it.

#### API Versioning Principles

Postel's Law is a guideline for creators of software protocols: "Be conservative in what you do, be liberal in what you acceot from others." where in a networking context, it is paraphrased as: "Be conservative in what you send, be liberal in what you accept."

#### Issues to avoid when extending the interface

Some of the "extending the interface" techniques include;-
- Never take anything away-always try to preserve what you already have.
- Never change the meaning of exsisting things-preserve the meaning.
- Make all new changes optional-don't require the client to provide a new parameter, or insist that they recognize new fields in the response.


## How to use an API?

The steps to implement a new API include:

- Obtaining an API key. This is done by creating a verified account with the API provider.
- Set up an HTTP API client. This tool allows you to structure API requests easily using the API keys received.
- If you don’t have an API client, you can try to structure the request yourself in your browser by referring to the API documentation.
- Once you are comfortable with the new API syntax, you can start using it in your code.

## Business Benefits of APIs

- APIs can be a new business channel of bringing revenue to an organisation by way of monetized access to it's data and services.
- Reach and retention.
- Faster Partnerships in situations where APIs are well-documented and usable which enables partners to onboard in record time.
- APIs are Mobile and Omnichannel meaning organisations can offer their services through APIs enabling them provide consistent digital experiences across all their business channels.
- Good Interaction Analysis made possible from having customers and partners access services through APIs thus creating a digital feedback loop that enables real-time analysis of user behavior. 
- Outsourced Innovation which is where an organisation makes available a public version of their API which can lead to innovative useage from third party developers thus benefiting the API owners.
- Self-Service Integration which enables API-enabled enterprises to allow more rapid integration of disparate business capabilities and assembly of new products.
- Realisation of Organisational Agility especially where there is adoption of "API First" engineering philosophy along with a microservice architecture maximising delivery speed, system stability and scalability.

## Where can I find new APIs?
New web APIs can be found on API marketplaces and API directories. API marketplaces are open platforms where anyone can list an API for sale. API directories are controlled repositories regulated by the directory owner. Expert API designers may assess and test a new API before adding it to their directory.  

Some popular API websites include:

- Rapid API – The largest global API market with over 10,000 public APIs and 1 million active developers on site. RapidAPI allows users to test APIs directly on the platform before committing to purchase.
- Public APIs – The platform groups remote APIs into 40 niche categories, making it easier to browse and find the right one to meet your needs.
- APIForThat and APIList – Both these websites have lists of 500+ web APIs, along with in-depth information on how to use them.   

## Introduction API Product Management

Today's connected world

The development of APIs should follow a thought process similar to developing any well-designed product with the end user in mind, who if you think about it, doesn't want to merely use an API but mostly solve a very specific problem.

API Product Management is all about knowing how to manage APIs from basic understanding of how APIs function, to designing and building APIs, to documentation best practices, API catalog management, and the basics of testing and securing APIs.

## Conclusion

APIs are mechanisms that enable two software components to communicate with each other using a set of definitions and protocols. At their simplest level, Application Programming Interfaces (APIs) enable communication between disparate software applications. Developers can connect APIs from different companies and services to achieve specific results.

Popular API uses include enabling the implementation of libraries and frameworks across languages, specifying the interface between an application and an operating system, manipulating remote resources through protocols, and defining the interface through which interactions happen between a third-party and the applications that use its assets. From independent mobile developers and web developers to large enterprises and governmental agencies, APIs are increasingly leveraged across industries and use cases.

Today, developers, enterprises, and organizations often create open APIs that allow others to integrate with their products and services. Hundreds of thousands of APIs designed to facilitate the exchange of information exist across industries. As the number of APIs continues to grow, the need for developers and enterprises to monitor and manage them in a secure and scalable way increases.

## Glossary

- **Application Programming Interfaces Abbreviated** as API...
- **API directories** are controlled repositories regulated by the directory owner. 
- **API marketplaces are open platforms where anyone can list an API for sale. 

## Resources & References

- [API Design: Step by step guide to learn how to design and build robust APIs.](https://roadmap.sh/api-design)
- [Getting Started with APIs - Postman](https://www.postman.com/what-is-an-api/)
- [What is an API (application programming interface)?](https://www.ibm.com/think/topics/api)
- [What is a RESTful API?](https://aws.amazon.com/what-is/restful-api/)
- [How to Write Good API Documentation](https://www.freecodecamp.org/news/how-to-write-good-api-docs/)
- [Discover API Security with Layer7](https://www.broadcom.com/products/software/layer7-api-security)
- [API Architecture](https://dev.to/jahid6597/api-architecture-1h9p)
- [Application And API (Presentation) Layers](https://www.linkedin.com/pulse/application-api-presentation-layers-sara-ali-scdnf/)
- [What Is API Caching? A Practical Overview for Developers](https://www.harpersystems.dev/post/what-is-api-caching-a-practical-overview-for-developers)
- [What is API orchestration?](https://www.ibm.com/think/topics/api-orchestration#:~:text=An%20orchestration%20layer%20puts%20all,to%20achieve%20a%20specific%20goal.)

## Keywords
``API``, ``Application Programming Interfaces``, ``Software``, ``Software Applications``, ``software interface``, ``Software System``, ``API design``, ``API Development``, ``API lifecycle`` ``API integrations``, ``API Management``, ``API architecture``, ``API economy``, ``API Intelligence``, ``Layer7 API Security``, ``APIOps``
