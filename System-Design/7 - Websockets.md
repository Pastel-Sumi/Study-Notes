HTTP has some limitations. That's why there are some protocols that fill the gaps:
* **FTP (File Transfer Protocol):** As the name implies, it's for transfering large files between computers. It runs on port 21.
* **SMTP (Secure Mail Transfer Protocol):** By default runs on port 25. Optimized for sending emails.
* **SSH (Secure Shell):** To remotely connect to another machine.
* **WebRTC:** For video and audio streaming. 

How do we load the chat of a stream in real time? Do we send an HTTP request every minute? But this doesn't bring us the most recent messages. There is a more direct and efficient way, and that is through **WebSockets**.

We first call a WebSocket handshake, where the client would send an HTTP request and that request is to establish a WebSocket connection.

The server would respond with a 101 and upgrades the connection into a WebSocket connection. We can send information in both directions. With HTTP usually the client initializes the request. Multiple messages can be sent and that information doesn't really need an answer. This is **bidirectional communication**.

Maybe the connection between the client and server could break at some point.
![[Pasted image 20260916165935.png]]

Polling.