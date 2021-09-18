# Rest

**API**

API stands for Application Programming Interface and basically it allows one program to talk to another program.

**REST**

- REST Stands for REpresentational State Transfer.
- It is an architectural style for distributed Hypermedia systems.

**Advantages of REST**

- REST is a lightweight protocol compared to SOAP.
- No contract is defined between a client and the server. Hence, it is loosely coupled.
- REST supports multiple technologies for data transfer such xml , json, text, image etc. whereas SOAP supports xml but not json. 

**6 guiding constraints of REST**

- Also known as 6 underlying constraints of REST.

- *Client-server*: The client and server are two separate systems. 
- *Stateless*: Server contains no information of client. Client contains all the necessary information for a successful call in its application state.
- *Cachable*: Cache constraints require that the data within a response to a request be implicitly or explicitly labeled as cacheable or non-cacheable. If a response is cacheable, then a client cache is given the right to reuse that response data for later, equivalent requests.
- *Layered System*: The system consists of multiple layers such that each layer only sees the immediate layer with which it is interacting.
- *Uniform interface*:  It defines a interface constraint between the client and the server.Request and responses use HTTP and HTTPS as transfer protocol. Request uses HTTP verbs like GET, PUT and so on. Response consists of HTTP status codes like 200, 404 etc.
- *Code on demand*: This constraint is optional. The server can temporarily extend client by downloading the logic from the server to the client. 

**Resource**

- Any information that can be named is a resource. For example: A document, image, collection of other resources etc. Resources are identified with: their URI, HTTP methods they support, and request/response data type and format of data.

**Purpose of URL**

- URL is used to identify where the resource is located.

**URI**

- URI stands for Uniform Resource Identifier.
- Used for identifying a resource.
- It has the following format: 

```

<protocol>://<service-name>/<ResourceType>/<ResourceId>

```
. For example: http://maps.googleapis.com/maps/api/geocode/json. Here: 

```
<protocol>://<service-name>/<ResourceType>/<ResourceId>

<service-name>==> maps.googleapis.com
```

whereas 

```
<ResourceType>==>/maps, /api, /geocode and /json.
```


**What are REST methods**

- Rest methods are used to access Rest resources.
- One can invoke GET,POST,PUT,DELETE etc on this URL to invoke the resource.
- POST is used for insertion whereas PUT is used for modifying a resource.

**Idempotent operation**

- If an operation with the same set of inputs produces the same output even when it is called multiple times, then it is an idempotent operation.
- GET, PUT(?) and DELETE(?) are idempotent whereas POST operation is not idempotent.

**JAX-RS**

- JAX-RS stand for Java API for RESTful Web service.
- A set of Java-based APIs that are provided in the Java EE which is useful in the implementation and development of RESTful web services.

Features of JAX-RS are:

- Open link 3 for more information.

**Some key annotations**

- 








References:
- [1](https://www.youtube.com/watch?v=7YcW25PHnAA): REST API concepts and examples
- [2](https://restfulapi.net/): REST API Tutorial
- [3](https://www.interviewbit.com/rest-api-interview-questions/): REST API Basic Interview Questions