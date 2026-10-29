* Many applications today are _data-intensive_, as opposed to _compute-intensive_. Raw CPU power is rarely a limiting factor for these applications.
A data-intensive application is typically built from standard building blocks that provide commonly needed functionality. For example, many applications need to:
* Store data so that they, or another application, can find it again later (_databases_)
* Remember the result of an expensive operation, to speed up reads (_caches_)
* Allow users to search data by keyword or filter it in various ways (_search indexes_)
* Send a message to another process, to be handled asynchronously (_stream processing_)
* Periodically crunch a large amount of accumulated data (_batch processing_).

We will start by exploring the fundamentals of what we are trying to achieve: reliable, scalable, and maintainable data systems.

## Thinking about Data Systems
![[Pasted image 20260818220207.png]]

Many new tools for data storage and processing have emerged in recent years. They are optimized for a variety of different use cases, and they no longer neatly fit into traditional categories. For example, there are datastores that are also used as message queues (Redis), and there are message queues with database-like durability guarantees(Apache Kafka). The boundaries between the categories are becoming blurred.

When you combine several tools in order to provide a service, the service’s interface or application programming interface (API) usually hides those implementation details from clients. Now you have essentially created a new, special-purpose data system from smaller, general-purpose components.

pag 27
