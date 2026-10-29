* **API (Application Programming Interface):** Any type of programming interface. 
For example to access the **Local Storage** of our browser (that stores the info of the user in the browser) we use an API.

Most commonly API is used to indicate some external service (HTTP). 
The 3 most important and common paradigms:
* **REST**
* **GraphQL**
* **gRPC**

## REST (REpresentation State Transfer)
They are built on top of HTTP. REST is not a protocol but more of a set of restrictions/standarizations that we apply to HTTP APIs.

* REST APIs are **stateless**.
What is an example of something having a state? Imagine we have this endpoint: `https://youtube.com/videos` as a GET endpoint. **Every REST endpoint is associated with something called a resource, a noun**, for example `videos` in this case. A state would be if the server has info/a session of every user it interacts with.

"The server should not have to manage any state related to the user"
Stateless basically means that from the perspective of the server there is no state being stored in the server itself.
* In the browser there will be some form of state, with cookies or session storage.

We use **pagination** instead of saving up the state. We send this information in every request. For example we would have a **query parameter** in the url of our query (in a ? symbol). For example:
`GET https://youtube.com/videos?limit=10?offset=0` where offset is the point "where we start". Like if we imagine that we already saw the first 10 videos then the offset will be 10

Why do we do this?
Imagine that if a page had multiple servers, and if a load balancer sends our requests to different servers then they might not have our info yet. This is why REST is stateless and the info is sent through the query via the query parameters.

* **JSON (JavaScript Object Notation)** is the most important and used data type in REST APIs

![[Pasted image 20260919183318.png]]

## GraphQL
It's not a protocol, it's actually built on top of HTTP but it only uses POST requests because we need to send data through a Body and we already discussed that GET requests have no body.
* In the body of the requests we include a Query which exactly tells what resources we want from the server.
* GraphQL solves the problem of **Overfetching** (fetching too much information).
* We can specify which fields of each resource we want
* We have a single endpoint in GraphQL
* We have two operations we can do:
	* **Query**: An operation where we read and don't modify any data on the server.
	* **Mutation:** Any type of mutation we do to the data, create or modify data on the server.
* The endpoints in GraphQL are built on top of POST requests, which are not Idempotent in HTTP. The downside of this is that we can't cache requests.
![[Pasted image 20260920232211.png]]

## gRPC

* Built on top of HTTP/2.
* It cannot be used directly from the browser so we use a proxy or gRPC - Web.
* Normally used for Server-to-Server connections
* In terms of performance it is faster than REST APIs because we send information in **Protocol Buffers**, essentially schema objects. These objects are serialized in a binary format.
* It allows to stream data from the client to the server and viceversa
* gRPC doesn't make use of HTTP codes.
![[Pasted image 20260920233256.png]]
