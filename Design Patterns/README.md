# Design Patterns

## Table of Contents
1. [Bulkhead](#bulkhead)
2. [Circuit Breaker](#circuit-breaker)
3. [Observer](#observer)
4. [Singleton](#singleton)


### Bulkhead

Provides protection from cascading failures, only if the size of 
the bulkhead is significantly smaller than the request pool size.   
Provides protection from overload to the services.  
Contains failures by partitioning. 
Limits the resources to specific groups.  

__Partition by client__  
Clustering services for different clients.

__Resources by application__  
Clustering by microservices.

__Resources by operation__    
Limit the threads.
 

It can be implemented by using semaphores.

The most important metrics are:
- Number of calls to the services
- Timeout ratio
- Rejected calls ratio
- Circuit break ratio
- Success/Fail ratio
- Response time



### Circuit Breaker

Circuit breakers are more proactive than a timeout.

They avoid calling a failing service.

They return errors immediately after detecting the service is unavailable until the problem is solved.

You must calculate the number of timeouts in a time period.



### Observer

Defines a one-to-many dependency between objects so that when one object changes state, all of its dependents are notified and updated automatically.

The observables, update observers using a common interface.

Observers are loosely coupled in that the observable knows nothing about them, other than that they implement the observer interface.



### Singleton

A class that can be constructed only once



