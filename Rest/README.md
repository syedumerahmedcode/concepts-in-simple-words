# Rest

**API**

API stands for Application Programming Interface and basically it allows one program to talk to another program.[1]

**REST**

- REST Stands for REpresentational State Transfer.
- It is an architectural style for distributed Hypermedia systems.

**6 guiding constraints of REST**

- Also known as 6 underlying constraints of REST.

- *Client-server*: The client and server are two separate systems. 
- *Stateless*: Server contains no information of client. Client contains all the necessary information for a successful call in its application state.
- *Cachable*: Cache constraints require that the data within a response to a request be implicitly or explicitly labeled as cacheable or non-cacheable. If a response is cacheable, then a client cache is given the right to reuse that response data for later, equivalent requests.
- *Layered System*: The system consists of multiple layers such that each layer only sees the immediate layer with which it is interacting.
- *Uniform interface*:  It defines a interface constraint between the client and the server.Request and responses use HTTP and HTTPS as transfer protocol. Request uses HTTP verbs like GET, PUT and so on. Response consists of HTTP status codes like 200, 404 etc.
- *Code on demand*: This constraint is optional. The server can temporarily extend client by downloading the logic from the server to the client. 
 

References:
- [1](https://www.youtube.com/watch?v=7YcW25PHnAA) REST API concepts and examples
- [2](https://restfulapi.net/) REST API Tutorial