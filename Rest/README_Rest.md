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
- Two less commonly used methods are: _OPTIONS_: It indicates which techniques are supported and _HEAD_: About the request URL it returns meta information.

**Idempotent operation**

- If an operation with the same set of inputs produces the same output even when it is called multiple times, then it is an idempotent operation.
- GET, PUT(?) and DELETE(?) are idempotent whereas POST operation is not idempotent.

**JAX-RS**

- JAX-RS stand for Java API for RESTful Web service.
- A set of Java-based APIs that are provided in the Java EE which is useful in the implementation and development of RESTful web services.

Features of JAX-RS are:

- Open link 3 for more information.

**Some key annotations**

- @Path: It represents the relative URI path to the REST resource.
- @PathParam: Defines parameters defined in the path of the URI. For example: In _.../v1/accounts/{id}_, {id} is a path parameter. This maps to _@PathVariable_ annotation in SpringBoot.
- @QueryParam: Defines parameters which are defined in the query part of a URI. For example: In _.../v1/accounts/?id=123_, id=123 is a query parameter.
- @Produces: What MIME media types are produced by the server and send to the client. For example: _MediaType.APPLICATION__JSON_.
- @Consumes: What MIME media types are consumed(i.e. accepted) by the server. 

**Authentication**

- Refers to providing correct identity.
- Authentication: Who are you?

**Authorization**

- Refers to allowing a certain action.
- Authorization: What can you do?

**Methods of Authentication**

- Basic Authentication
- Digest Access Authentication
- Asymmetric Cryptography
- OAuth
- JSON Web Tokens

**Basic Authentication**

- Every time the client wants to talk to a server using REST AP, it sends its user name and password combination.
- In the request header, one passes user name and password.
- The way to do is: on the client side, add both user name and password as _username:password_ --> Perform a Base64 encoding on this string --> Create a new header key called Authorization --> Value of Authorization: Basic _encodedBase64String_.
- Server side: Looks at first part of header and knows that it is Basic encoding--> Perform a Base64 decoding on the second part of the string-->Takes the string before the _:_ as user name-->Takes the string after the _:_ as the password--> Finally,it checks if the combination of user name and password matches with what is stored on the server.
- Encoding is just a way to convert a string into another string i.e. Encoding!=Encryption. Due to this fact, it is **not** a secure method. 
- One workaround is to always send the encoded string via HTTPS.
- Why encode? The intent of the encoding is _to encode non-HTTP compatible characters_ that may be in the user name and password into those that are HTTP-compatible.


**Disadvantages of Basic Authentication**

- It is subject to replay attacks.
- No encryption performed.







References:
- [1](https://www.youtube.com/watch?v=7YcW25PHnAA): REST API concepts and examples
- [2](https://restfulapi.net/): REST API Tutorial
- [3](https://www.interviewbit.com/rest-api-interview-questions/): REST API Basic Interview Questions
- [4](https://www.youtube.com/watch?v=501dpx2IjGY): Advanced JAX-RS 22 - REST API Authentication Mechanisms
 	 	 