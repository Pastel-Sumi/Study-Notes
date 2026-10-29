Every machine that it's going to be communicating over the public internet and sending data back and forth needs to be assigned a **public IP Address.** 
* An IP Address is how a machine identifies and distinguish another machine.
* An IP Address is a 32 bit integer and it's written usually like this `012.345.678.910` . The max number of each separation can go from `0. to 255.` With 32 bit we can have 4 billion public IPs. This is part of **IPv4** 
* **IPv6** is newer and uses 128 bit but IPv4 is still being used. 

How do we actually send the data? What are the rules of communications between computers?
* The rules to send data is called **Internet Protocol (IP)**
* The data that is being sent it's called a **packet (IP Packet)**.
	* A portion of this packet is going to be reserved for the information that's needed for the communication (this is called metadata).
	* This is what we call the **Header**: Includes the source IP address; The destination IP address, among other info.
	
![[Pasted image 20260907161512.png]]

If we were to send a lot of information, how does the server knows how to assemble/order this information? This is where **TCP (Transmission Control Protocol)** comes into play.

When we are using TCP, the data is divided into more portions:
* One of those portions it's called **TCP Header**. This is metadata of the TCP package.
	* It includes things such as the **Sequence number** of the package.  This means when the server receives all the packages it can understand the order of the packages and reassemble it.

We take TCP and IP protocol as granted. We will mostly care about the **Application Data** that we send through **HTTP**.

![[Pasted image 20260907163934.png]]

## Public vs Private IP Address

Servers need a public IP Address to be accessible in the internet. We can have multiple clients on the same Network and it will not be necessary for each one of these to have a public IP Address since the connection will be going through a **Router** which is the one that will have a public IP Address.

* This same routers are the ones that give a Private IP Address to our dispositives in our **Local Area Network (LAN)**. 
![[Pasted image 20260907164417.png]]

## Static vs Dynamic IP Address

* **Static:** As the name implies, are IP Addresses that do not change. This would be more important for the server-side.
* **Dynamic:** The IP Addresses constantly change over time.

### Ports
"Are a sort of channel of communication between machines". Machines communicate through IP address but also through Ports (443, 80, etc).
* It is a 2^16 ~ 65000 ports for machines.
* There are some specific/default ports, like HTTP using port 80, HTTPS using port 443, for example.