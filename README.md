# System Design
Systems design a procedure by which we define the architecture of a system to satisfy given requirements. It is a technique by which the required amounts of scalability, reliability, performance and consistency are satisfied in real world systems.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------
## System Design Concepts
- Scalability
- Load Balancing
-
-
-





-----------------------------------------------------------------------------------------------------------------------------------------------------------------


## Scalability
  - Vertical scaling
  - Horizontal scaling

We would introduce Scalability concept by Pizza restaurant, WoW I LIKE IT SO MUCH.

![image](https://user-images.githubusercontent.com/64374947/137215027-50252638-023d-4bcf-9002-a83ff9510934.png)

Assume in this restaurant there are one chief to preparing pizaa, when we opend this restaurant there are 5 customer come per hour and chief is enable to serve them

but after month there are 30 cutomer come per hour and chief is not able to serve all these orders so manager decided to hire another 2 chief <br>
but after two weeks there are 70 customer come per hour and manager manager decided to hire another 2 chief <br>
but ... <br>
and so on.

**this solution called Vertical scaling.**

But if manager decided to **open another restaurant** to handle number of customers **this solution called Horizontal scaling.**

Purpose of Scalability handling huge number of orders.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------


## Load Balancing
Modern high‑traffic websites must serve hundreds of thousands, if not millions, of concurrent requests from users or clients and return the correct response in a fast and reliable manner.

![image](https://user-images.githubusercontent.com/64374947/137583070-5aa6df43-adf0-48a2-9490-fc381d8b496b.png)


A load balancer acts as the “traffic cop” sitting in front of your servers and routing client requests across all servers capable of fulfilling those requests in a manner that maximizes speed and capacity utilization and ensures that no one server is overworked, which could degrade performance. If a single server goes down, the load balancer redirects traffic to the remaining online servers. When a new server is added to the server group (**Horizontal scaling**), the load balancer automatically starts to send requests to it.

In this manner, a load balancer performs the following functions:
- Distributes client requests or network load efficiently across multiple servers.
- Ensures high availability and reliability by sending requests only to servers that are online.
- Provides the flexibility to add or subtract servers as demand dictates.

## Load Balancing Algorithms
Different load balancing algorithms provide different benefits; the choice of load balancing method depends on your needs:
- Round Robin – Requests are distributed across the group of servers sequentially.
- Least Connections – A new request is sent to the server with the fewest current connections to clients. The relative computing capacity of each server is factored into determining which one has the least connections.
- Least Time – Sends requests to the server selected by a formula that combines the fastest response time and fewest active connections.
- IP Hash – The IP address of the client is used to determine which server receives the request.
- Random with Two Choices – Picks two servers at random and sends the request to the one that is selected by then applying the Least Connections or the Least Time algorithm.

## Benefits of Load Balancing
- Reduced downtime
- Scalable
- Flexibility
- Efficiency
- Availability

-----------------------------------------------------------------------------------------------------------------------------------------------------------------
