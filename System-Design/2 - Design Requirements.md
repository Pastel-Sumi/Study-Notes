Our goal is to design effective systems to solve very big problems. 

* We have to weight the trade-offs and figure out which option is the best.

At a high level all systems are doing:
1) **Move Data**: We already talked about how data moves between the CPU, RAM and Disk. In larger systems the data could be running across different machines, even on different sides of the world.
2) **Store Data**: We already talked about how storing data on RAM is different than storing it on Disk.  In the terms of data algorithms it is the same, Arrays and binary trees have their own uses and trade-offs. But in large systems we usually store the data on Data Bases, or Blob Stores or distributed systems. These also have their different trade-offs.
3) **Transform Data**: As an example we can take logs and calculate the % of successful or failed requests.

"Bad design choices in our application architecture are very difficult to correct later".

## What is good design?

We have to think in terms of **trade-offs**. But how do we measure these trade-offs?
* **Availability**: Mathematically this could be represented as the `total_uptime/(uptime + downtime)` of our server/application/service.
	* Ej: 23 hour / 24 hour = 96%. The availability of our service was 96%
	We want our availability as higher as possible. The 100% availability it's theoretically impossible.

![[Pasted image 20260831161514.png]]

Availability is measured in terms of 9's -> 99%, 99.9%, 99.99%, etc etc...

Availability is commonly used to define **SLO (SERVICE LEVEL OBJECTIVE)**. Since we are developers we want to target something, an objective of sorts.

**SLA (SERVICE LEVEL AGREEMENT)** is the SLO + other agreements made with the customer.

## Other important terms

* **Reliability:** Probability that a system won't fail.
![[Pasted image 20260901141531.png]]
By adding more servers we can increase the reliability.

* **Fault Tolerance:** If one portion of our system has a fault then our system keeps working. The system it's tolerant to faults of portions of it.
* **Redundancy:** We don't need more servers, they are redundant between them since they are doing the same. But at the same time this helps us because in the event of a fault/failure we have multiple copies so we can still do what we need to do, and our system keeps working.

These 3 terms are entagled with each other and dependant between them.

* **Throughput:** The amount of operations or data we can handle over some period of time.  
![[Pasted image 20260901143138.png]]
Databases have the same problems as servers:
* We can vertically scale it but this has limitations.
* We can horizontally scale it but this means the data has to be copied to each DB and things get complicated. We can sync them but this adds another layer of complexity, specially when these DBs are on opposite parts of the world.

![[Pasted image 20260901143634.png]]
Depending on the context, it can be useful to measure throughput in terms of data transfered/second. Maybe our system transforms data so this kind of measure it's important.

* **Latency:** The amount of time it takes an operation to complete. It doesn't necessarily includes the network it's being used as one of the factors.
	* To reduce the latency we can once again add more servers but in different parts of the world
![[Pasted image 20260901144309.png]]
