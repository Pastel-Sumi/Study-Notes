 * **Vertical Scaling:** To take a single resource like a server/computer and making it better, improving it's CPU, RAM, etc. 
* **Horizontal Scaling:** To take our server and "make more copies", in the end, this is to have more servers that can handle more requests at the same time.
Horizontal Scaling introduces the question, "how do we know which server the request should go to?". This is where **Load Balancers** come into play.
	This load balancer will be able to handle and forward the request to the less trafficked server so that each of the servers has a balanced amount of traffic.

Our servers may be connected with other servers. For example there may be a **Logging** server that logs all the requests made by users.

There could also be a **Metrics Service** at play to know more about the metrics of our servers and states.

Log-based metrics are essential because since logging are time-series we can see if there is a problem, or a tendency, etc within these metrics.

We want a push notification from the metrics so we feed our data metrics to a **Alerting Service** which tell us if a metric passes or goes below a threshold.

![[Pasted image 20260831155256.png]]
