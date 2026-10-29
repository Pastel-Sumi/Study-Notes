Transport layer protocols.

## Internet Procol Suite
It's more commonly referred to **TCP/IP** which means that TCP is running on top of IP.

* **TCP:** The ordering of the data does indeed matter. That being said how the server that receives it knows how to reassemble it? TCP handles the ordering
	* An important benefit of TCP is that is **Reliable**.
	* What if a package is missing? Then that package gets resend. This is called **Retransmission of Lost Packages**.
	* This is possible because TCP actually establishes a two-way connection between machines that are communicating.
	* TCP establishes something called a **3-Way Handshake**. Which is kind of expensive since it requires to send a couple of messages between the connected machines: A **SYN** message and an **ACK** message.
![[Pasted image 20260907170242.png]]

* **UDP(USER DATAGRAM PROTOCOL):** Datagram is the word used for package.
	* The benefits of UDP is that we don't need to establish a connection. A handshake it's not necessary. The server just starts sending data.
	* The data is not ordered.
	* It's a lot faster than TCP
	* Most popular use it's on streaming data.
	* It's also used on DNS
	![[Pasted image 20260908215848.png]]
