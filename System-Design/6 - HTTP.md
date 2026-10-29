It is an **Application Layer Protocol**.

## Client-Server Model
An assumption that has been made is that the client is going to be some end-user that it's using a laptop/computer. 

* Client is a general term, basically is "the one that makes the requests".
* The server is not a end-user machine but it's the one that fulfill the requests.
* It really depends on this which one is the "Client" and which one is the "server".

## RPC (Remote Procedure Call)
We mentioned moving data between machines. 
* We communicate via code.
* The way multiple machines talk to each other remotely over a network is via a **Remote Procedure Call**.
* Just like a function call.
* For example, we use RPC to execute a code that it's on the server.

![[Pasted image 20260908224150.png]]


## HTTP (HYPERTEXT TRANSFER PROTOCOL)

An application protocol that is built on top of IP and TCP.
* It is a **request-response protocol.** The client makes a request and the server replies with a response.
* **HTTPS** is a variation of HTTP that it's more secure.

In dev tools h3 in protocol means HTTP3.
Every HTTP request has two main components:
* **Headers**: There are 3 main groups of headers.
	* **General Headers:** Includes basic info like the url of where we send the request to; There is also the **request method (GET, POST, PUT, DELETE, etc)**. There is also the **status code**.
	* **Request Headers:** What the requester client it's actually going to send. Content type; Among others.
	* **Response Headers:** This says what the content type was actually return.
* **Body** of the request.


## Methods: GET, POST, PUT, DELETE
We know that every request has to go to an url (a **Route** in an API). This same route could serve multiple HTTP methods
* **Endpoint:** A route in an API that serves/responds to an HTTP request method (`Ex: http;//youtube.com GET`).
* `GET`: Usually used to retrieve information. Don't have bodies, only headers. Idempotent.
* `POST`: For creating information.
* `PUT`: Update information.
* `DELETE`: Deleting information. 

## Status Codes
Very useful for developers. They tell us if a request went well or if something unexpected happened.

![[Pasted image 20260915161116.png]]

### SSL / TLS 
HTTP is not necessarily secure, that's why we add the S (Secure) to make it HTTPS.  SSL and TLS encript everything you send over HTTP.
* **SSL (SECURE SOCKET LAYER):** Outdated but still mentioned. Now TLS is used.
* **TLS (TRANSPORT LAYER SECURITY)**.