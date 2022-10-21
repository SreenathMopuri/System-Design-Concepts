# Fundamentals of Distributed Systems
Nowadays, almost every large-scale application is based in distributed computing. So understanding distributed system concepts 
is crucial in designing fault-tolerant, highly scalable, and low-latency srvices. 

## What is Distributed System ? How does it Work?
A distributed system is a collection of independent software components or machines that work together as a single
system for the end user. These components are spread across multiple computer connected by a local or a wide area 
network and exchange messages to complete tasks efficiently. Most of the time, these components operate concurrently
and fail independently without affecting the system's performance.

Distributed systems can process large numbers of requests and manage millions of users at the same time. Because several
machines can perform the same task concurrently, if one machine is unavialble, the others keep the system running, ensuring
fault tolerance and reliability. They are easily scalable and significantly increase performance as well.

For example, suppose we are using traditional databases stored on a single machineto perform read and write operations. 
If the volume of data increases, the query performance will decrease. One solution is to partition the database system on multiple machines.
If read traffic is much more than write traffic, we can use master-slave replication to handle read and write requests separately.

So it is evident that such systems consist of considerable complexity. The critical question is: Why are we using distributed systems if they are challenging
to manage? Think!

## Scalability in a distributed System

One of the major advantages of adopting distributed systems is their ability to provide highly scalable services. Such systems can continuously evolve 
to support growing workloads like handling a large number of user requests or a large number of database transactions. So the goal of a scalable distributed
system is to achieve high scalability without performance loss.

Generally, the performance of a system declines with the increase in system size. For example, network speed may become slower because nodes tend to be 
far apart, performance may decrease due to increased user traffic, etc. So scalable distributed systems avoid such a situation and evenly balance the 
incoming load among all available nodes.

Traditional systems generally scale using `Vertical Scaling`, i.e., by adding more power(CPU, RAM, Storage, etc.) to an existing server. Such vertical 
scalable services are incompatible when operating on a vast scale because they are expensive and more prone to a single point of failure. This is 
usually limited to the capacity of a single server and scaling beyond that capacity often involves downtime.

However, `horizontal scaling` allows us to scale indefinitely by adding more servers tothe pool of resources. If there is any performance degradation, 
we only need to add more machines, making the service extremely fast without much overhead costcompared to vertical scaling.

The figure below describes how much a company costs to use Vertical vs Horizontal Scaling.
![Vertical vs Horizontal Scale](Vertical_vs_Horizonal_Scale.png)


