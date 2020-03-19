# Coding Tips
Summary containing notes on different languages and technologies.

## Table of Contents
1. [Development Resources](#development-resources)
2. [Python](./Python/README.md)
3. [Java](./Java/README.md)
4. [Design Patterns](./Python/README.md)
5. [Go](./Go/README.md)

## Development Resources

### Timeouts
Use timeouts to return a thread so it can be released.  
Avoid using threads for extended periods of time.  
Timeouts have to be aggressive(short time).  
Implement timeouts for clients and between services.  

### Test Driven Development

It is a cycle by switching between laws.  
You want to debug like if the code worked a minute ago.  
Unit tests are independent rules of code that show how the logic of the system must be.  

__The Tree Laws of TDD__

1. YOU ARE NOT ALLOWED TO WRITE ANY PRODUCTION CODE UNLESS IT IS TO MAKE A FAILING UNIT TEST PASS  

2. YOU ARE NOT ALLOWED TO WRITE ANY MORE OF A UNIT TEST THAN IS SUFFICIENT TO FAIL;
 AND COMPILATION FAILURES ARE FAILURES  

3. YOU ARE NOT ALLOWED TO WRITE ANY MORE PRODUCTION CODE THAN IS SUFFICIENT TO PASS THE ONE FAILING UNIT TEST  


### From Monolithic to Microservices

Before refactoring any application to microservices you first have to solve any problem the app has.

- Do CI/CD in monolithic apps before doing any migration.
- Watch out for high latency between services.
- Use CorrelationIDs and Mapped Diagnostic Context.
- Make sure the code is loosely coupled and highly cohesive, use the SOLID principles and Command Query Responsibility Segregation.


