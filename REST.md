# REST Architecture

## Introduction

REST stands for Representational State Transfer. It is an architectural style used to build web services that allow applications to communicate with each other over a network. It commonly uses HTTP to exchange data between clients and servers. REST APIs are widely used in Java Full Stack development to connect frontend applications with backend services.

## Key Concepts of REST Architecture

1. **Client-Server Architecture:** The client handles the user interface, while the server manages business logic and data. Both can develop independently.

2. **Stateless Communication:** Every request must contain all the information required by the server. The server does not store client session state between requests.

3. **Resource-Based:** Everything is treated as a resource, such as users, products, or orders. Each resource is identified using a URL.

4. **Uniform Interface:** REST uses standard HTTP methods to perform operations:
   - GET – Retrieve data.
   - POST – Create new data.
   - PUT – Replace existing data.
   - PATCH – Partially update data.
   - DELETE – Remove data.

5. **Cacheable:** Responses can be cached to reduce unnecessary requests and improve application performance.

6. **Layered System:** Communication can pass through different layers, such as proxies, gateways, and load balancers, without the client needing to know about them.

7. **Code on Demand (Optional):** A server can optionally send executable code to the client.

## REST API in Java Full Stack

In Java Full Stack development, Spring Boot makes it easier to build REST APIs using annotations such as `@RestController`, `@GetMapping`, and `@PostMapping`. A frontend application built using React can communicate with these APIs, while the backend processes requests and interacts with a database.

For example, when a user logs into an application, React sends login credentials to a Spring Boot REST API. The backend validates the credentials and sends an appropriate response, usually in JSON format.

## Conclusion

REST architecture makes communication between frontend and backend applications simple, scalable, and flexible. Understanding REST is important for Java Full Stack developers because it is commonly used when building real-world web applications.

## References

* [Roy Fielding's REST Architectural Style](https://ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm)
* [MDN - HTTP Request Methods](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods)
* [Spring - Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
